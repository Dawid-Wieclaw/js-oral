---
theme: default
background: '#1A1A2E'
class: text-white
highlighter: shiki
lineNumbers: false
fonts:
  sans: 'Inter'
  mono: 'Fira Code'
---

<div class="flex items-center gap-8 h-full">
  <div class="bg-yellow-400 w-40 h-40 flex items-center justify-center rounded-sm shadow-xl">
    <span class="text-6xl font-black text-gray-900">JS</span>
  </div>
  <div>
    <h1 class="text-6xl font-black text-white">JavaScript</h1>
    <p class="text-yellow-400 text-2xl italic mt-2">Histoire, Usages & Frameworks</p>
    <div class="mt-6 h-px w-80 bg-gray-500"></div>
    <div class="mt-4 flex gap-6 text-sm text-gray-400">
      <span>👤 [Dawid] — Histoire</span>
      <span>👤 [Ndoumbe] — Usages</span>
      <span>👤 [Jérôme] — Frameworks</span>
    </div>
  </div>
</div>

---
layout: default
background: '#1A1A2E'
---

# <span class="text-white">Plan</span>

<div class="grid grid-cols-3 gap-6 mt-8">
  <div class="bg-yellow-400 rounded p-6 text-gray-900">
    <div class="text-5xl font-black">01</div>
    <div class="font-bold text-lg mt-3">Histoire & Création</div>
    <div class="text-sm mt-2 opacity-70">Origines, Brendan Eich, ECMAScript, évolution</div>
    <div class="text-xs mt-3 font-bold">[Dawid]</div>
  </div>
  <div class="bg-blue-900 rounded p-6">
    <div class="text-5xl font-black text-yellow-400">02</div>
    <div class="font-bold text-lg mt-3 text-white">Utilisations Aujourd'hui</div>
    <div class="text-sm mt-2 text-gray-400">Front-end, Back-end, Mobile, IoT</div>
    <div class="text-xs mt-3 font-bold text-yellow-400">[Ndoumbe]</div>
  </div>
  <div class="bg-blue-900 rounded p-6">
    <div class="text-5xl font-black text-yellow-400">03</div>
    <div class="font-bold text-lg mt-3 text-white">Frameworks & Three.js</div>
    <div class="text-sm mt-2 text-gray-400">React, Vue, Angular, démo live</div>
    <div class="text-xs mt-3 font-bold text-yellow-400">[Jérôme]</div>
  </div>
</div>

---
layout: default
background: '#1A1A2E'
---

<div class="flex items-center gap-3 mb-1">
  <span class="bg-yellow-400 text-gray-900 font-bold px-3 py-1 rounded text-xs">PARTIE 1 · [Dawid]</span>
  <span class="text-gray-500 text-sm">Histoire & Création</span>
</div>

# <span class="text-white">La Naissance — 1995</span>

<div class="grid grid-cols-2 gap-8 mt-4">
  <div>
    <h3 class="text-yellow-400 font-bold mb-3">Le contexte</h3>
    <ul class="text-gray-200 space-y-2 text-sm">
      <li>🌐 Netscape Navigator domine le marché du web</li>
      <li>📄 Les pages sont 100% statiques — aucune interaction</li>
      <li>☕ Sun Microsystems propose Java, trop complexe pour les designers</li>
      <li>🎯 Netscape veut un petit langage simple, accessible à tous</li>
    </ul>
    <h3 class="text-yellow-400 font-bold mt-5 mb-3">La mission</h3>
    <ul class="text-gray-200 space-y-2 text-sm">
      <li>👤 <strong class="text-white">Brendan Eich</strong> recruté en avril 1995</li>
      <li>⚡ Prototype complet en <strong class="text-white">10 jours</strong> seulement</li>
      <li>🏷️ <strong class="text-white">Mocha</strong> → LiveScript → <strong class="text-yellow-400">JavaScript</strong></li>
      <li>📣 Nom "JavaScript" : stratégie marketing liée à Java</li>
    </ul>
  </div>
  <div class="bg-blue-900 rounded p-5 flex flex-col items-center justify-center">
    <div class="w-20 h-20 bg-blue-800 rounded-full flex items-center justify-center mb-3">
      <span class="text-3xl font-black text-yellow-400">B.E.</span>
    </div>
    <p class="font-bold text-white text-lg">Brendan Eich</p>
    <p class="text-yellow-400 text-sm italic mb-4">Créateur de JavaScript</p>
    <div class="space-y-2 w-full">
      <div class="bg-blue-800 rounded px-3 py-2 text-xs text-gray-300 text-center">Inspiré de <strong class="text-white">Java</strong> pour la syntaxe</div>
      <div class="bg-blue-800 rounded px-3 py-2 text-xs text-gray-300 text-center">Inspiré de <strong class="text-white">Scheme</strong> pour les fonctions</div>
      <div class="bg-blue-800 rounded px-3 py-2 text-xs text-gray-300 text-center">Inspiré de <strong class="text-white">Self</strong> pour les prototypes</div>
    </div>
  </div>
