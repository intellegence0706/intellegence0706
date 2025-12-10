<!-- README.md: Space-themed animated developer profile (Full-Stack, AI, Blockchain) -->
<!-- Replace YOUR_GITHUB and YOUR_REPO if you host assets in the same repo -->
<h1 align="center">
  <img alt="nebula banner" src="./assets/banner/nebula.gif" width="100%" style="border-radius:12px;box-shadow:0 8px 30px rgba(0,0,0,0.45)"/>
</h1>

<p align="center">
  <img src="./assets/nebula/space-glow.gif" alt="space-glow" width="24" style="vertical-align:middle"/> 
  <strong style="font-size:1.6em;color:#9be7ff;text-shadow:0 0 12px rgba(155,231,255,0.6)">A+1 • Full-Stack • AI • Blockchain</strong>
</p>

<div align="center" style="margin: 18px 0;">
  <!-- Orbiting icons row -->
  <img src="./assets/icons/react.svg" alt="React" width="92" style="margin:6px"/>
  <img src="./assets/icons/node.svg" alt="Node" width="92" style="margin:6px"/>
  <img src="./assets/icons/python.svg" alt="Python" width="92" style="margin:6px"/>
  <img src="./assets/icons/solidity.svg" alt="Solidity" width="92" style="margin:6px"/>
  <img src="./assets/icons/docker.svg" alt="Docker" width="92" style="margin:6px"/>
  <img src="./assets/icons/aws.svg" alt="AWS" width="92" style="margin:6px"/>
</div>

---

## ✨ About — cosmic edition
> Building scalable full-stack apps with intelligence.  
> AI-first, blockchain-ready, design-minded.

---

## 🛰 Features
- Animated **space nebula** banner (GIF)  
- **SVG animated** tech icons (non-GIF; small, crisp vectors)  
- Clean layout that works on **GitHub mobile + desktop**  
- Click-to-copy code blocks for every code snippet (GitHub built-in)  
- Minimal external hosting — keep assets inside the repo (`/assets/...`)

---

## 🛠 Tech Stack (animated SVG icons)
Below are the animated SVGs used above — they are **vector** and **animated** (orbiting elements, glow).  
Copy each SVG block (click the copy button) into the corresponding file path:

