<img src="https://capsule-render.vercel.app/api?type=waving&height=180&color=0:F48FB8,100:D63F7A&text=Hi,%20I'm%20Neelab%20🌸&fontColor=FFFFFF&fontSize=46&fontAlignY=38&desc=systems%20•%20performance%20•%20full-stack&descAlignY=60&descSize=16" width="100%" alt="Hi, I'm Neelab" />

<div align="center">

🎀 **Computer Science @ University of Waterloo** · Previously at **Microsoft** 🎀

I like systems and performance work: laying data out the way the hardware wants it,<br>
and then measuring whether it actually got faster. I also build full-stack web apps ✨

📍 Waterloo, ON

</div>

<br>

## 💗 Featured projects

<table>
<tr>
<td width="100%">

### 🐉 [SIMD & Sorcery](https://github.com/NeelabK/simd-and-sorcery)

**A turn-based dungeon crawler played by D&D 5e rules, running on a hand-vectorized map engine.**

![C++17](https://img.shields.io/badge/C++17-E0457B?style=flat-square&logo=cplusplus&logoColor=white)
![AVX-512](https://img.shields.io/badge/AVX--512-E0457B?style=flat-square&logo=intel&logoColor=white)
![ARM NEON](https://img.shields.io/badge/ARM_NEON-E0457B?style=flat-square&logo=arm&logoColor=white)
![Make](https://img.shields.io/badge/Make-E0457B?style=flat-square&logo=gnu&logoColor=white)

- 🌸 Map stored as structure-of-arrays byte grids, each row padded to **128 bytes** (two 512-bit registers) with a zero border, so every neighbour is a fixed memory offset and there are no bounds checks
- 🌸 Whole-map work (enemy movement, spawning, rendering) runs as **AVX-512** and **NEON** kernels with a scalar reference, chosen **at runtime** from CPU feature detection, with no special build flags
- 🌸 **16.9x** faster enemy-move computation and **23.6x** faster glyph classification on an Apple M2 (`--bench`)
- 🌸 `--selftest` checks every SIMD backend against the scalar version **byte for byte** on 500 random maps
- 🌸 Full 5e rules on top: d20 vs AC, crits, advantage/disadvantage, saving throws, four classes with spells, monster stat blocks, XP and levelling

</td>
</tr>
<tr>
<td width="100%">

### 🎙️ [Holo Agents](https://github.com/NeelabK/holo-agents)

**A web app for real-time voice conversations with AI hologram characters.**

![JavaScript](https://img.shields.io/badge/JavaScript-F06BA8?style=flat-square&logo=javascript&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-F06BA8?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-F06BA8?style=flat-square&logo=express&logoColor=white)
![Solana](https://img.shields.io/badge/Solana-F06BA8?style=flat-square&logo=solana&logoColor=white)
![Webpack](https://img.shields.io/badge/Webpack-F06BA8?style=flat-square&logo=webpack&logoColor=white)

- 🌸 Carousel of 25+ hologram characters, each with its own persona, talking back by voice in real time through the **Ultravox** voice-AI API
- 🌸 Personas live in a YAML file, so adding or changing a character is a text edit, not a code change
- 🌸 **Solana** wallet check (web3.js + Helius RPC) gates access to token holders
- 🌸 Express backend, Webpack + Babel front-end build

</td>
</tr>
<tr>
<td width="100%">

### 🧱 [Biquadris](https://github.com/NeelabK/Biquadris-CS246-Project)

**A two-player, Tetris-style battle game in C++ with text and graphical interfaces.**

![C++](https://img.shields.io/badge/C++-C2185B?style=flat-square&logo=cplusplus&logoColor=white)
![X11](https://img.shields.io/badge/X11-C2185B?style=flat-square&logo=xdotorg&logoColor=white)
![Make](https://img.shields.io/badge/Make-C2185B?style=flat-square&logo=gnu&logoColor=white)

- 🌸 Object-oriented design with game logic separated from presentation, so the console and X11 graphical views share one engine
- 🌸 Multiple difficulty levels, special effects players trigger against each other, and persistent high scores
- 🌸 Team project; the repo includes the UML architecture diagram

</td>
</tr>
<tr>
<td width="100%">

### 👛 [Y2K Dress Up Game](https://github.com/NeelabK/y2k-dress-up-game)

**A 2000s Flash-style fashion dress-up game that runs in the browser. [Play it here](https://neelabk.github.io/y2k-dress-up-game/).**

![JavaScript](https://img.shields.io/badge/JavaScript-F06BA8?style=flat-square&logo=javascript&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-F06BA8?style=flat-square&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-F06BA8?style=flat-square&logo=css&logoColor=white)
![Python](https://img.shields.io/badge/Python-F06BA8?style=flat-square&logo=python&logoColor=white)

<a href="https://neelabk.github.io/y2k-dress-up-game/"><img src="https://raw.githubusercontent.com/NeelabK/y2k-dress-up-game/main/screenshots/mall.png" width="640" alt="Screenshot of the dress-up game at the mall" /></a>

- 🌸 Paper-doll layering: every item is a transparent PNG drawn in place on one shared canvas, stacked in a fixed order (shoes, bottoms, tops, coat, bag, shades)
- 🌸 Clothes are actually worn, not pasted on: the doll's base layer is redrawn under each item, and the coat has a back panel plus a mask so tops tuck inside it
- 🌸 24 items across four closets, three places to visit, a random-outfit button and a Y2K soundtrack
- 🌸 One HTML file with no framework or build step, hosted on **GitHub Pages**; the art was fitted to the doll with a Python image pipeline (Pillow, NumPy, SciPy)

</td>
</tr>
<tr>
<td width="100%">

### 🎧 [Pink Mini Player](https://github.com/NeelabK/retro-pink-music-player)

**A retro pink click-wheel music player for your phone that plays your own MP3s. [Try it here](https://neelabk.github.io/retro-pink-music-player/).**

![JavaScript](https://img.shields.io/badge/JavaScript-F06BA8?style=flat-square&logo=javascript&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-F06BA8?style=flat-square&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-F06BA8?style=flat-square&logo=css&logoColor=white)
![PWA](https://img.shields.io/badge/PWA-F06BA8?style=flat-square&logo=pwa&logoColor=white)

<a href="https://neelabk.github.io/retro-pink-music-player/"><img src="https://raw.githubusercontent.com/NeelabK/retro-pink-music-player/main/screenshots/menu.jpg" width="200" alt="Main menu of the pink music player" /> <img src="https://raw.githubusercontent.com/NeelabK/retro-pink-music-player/main/screenshots/songs.jpg" width="200" alt="Song list with two songs numbered in the queue" /> <img src="https://raw.githubusercontent.com/NeelabK/retro-pink-music-player/main/screenshots/now-playing.jpg" width="200" alt="Now Playing screen with a progress bar" /></a>

- 🌸 Working click wheel: dragging a finger around it is converted from angle change into scroll steps, and the screen also takes swipes and taps
- 🌸 Songs you add are stored on the device in **IndexedDB**, with titles and artists read by a hand-written **ID3v2** tag parser
- 🌸 Play queue (press and hold a song), shuffle, repeat, and lock-screen controls through the **Media Session API**
- 🌸 Installs to the home screen and works offline: a service worker answers Safari's byte-range audio requests from its cache
- 🌸 One HTML file with no framework or build step, hosted on **GitHub Pages**

</td>
</tr>
</table>

<br>

## 🎀 Tech stack

**Languages**<br>
![C++](https://img.shields.io/badge/C++-FF5FA2?style=for-the-badge&logo=cplusplus&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-FF5FA2?style=for-the-badge&logo=javascript&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-FF5FA2?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-FF5FA2?style=for-the-badge&logo=css&logoColor=white)

**Systems & performance**<br>
![AVX-512](https://img.shields.io/badge/AVX--512-E0457B?style=for-the-badge&logo=intel&logoColor=white)
![ARM NEON](https://img.shields.io/badge/ARM_NEON-E0457B?style=for-the-badge&logo=arm&logoColor=white)
![Make](https://img.shields.io/badge/Make-E0457B?style=for-the-badge&logo=gnu&logoColor=white)
![X11](https://img.shields.io/badge/X11-E0457B?style=for-the-badge&logo=xdotorg&logoColor=white)

**Web & backend**<br>
![Node.js](https://img.shields.io/badge/Node.js-C2185B?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-C2185B?style=for-the-badge&logo=express&logoColor=white)
![Webpack](https://img.shields.io/badge/Webpack-C2185B?style=for-the-badge&logo=webpack&logoColor=white)
![Babel](https://img.shields.io/badge/Babel-C2185B?style=for-the-badge&logo=babel&logoColor=white)
![Solana](https://img.shields.io/badge/Solana-C2185B?style=for-the-badge&logo=solana&logoColor=white)

**Tools**<br>
![Git](https://img.shields.io/badge/Git-F06BA8?style=for-the-badge&logo=git&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-F06BA8?style=for-the-badge&logo=linux&logoColor=white)
![macOS](https://img.shields.io/badge/macOS-F06BA8?style=for-the-badge&logo=apple&logoColor=white)

<br>

<div align="center">

💌 Reach me through GitHub, or open an issue on any of my repos.

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&height=100&section=footer&color=0:D63F7A,100:F48FB8" width="100%" alt="" />