</div>

---
layout: default
background: '#1A1A2E'
---

<div class="flex items-center gap-3 mb-1">
  <span class="bg-yellow-400 text-gray-900 font-bold px-3 py-1 rounded text-xs">PARTIE 1 · [Dawid]</span>
  <span class="text-gray-500 text-sm">Histoire & Création</span>
</div>

# <span class="text-white">Standardisation & ECMAScript</span>

<div class="grid grid-cols-2 gap-8 mt-4">
  <div>
    <h3 class="text-yellow-400 font-bold mb-3">La guerre des navigateurs</h3>
    <ul class="text-gray-200 space-y-2 text-sm">
      <li>⚔️ Microsoft crée <strong class="text-white">JScript</strong> — copie de JS pour Internet Explorer</li>
      <li>💥 Code incompatible d'un navigateur à l'autre</li>
      <li>😤 Les développeurs doivent coder deux fois</li>
      <li>📜 1997 : <strong class="text-white">Ecma International</strong> publie la norme ECMAScript</li>
      <li>✅ Garantit la compatibilité cross-browser</li>
    </ul>
  </div>
  <div>
    <h3 class="text-yellow-400 font-bold mb-3">Les grandes versions</h3>
    <table class="text-sm w-full">
      <thead>
        <tr class="text-yellow-400 border-b border-gray-600">
          <th class="text-left pb-2">Version</th>
          <th class="text-left pb-2">Année</th>
          <th class="text-left pb-2">Apport clé</th>
        </tr>
      </thead>
      <tbody class="text-gray-200">
        <tr class="border-b border-gray-800"><td class="py-1">ES3</td><td>1999</td><td>Base stable, regex</td></tr>
        <tr class="border-b border-gray-800"><td class="py-1">ES5</td><td>2009</td><td>strict mode, JSON</td></tr>
        <tr class="border-b border-gray-800"><td class="py-1 text-yellow-400 font-bold">ES6</td><td class="text-yellow-400">2015</td><td class="text-yellow-400">Classes, arrow fn, promesses</td></tr>
        <tr><td class="py-1">ES2017+</td><td>annuel</td><td>async/await, modules</td></tr>
      </tbody>
    </table>
  </div>
</div>

---
layout: default
background: '#1A1A2E'
---

<div class="flex items-center gap-3 mb-1">
  <span class="bg-yellow-400 text-gray-900 font-bold px-3 py-1 rounded text-xs">PARTIE 1 · [Dawid]</span>
  <span class="text-gray-500 text-sm">Histoire & Création</span>
</div>

# <span class="text-white">Caractéristiques du Langage</span>

