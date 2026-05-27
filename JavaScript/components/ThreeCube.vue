<template>
  <div ref="container" class="w-full h-full rounded" />
</template>

<script setup>
import { ref, onMounted, onBeforeUnmount } from 'vue'
import * as THREE from 'three'

const container = ref(null)
let renderer, animationId

onMounted(() => {
  const w = container.value.clientWidth
  const h = container.value.clientHeight

  const scene = new THREE.Scene()

  const camera = new THREE.PerspectiveCamera(80, w / h, 0.1, 1000)
  camera.position.z = 5

  // ❌ alpha: true supprimé — on garde le fond original
  renderer = new THREE.WebGLRenderer({ antialias: true })
  renderer.setSize(w, h)
  container.value.appendChild(renderer.domElement)

  // ===== Fond dégradé (code original du collègue) =====
  const backgroundGeometry = new THREE.PlaneGeometry(20, 20)
  const backgroundColors = []
  const nightBlue = new THREE.Color(0x0A1026)
  const cyberPurple = new THREE.Color(0x6D28D9)
  const backgroundPosition = backgroundGeometry.getAttribute('position')

  for (let i = 0; i < backgroundPosition.count; i++) {
    const y = backgroundPosition.getY(i)
    const mixedColor = nightBlue.clone().lerp(cyberPurple, (y + 10) / 20)
    backgroundColors.push(mixedColor.r, mixedColor.g, mixedColor.b)
  }
  backgroundGeometry.setAttribute('color', new THREE.Float32BufferAttribute(backgroundColors, 3))

  const background = new THREE.Mesh(
    backgroundGeometry,
    new THREE.MeshBasicMaterial({ vertexColors: true, side: THREE.DoubleSide })
  )
  background.position.z = -5
  scene.add(background)

  // ===== Cube principal =====
  const geometry = new THREE.BoxGeometry()
  const colors = []
  const beige = new THREE.Color(0xE8D3B0)
  const turquoise = new THREE.Color(0x14B8A6)
  const positionAttribute = geometry.getAttribute('position')

  for (let i = 0; i < positionAttribute.count; i++) {
    const y = positionAttribute.getY(i)
    const mixedColor = beige.clone().lerp(turquoise, y + 0.5)
    colors.push(mixedColor.r, mixedColor.g, mixedColor.b)
  }
  geometry.setAttribute('color', new THREE.Float32BufferAttribute(colors, 3))

  const cube = new THREE.Mesh(
    geometry,
    new THREE.MeshStandardMaterial({ vertexColors: true })
  )
  scene.add(cube)

  const light = new THREE.DirectionalLight(0xffffff, 1)
  light.position.set(2, 2, 5)
  scene.add(light)

  // ===== Petit cube en orbite =====
  const orbitGroup = new THREE.Group()
  scene.add(orbitGroup)

  const smallCube = new THREE.Mesh(
    new THREE.BoxGeometry(0.3, 0.3, 0.3),
    new THREE.MeshStandardMaterial({ color: 0x3b82f6 })
  )
  smallCube.position.x = 2
  orbitGroup.add(smallCube)

  // ===== Animation =====
  function animate() {
    animationId = requestAnimationFrame(animate)
    cube.rotation.y += 0.01
    cube.rotation.x += 0.01
    cube.rotation.z += 0.01
    smallCube.rotation.x += 0.03
    smallCube.rotation.y += 0.03
    orbitGroup.rotation.y += 0.01
    renderer.render(scene, camera)
  }
  animate()
})

onBeforeUnmount(() => {
  cancelAnimationFrame(animationId)
  renderer?.dispose()
})
</script>