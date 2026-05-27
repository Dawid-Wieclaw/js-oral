# JavaScript — Histoire, Usages & Frameworks

---

## Slide 1 — La Naissance (1995)

**Contexte**
- 1995 : le web est statique, Netscape Navigator domine
- Besoin d'un langage simple pour animer les pages sans rechargement
- Brendan Eich recruté chez Netscape avec une mission claire

**La création**
- Prototype développé en **10 jours** seulement
- Nom initial : **Mocha** → LiveScript → **JavaScript**
- Inspiré de Java (syntaxe), Scheme (fonctions), Self (prototypes)

---

## Slide 2 — Standardisation & Évolution

**La guerre des navigateurs**
- Microsoft copie JS sous le nom **JScript** pour IE → incompatibilités majeures
- 1997 : Ecma International publie la norme **ECMAScript**

**Les grandes versions**
| Version | Année | Apport clé |
|---|---|---|
| ES3 | 1999 | Base stable, regex |
| ES5 | 2009 | strict mode, JSON |
| ES6 | 2015 | classes, arrow fn, promesses |
| ES2017+ | annuel | async/await, modules |

---

## Slide 3 — Caractéristiques & Chiffres

**Ce qui rend JS unique**
- Langage **interprété** (JIT via V8, SpiderMonkey)
- **Mono-thread** + event loop → asynchrone non-bloquant
- Typage **dynamique et faible** — flexible mais piégeux
- Fonctions comme citoyens de première classe

**JS en chiffres**
- 🏆 Langage **#1** sur StackOverflow 12 années de suite
- **98%** des sites web l'utilisent côté client
- **3M+** packages sur npm
- De Netscape 1995 à serveurs, mobiles et IoT aujourd'hui

---

## Slide 4 — Le Web Front-End

**Le rôle fondamental**
- JS est le seul langage natif des navigateurs — pas d'alternative
- Manipulation du **DOM** : modifier le HTML/CSS en temps réel
- Gestion des événements : clics, formulaires, animations

**Ce que ça permet concrètement**
- Validation de formulaires côté client
- Chargement sans rechargement de page (**AJAX**)
- Interfaces riches : drag & drop, modales, notifications
- Exemples : Google Maps, Gmail, Twitter/X

---

## Slide 5 — Au-delà du Navigateur

**Back-end avec Node.js (2009)**
- JS côté serveur grâce au moteur V8 de Chrome
- Architecture **non-bloquante** — idéal pour les APIs et le temps réel
- Utilisé par Netflix, LinkedIn, PayPal

**Mobile & Desktop**
- **React Native** — applications iOS et Android en JS
- **Electron** — apps desktop : VS Code, Slack, Discord sont en JS

---

## Slide 6 — L'Écosystème npm

**Le plus grand registre de packages au monde**
- 3 millions+ de packages open source disponibles
- Un seul langage du front au back — **JavaScript fullstack**
- Recrutement facilité : compétence web la plus demandée

**Usages inattendus**
- Objets connectés (**IoT**) avec Johnny-Five
- Machine learning avec **TensorFlow.js**
- Scripts d'automatisation, outils CLI

---

## Slide 7 — L'Écosystème des Frameworks

**Pourquoi des frameworks ?**
- JS vanilla devient vite complexe sur de gros projets
- Les frameworks apportent structure, performance, réutilisabilité

**Les grands noms**
- **React** (Meta, 2013) — composants UI, le plus utilisé au monde
- **Vue** (2014) — plus accessible, progressif
- **Angular** (Google, 2016) — framework complet, TypeScript natif
- **Next.js / Nuxt** — full-stack, rendu serveur

---

## Slide 8 — Three.js, la 3D dans le Navigateur

**C'est quoi ?**
- Librairie créée par **Ricardo Cabello (mrdoob)** en 2010
- Abstraction au-dessus de **WebGL** — l'API 3D native des navigateurs
- WebGL seul = très complexe ; Three.js = accessible en quelques lignes

**Ce que ça permet**
- Scènes 3D interactives directement dans le navigateur, sans plugin
- Animations, lumières, textures, caméras
- Utilisé par Nike, Apple, des jeux, des data viz 3D

---

## Slide 9 — Démo Live : Le Cube

**~20 lignes de code pour une scène 3D complète**

- `Scene` — le monde 3D
- `Camera` — le point de vue
- `Mesh` = `Geometry` + `Material`
- `Renderer` — dessine via WebGL
- `animate()` — boucle 60fps pour faire tourner le cube

> 💡 Démonstration en direct dans le navigateur