<div class="grid grid-cols-3 gap-4 mt-6">
  <div class="bg-blue-900 rounded p-4">
    <div class="text-yellow-400 font-bold mb-2">⚙️ Interprété (JIT)</div>
    <p class="text-gray-300 text-xs">Compilé à la volée par le moteur — V8 (Chrome), SpiderMonkey (Firefox), JavaScriptCore (Safari)</p>
  </div>
  <div class="bg-blue-900 rounded p-4">
    <div class="text-yellow-400 font-bold mb-2">🔄 Event Loop</div>
    <p class="text-gray-300 text-xs">Mono-thread mais non-bloquant grâce à la boucle événementielle — gère l'asynchrone</p>
  </div>
  <div class="bg-blue-900 rounded p-4">
    <div class="text-yellow-400 font-bold mb-2">🎲 Typage dynamique</div>
    <p class="text-gray-300 text-xs">Types déterminés à l'exécution — flexible mais source d'erreurs subtiles</p>
  </div>
  <div class="bg-blue-900 rounded p-4">
    <div class="text-yellow-400 font-bold mb-2">🧬 Orienté Prototype</div>
    <p class="text-gray-300 text-xs">Pas de classes traditionnelles à l'origine — héritage via la chaîne de prototypes</p>
  </div>
  <div class="bg-blue-900 rounded p-4">
    <div class="text-yellow-400 font-bold mb-2">🧩 Fonctionnel</div>
    <p class="text-gray-300 text-xs">Les fonctions sont des citoyens de première classe — passées en argument, retournées</p>
  </div>
  <div class="bg-yellow-400 rounded p-4">
    <div class="text-gray-900 font-bold mb-2">🏆 Langage #1</div>
    <p class="text-gray-800 text-xs">StackOverflow 12 ans de suite — 98% des sites web — 3M+ packages npm</p>
  </div>
</div>

---
layout: default
background: '#1A1A2E'
---

<div class="flex items-center gap-3 mb-1">
  <span class="bg-blue-500 text-white font-bold px-3 py-1 rounded text-xs">PARTIE 2 · [Ndoumbe]</span>
  <span class="text-gray-500 text-sm">Utilisations Aujourd'hui</span>
</div>

# <span class="text-white">Le Web Front-End</span>

<div class="grid grid-cols-2 gap-8 mt-4">
  <div>
    <h3 class="text-yellow-400 font-bold mb-3">Le rôle fondamental</h3>
    <ul class="text-gray-200 space-y-2 text-sm">
      <li>🌐 <strong class="text-white">Seul langage natif</strong> des navigateurs — pas d'alternative</li>
      <li>🎨 Manipulation du <strong class="text-white">DOM</strong> — modifier HTML/CSS en temps réel</li>
      <li>👆 Gestion des événements : clics, scroll, formulaires</li>
      <li>📡 <strong class="text-white">AJAX</strong> — données sans rechargement de page</li>
      <li>✨ Animations, transitions, drag & drop</li>
    </ul>
  </div>
  <div>
    <h3 class="text-yellow-400 font-bold mb-3">Applications concrètes</h3>
    <div class="grid grid-cols-2 gap-2">
      <div class="bg-blue-900 rounded p-3 text-center text-sm">
        <div class="text-xl mb-1">🗺️</div>
        <div class="text-white font-bold">Google Maps</div>
        <div class="text-gray-400 text-xs">Carte interactive</div>
      </div>
      <div class="bg-blue-900 rounded p-3 text-center text-sm">
        <div class="text-xl mb-1">📧</div>
        <div class="text-white font-bold">Gmail</div>
        <div class="text-gray-400 text-xs">Interface dynamique</div>
      </div>
      <div class="bg-blue-900 rounded p-3 text-center text-sm">
        <div class="text-xl mb-1">🐦</div>
        <div class="text-white font-bold">Twitter/X</div>
        <div class="text-gray-400 text-xs">Feed en temps réel</div>
      </div>
      <div class="bg-blue-900 rounded p-3 text-center text-sm">
        <div class="text-xl mb-1">📺</div>
        <div class="text-white font-bold">YouTube</div>
        <div class="text-gray-400 text-xs">Lecteur vidéo</div>
      </div>
    </div>
  </div>
</div>

---
layout: default
background: '#1A1A2E'
---

<div class="flex items-center gap-3 mb-1">
  <span class="bg-blue-500 text-white font-bold px-3 py-1 rounded text-xs">PARTIE 2 · [Ndoumbe]</span>
  <span class="text-gray-500 text-sm">Utilisations Aujourd'hui</span>
</div>

# <span class="text-white">Au-delà du Navigateur</span>