### `./assets/icons/react.svg`
\```svg
<!-- React-style animated orb (placeholder, abstracted icon) -->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 120 120" width="120" height="120">
  <defs>
    <linearGradient id="g" x1="0" x2="1">
      <stop offset="0%" stop-color="#61dafb"/>
      <stop offset="100%" stop-color="#7fffd4"/>
    </linearGradient>
    <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="3.5" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <!-- central core -->
  <circle cx="60" cy="60" r="20" fill="url(#g)" filter="url(#glow)"/>

  <!-- three orbit paths -->
  <g fill="none" stroke="rgba(155,231,255,0.35)" stroke-width="2">
    <ellipse cx="60" cy="60" rx="36" ry="14" transform="rotate(0 60 60)"/>
    <ellipse cx="60" cy="60" rx="36" ry="14" transform="rotate(60 60 60)"/>
    <ellipse cx="60" cy="60" rx="36" ry="14" transform="rotate(120 60 60)"/>
  </g>

  <!-- three orbiting dots (animated with SMIL) -->
  <g fill="#fff">
    <circle r="4" fill="#61dafb">
      <animateMotion dur="6s" repeatCount="indefinite" keyPoints="0;1" keyTimes="0;1">
        <mpath xlink:href="#path0"/>
      </animateMotion>
    </circle>
  </g>

  <!-- invisible path definitions for animateMotion -->
  <path id="path0" d="M96 60 A36 14 0 1 0 24 60 A36 14 0 1 0 96 60" fill="none" stroke="none"/>
</svg>
\```

### `./assets/icons/node.svg`
\```svg
<!-- Node-style animated orb (abstract node icon) -->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 120 120" width="120" height="120">
  <defs>
    <linearGradient id="ng" x1="0" x2="1">
      <stop offset="0%" stop-color="#8cc84b"/>
      <stop offset="100%" stop-color="#a8f78b"/>
    </linearGradient>
    <filter id="g2"><feGaussianBlur stdDeviation="3" result="b"/><feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge></filter>
  </defs>

  <polygon points="60,20 92,40 92,80 60,100 28,80 28,40" fill="url(#ng)" filter="url(#g2)" />
  <circle cx="60" cy="60" r="8" fill="#fff"/>
  <g>
    <circle cx="60" cy="60" r="3" fill="#2b2b2b">
      <animate attributeName="r" values="3;6;3" dur="2s" repeatCount="indefinite"/>
    </circle>
  </g>
</svg>
\```

### `./assets/icons/python.svg`
\```svg
<!-- Python-style abstracted animated icon -->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 120 120" width="120" height="120">
  <defs>
    <linearGradient id="pg" x1="0" x2="1"><stop stop-color="#3776ab" offset="0"/><stop stop-color="#ffd43b" offset="1"/></linearGradient>
  </defs>
  <rect x="12" y="18" rx="10" ry="10" width="96" height="84" fill="url(#pg)" />
  <circle cx="36" cy="36" r="6" fill="#fff">
    <animate attributeName="cy" dur="3s" values="36;48;36" repeatCount="indefinite"/>
  </circle>
  <circle cx="84" cy="84" r="6" fill="#000">
    <animate attributeName="cx" dur="4s" values="84;72;84" repeatCount="indefinite"/>
  </circle>
</svg>
\```

### `./assets/icons/solidity.svg`
\```svg
<!-- Solidity abstract token icon with glow -->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 120 120" width="120" height="120">
  <defs>
    <linearGradient id="sg"><stop offset="0" stop-color="#8a2be2"/><stop offset="1" stop-color="#4b0082"/></linearGradient>
  </defs>
  <path d="M60 18 L94 60 L60 102 L26 60 Z" fill="url(#sg)" stroke="#fff" stroke-opacity="0.12"/>
  <circle cx="60" cy="60" r="10" fill="#fff" opacity="0.9">
    <animate attributeName="r" dur="2.5s" values="8;12;8" repeatCount="indefinite"/>
  </circle>
</svg>
\```

### `./assets/icons/docker.svg`
\```svg
<!-- Docker abstract container with animated waves -->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 120 120" width="120" height="120">
  <defs>
    <linearGradient id="dg"><stop stop-color="#2496ed"/><stop stop-color="#00b4ff"/></linearGradient>
  </defs>
  <rect x="16" y="36" width="88" height="48" rx="6" fill="url(#dg)"/>
  <g fill="#fff" opacity="0.85">
    <rect x="26" y="28" width="14" height="12" rx="2"/>
    <rect x="44" y="28" width="14" height="12" rx="2"/>
    <rect x="62" y="28" width="14" height="12" rx="2"/>
    <rect x="80" y="28" width="14" height="12" rx="2"/>
  </g>
  <path d="M18 76 Q60 88 102 76" fill="none" stroke="#fff" stroke-width="2" stroke-opacity="0.6">
    <animate attributeName="d" dur="4s" repeatCount="indefinite"
      values="M18 76 Q60 88 102 76; M18 76 Q60 84 102 76; M18 76 Q60 88 102 76"/>
  </path>
</svg>
\```

### `./assets/icons/aws.svg`
\```svg
<!-- AWS abstract cloud with glow -->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 120 120" width="120" height="120">
  <defs>
    <linearGradient id="ag"><stop stop-color="#ff9900"/><stop stop-color="#ffcc66"/></linearGradient>
  </defs>
  <ellipse cx="60" cy="66" rx="38" ry="18" fill="url(#ag)" opacity="0.95"/>
  <g fill="#fff">
    <circle cx="44" cy="60" r="3">
      <animate attributeName="cy" values="60;66;60" dur="2.6s" repeatCount="indefinite"/>
    </circle>
    <circle cx="76" cy="60" r="3">
      <animate attributeName="cy" values="60;54;60" dur="2.6s" repeatCount="indefinite"/>
    </circle>
  </g>
</svg>
\```

---

## 🎛 Example usage — "icons orbiting your name"
Copy this HTML block into `README.md` (it will render on GitHub):

\```html
<div align="center" style="padding:18px;">
  <h2 style="color:#bfe9ff;text-shadow:0 0 14px rgba(191,233,255,0.45)">⭐ A+1 — Full-Stack • AI • Blockchain</h2>
  <div style="display:flex;gap:18px;justify-content:center;align-items:center;margin-top:12px;">
    <img src="./assets/icons/react.svg" width="76" alt="React"/>
    <img src="./assets/icons/node.svg" width="76" alt="Node"/>
    <img src="./assets/icons/python.svg" width="76" alt="Python"/>
    <img src="./assets/icons/solidity.svg" width="76" alt="Solidity"/>
    <img src="./assets/icons/docker.svg" width="76" alt="Docker"/>
    <img src="./assets/icons/aws.svg" width="76" alt="AWS"/>
  </div>
</div>
\```

---

## 📎 Click-to-copy tip
All fenced code blocks in this README are copyable with GitHub's built-in copy button.  
If you want runnable examples (like `package.json` or `docker-compose.yml`), paste them into fenced blocks — users can copy them with one click.

---

## ⚠️ Notes & troubleshooting
- **If icons or animated SVGs do not show**: make sure the file paths match case-sensitively (`assets/icons/react.svg`).  
- **If GIF banner does not animate**: upload `nebula.gif` to `./assets/banner/nebula.gif` and reference that path.  
- GitHub **sanitizes** SVGs — these SVGs avoid embedded scripts and use SMIL/CSS-style animations, which usually render safely. If an environment blocks SVG animation, fallback to a small animated GIF.

---

## 📬 Contact
If you want, tell me:
- Your GitHub username (I will inject the correct `raw.githubusercontent` links)
- Or upload your nebula GIF and I will adapt the README to exact URLs

---

*Enjoy your space-themed, animated GitHub profile!*