<div class="grid grid-cols-3 gap-5 mt-6">
  <div class="bg-blue-900 rounded p-5">
    <div class="text-3xl mb-3">🖥️</div>
    <h3 class="text-yellow-400 font-bold mb-2">Back-end</h3>
    <p class="text-sm text-gray-300 mb-2"><strong class="text-white">Node.js</strong> (2009) — JS côté serveur grâce au moteur V8</p>
    <ul class="text-xs text-gray-400 space-y-1">
      <li>• Architecture non-bloquante</li>
      <li>• Idéal pour les APIs REST</li>
      <li>• Netflix, LinkedIn, PayPal</li>
    </ul>
  </div>
  <div class="bg-blue-900 rounded p-5">
    <div class="text-3xl mb-3">📱</div>
    <h3 class="text-yellow-400 font-bold mb-2">Mobile</h3>
    <p class="text-sm text-gray-300 mb-2"><strong class="text-white">React Native</strong> — iOS & Android en JS</p>
    <ul class="text-xs text-gray-400 space-y-1">
      <li>• Un seul code pour deux plateformes</li>
      <li>• Performances proches du natif</li>
      <li>• Facebook, Instagram, Shopify</li>
    </ul>
  </div>
  <div class="bg-blue-900 rounded p-5">
    <div class="text-3xl mb-3">💻</div>
    <h3 class="text-yellow-400 font-bold mb-2">Desktop</h3>
    <p class="text-sm text-gray-300 mb-2"><strong class="text-white">Electron</strong> — apps desktop multiplateformes</p>
    <ul class="text-xs text-gray-400 space-y-1">
      <li>• Windows, Mac, Linux</li>
      <li>• VS Code écrit en JS</li>
      <li>• Slack, Discord, Figma</li>
    </ul>
  </div>
</div>

---
layout: default
background: '#1A1A2E'
---

<div class="flex items-center gap-3 mb-1">
  <span class="bg-blue-500 text-white font-bold px-3 py-1 rounded text-xs">PARTIE 2 · [Ndoumbe]</span>
  <span class="text-gray-500 text-sm">Utilisations Aujourd'hui</span>
</div>

# <span class="text-white">L'Écosystème npm</span>

<div class="grid grid-cols-2 gap-8 mt-4">
  <div>
    <h3 class="text-yellow-400 font-bold mb-3">Le plus grand registre du monde</h3>
    <ul class="text-gray-200 space-y-2 text-sm">
      <li>📦 <strong class="text-white">3 millions+</strong> de packages open source</li>
      <li>⬇️ Une commande pour ajouter n'importe quelle fonctionnalité</li>
      <li>🔄 <strong class="text-white">JS fullstack</strong> — un seul langage du front au back</li>
      <li>👥 Communauté massive — solutions pour presque tout</li>
    </ul>
    <h3 class="text-yellow-400 font-bold mt-5 mb-3">Usages inattendus</h3>
    <ul class="text-gray-200 space-y-2 text-sm">
      <li>🔌 <strong class="text-white">IoT</strong> — objets connectés avec Johnny-Five</li>
      <li>🤖 <strong class="text-white">Machine Learning</strong> — TensorFlow.js dans le navigateur</li>
      <li>🛠️ Scripts d'automatisation, outils CLI</li>
    </ul>
  </div>
  <div class="grid grid-cols-2 gap-3 content-start">
    <div class="bg-blue-900 rounded p-4 text-center">
      <div class="text-4xl font-black text-yellow-400">3M+</div>
      <div class="text-xs text-gray-400 mt-1">packages npm</div>
    </div>
    <div class="bg-blue-900 rounded p-4 text-center">
      <div class="text-4xl font-black text-yellow-400">#1</div>
      <div class="text-xs text-gray-400 mt-1">compétence web<br/>la + demandée</div>
    </div>
    <div class="bg-yellow-400 rounded p-4 text-center col-span-2">
      <div class="text-2xl font-black text-gray-900">Fullstack JS</div>
      <div class="text-xs text-gray-700 mt-1">Front · Back · Mobile · Desktop · IoT · IA</div>
    </div>
  </div>
</div>

---
layout: default
background: '#1A1A2E'
---

<div class="flex items-center gap-3 mb-1">
  <span class="bg-green-500 text-white font-bold px-3 py-1 rounded text-xs">PARTIE 3 · [Jérôme]</span>
  <span class="text-gray-500 text-sm">Frameworks & Three.js</span>
</div>

# <span class="text-white">Les Frameworks Majeurs</span>

<div class="grid grid-cols-2 gap-6 mt-4">
  <div>
    <h3 class="text-yellow-400 font-bold mb-3">Pourquoi des frameworks ?</h3>
    <ul class="text-gray-200 space-y-2 text-sm">
      <li>🧱 JS vanilla devient ingérable sur de gros projets</li>
      <li>🏗️ Structure, performance, réutilisabilité des composants</li>
      <li>👥 Collaboration en équipe facilitée</li>
      <li>🚀 Fonctionnalités prêtes à l'emploi</li>
    </ul>
  </div>
  <div class="space-y-2">
    <div class="bg-blue-900 rounded p-3 flex items-center gap-4">
      <span class="text-yellow-400 font-black w-20 text-sm shrink-0">React</span>
      <span class="text-gray-300 text-xs">Meta, 2013 — composants UI, le plus utilisé au monde</span>
    </div>
    <div class="bg-blue-900 rounded p-3 flex items-center gap-4">
      <span class="text-yellow-400 font-black w-20 text-sm shrink-0">Vue</span>
      <span class="text-gray-300 text-xs">2014 — progressif et accessible, idéal pour débuter</span>
    </div>
    <div class="bg-blue-900 rounded p-3 flex items-center gap-4">
      <span class="text-yellow-400 font-black w-20 text-sm shrink-0">Angular</span>
      <span class="text-gray-300 text-xs">Google, 2016 — framework complet, TypeScript natif</span>
    </div>
    <div class="bg-blue-900 rounded p-3 flex items-center gap-4">
      <span class="text-yellow-400 font-black w-20 text-sm shrink-0">Next.js</span>
      <span class="text-gray-300 text-xs">Full-stack, rendu serveur, basé sur React</span>
    </div>
    <div class="bg-blue-900 rounded p-3 flex items-center gap-4">
      <span class="text-yellow-400 font-black w-20 text-sm shrink-0">Svelte</span>
      <span class="text-gray-300 text-xs">Pas de virtual DOM — compilé, ultra-léger</span>
    </div>
  </div>
</div>

---
layout: default
background: '#1A1A2E'
---

<div class="flex items-center gap-3 mb-1">
  <span class="bg-green-500 text-white font-bold px-3 py-1 rounded text-xs">PARTIE 3 · [Jérôme]</span>
  <span class="text-gray-500 text-sm">Frameworks & Three.js</span>
</div>

# <span class="text-white">Three.js — La 3D dans le Navigateur</span>

<div class="grid grid-cols-2 gap-8 mt-4">
  <div>
    <h3 class="text-yellow-400 font-bold mb-3">C'est quoi ?</h3>
    <ul class="text-gray-200 space-y-2 text-sm">
      <li>📅 Créé par <strong class="text-white">Ricardo Cabello (mrdoob)</strong> en 2010</li>
      <li>🔧 Abstraction au-dessus de <strong class="text-white">WebGL</strong> — l'API 3D native des navigateurs</li>
      <li>✨ WebGL seul = des centaines de lignes ; Three.js = quelques dizaines</li>
    </ul>
    <h3 class="text-yellow-400 font-bold mt-4 mb-3">Ce que ça permet</h3>
    <ul class="text-gray-200 space-y-2 text-sm">
      <li>🎮 Scènes 3D interactives dans le navigateur, sans plugin</li>
      <li>💡 Lumières, textures, caméras, physique</li>
      <li>🏢 Utilisé par Nike, Apple, des data viz, des jeux</li>
    </ul>
  </div>
  <div class="space-y-2">
    <h3 class="text-yellow-400 font-bold mb-3">Les concepts clés</h3>
    <div class="bg-blue-900 rounded px-4 py-2 flex items-center gap-3">
      <code class="text-yellow-400 text-sm w-24 shrink-0">Scene</code>
      <span class="text-gray-300 text-xs">Le monde 3D — contient tous les objets</span>
    </div>
    <div class="bg-blue-900 rounded px-4 py-2 flex items-center gap-3">
      <code class="text-yellow-400 text-sm w-24 shrink-0">Camera</code>
      <span class="text-gray-300 text-xs">Le point de vue — perspective ou orthographique</span>
    </div>
    <div class="bg-blue-900 rounded px-4 py-2 flex items-center gap-3">
      <code class="text-yellow-400 text-sm w-24 shrink-0">Geometry</code>
      <span class="text-gray-300 text-xs">La forme — cube, sphère, cylindre…</span>
    </div>
    <div class="bg-blue-900 rounded px-4 py-2 flex items-center gap-3">
      <code class="text-yellow-400 text-sm w-24 shrink-0">Material</code>
      <span class="text-gray-300 text-xs">L'apparence — couleur, texture, brillance</span>
    </div>
    <div class="bg-blue-900 rounded px-4 py-2 flex items-center gap-3">
      <code class="text-yellow-400 text-sm w-24 shrink-0">Renderer</code>
      <span class="text-gray-300 text-xs">Dessine la scène via WebGL à chaque frame</span>
    </div>
    <div class="bg-blue-900 rounded px-4 py-2 flex items-center gap-3">
      <code class="text-yellow-400 text-sm w-24 shrink-0">animate()</code>
      <span class="text-gray-300 text-xs">Boucle 60fps — requestAnimationFrame</span>
    </div>
  </div>
</div>

---
layout: default
background: '#1A1A2E'
---

<div class="flex items-center gap-3 mb-1">
  <span class="bg-green-500 text-white font-bold px-3 py-1 rounded text-xs">PARTIE 3 · [Jérôme]</span>
  <span class="text-gray-500 text-sm">Démo Live</span>
</div>

# <span class="text-white">Le Cube — Démo Live</span>

<div class="grid grid-cols-2 gap-8 mt-4">
  <div>
    <h3 class="text-yellow-400 font-bold mb-3">Ce que vous allez voir</h3>
    <ul class="text-gray-200 space-y-2 text-sm">
      <li>🎲 Un cube 3D qui flotte et tourne en temps réel</li>
      <li>💻 Codé en JavaScript pur avec Three.js</li>
      <li>🌐 Rendu directement dans le navigateur — aucun plugin</li>
    </ul>

```js
const scene = new THREE.Scene();
const camera = new THREE.PerspectiveCamera(75, w/h);
const geometry = new THREE.BoxGeometry();
const material = new THREE.MeshStandardMaterial();
const cube = new THREE.Mesh(geometry, material);
scene.add(cube);

function animate() {
  cube.rotation.x += 0.01;
  cube.rotation.y += 0.01;
  renderer.render(scene, camera);
}
animate();
```
  </div>
 <div class="bg-blue-900 rounded" style="height: 300px;">
   <ClientOnly>
     <ThreeCube />
   </ClientOnly>
</div>
</div>

---
layout: default
background: '#1A1A2E'
---

<div class="flex flex-col items-center justify-center h-full gap-6 text-center">
  <div class="bg-yellow-400 w-24 h-24 flex items-center justify-center rounded-sm shadow-xl">
    <span class="text-4xl font-black text-gray-900">JS</span>
  </div>
  <h1 class="text-5xl font-black text-white">Merci !</h1>
  <p class="text-yellow-400 text-xl italic">Des questions ?</p>
  <div class="h-px w-60 bg-gray-600 mt-2"></div>
  <div class="flex gap-10 text-sm text-gray-400 mt-2">
    <div class="text-center">
      <div class="text-white font-bold">[Dawid]</div>
      <div class="text-xs">Histoire & Création</div>
    </div>
    <div class="text-center">
      <div class="text-white font-bold">[Ndoumbe]</div>
      <div class="text-xs">Utilisations</div>
    </div>
    <div class="text-center">
      <div class="text-white font-bold">[Jérôme]</div>
      <div class="text-xs">Frameworks & Three.js</div>
    </div>
  </div>
</div>