# Vikas — Build. Learn. Ship. ⚡

<div align="center">
  <svg width="100%" height="320" viewBox="0 0 1200 450" xmlns="http://www.w3.org/2000/svg">
    <defs>
      <linearGradient id="bgGradient" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" stop-color="#0a0a0f">
          <animate attributeName="stop-color" values="#0a0a0f;#1a0b2e;#2d1b69;#0a0a0f" dur="10s" repeatCount="indefinite"/>
        </stop>
        <stop offset="50%" stop-color="#0f0a1a">
          <animate attributeName="stop-color" values="#0f0a1a;#2e1065;#1a0b2e;#0f0a1a" dur="12s" repeatCount="indefinite"/>
        </stop>
        <stop offset="100%" stop-color="#1a0f2e">
          <animate attributeName="stop-color" values="#1a0f2e;#0b1426;#2e1a65;#1a0f2e" dur="8s" repeatCount="indefinite"/>
        </stop>
      </linearGradient>

      <linearGradient id="neonPink" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stop-color="#ff0080"/>
        <stop offset="50%" stop-color="#ff4081"/>
        <stop offset="100%" stop-color="#e91e63"/>
      </linearGradient>

      <linearGradient id="neonCyan" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stop-color="#00ffff"/>
        <stop offset="50%" stop-color="#40e0d0"/>
        <stop offset="100%" stop-color="#0ff"/>
      </linearGradient>

      <linearGradient id="neonPurple" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stop-color="#8a2be2"/>
        <stop offset="50%" stop-color="#9d4edd"/>
        <stop offset="100%" stop-color="#a663cc"/>
      </linearGradient>

      <linearGradient id="neonGreen" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stop-color="#39ff14"/>
        <stop offset="50%" stop-color="#32cd32"/>
        <stop offset="100%" stop-color="#00ff41"/>
      </linearGradient>

      <linearGradient id="waveGradient" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stop-color="#ff0080">
          <animate attributeName="stop-color" values="#ff0080;#00ffff;#39ff14;#8a2be2;#ff0080" dur="4s" repeatCount="indefinite"/>
        </stop>
        <stop offset="33%" stop-color="#00ffff">
          <animate attributeName="stop-color" values="#00ffff;#39ff14;#8a2be2;#ff0080;#00ffff" dur="4s" repeatCount="indefinite"/>
        </stop>
        <stop offset="66%" stop-color="#39ff14">
          <animate attributeName="stop-color" values="#39ff14;#8a2be2;#ff0080;#00ffff;#39ff14" dur="4s" repeatCount="indefinite"/>
        </stop>
        <stop offset="100%" stop-color="#8a2be2">
          <animate attributeName="stop-color" values="#8a2be2;#ff0080;#00ffff;#39ff14;#8a2be2" dur="4s" repeatCount="indefinite"/>
        </stop>
      </linearGradient>

      <filter id="neonGlow" x="-50%" y="-50%" width="200%" height="200%">
        <feGaussianBlur stdDeviation="4" result="coloredBlur"/>
        <feMerge> 
          <feMergeNode in="coloredBlur"/>
          <feMergeNode in="SourceGraphic"/>
        </feMerge>
      </filter>

      <filter id="cyanGlow" x="-50%" y="-50%" width="200%" height="200%">
        <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
        <feMerge> 
          <feMergeNode in="coloredBlur"/>
          <feMergeNode in="SourceGraphic"/>
        </feMerge>
      </filter>

      <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
        <path d="M 40 0 L 0 0 0 40" fill="none" stroke="rgba(0,255,255,0.1)" stroke-width="1">
          <animate attributeName="stroke" values="rgba(0,255,255,0.1);rgba(255,0,128,0.1);rgba(57,255,20,0.1);rgba(138,43,226,0.1);rgba(0,255,255,0.1)" dur="8s" repeatCount="indefinite"/>
        </path>
      </pattern>

      <style>
        .title-main { 
          font: 800 64px 'Courier New', monospace; 
          fill: url(#neonCyan); 
          filter: url(#cyanGlow);
        }
        .title-accent { 
          font: 800 64px 'Courier New', monospace; 
          fill: url(#neonPink); 
          filter: url(#neonGlow);
        }
        .subtitle { 
          font: 600 20px 'Courier New', monospace; 
          fill: #ffffff;
          opacity: 0.9;
        }
        .chip {
          transition: transform 0.4s ease;
          cursor: pointer;
        }
        .chip:hover {
          transform: translateY(-4px) scale(1.05);
        }
        .particle {
          animation: float 6s ease-in-out infinite;
        }
        .pulse {
          animation: pulse 4s ease-in-out infinite;
        }
        @keyframes float {
          0%, 100% { transform: translateY(0); opacity: 0.6; }
          50% { transform: translateY(-20px); opacity: 1; }
        }
        @keyframes pulse {
          0%, 100% { opacity: 0.6; }
          50% { opacity: 1; }
        }
      </style>
    </defs>

    <rect width="1200" height="450" fill="url(#bgGradient)" rx="25"/>
    <rect width="1200" height="450" fill="url(#grid)" rx="25" opacity="0.3"/>

    <g transform="translate(200, 150)">
      <circle class="particle" cx="0" cy="0" r="3" fill="url(#neonPink)" filter="url(#neonGlow)"/>
    </g>
    <g transform="translate(400, 200)">
      <circle class="particle" cx="0" cy="0" r="2" fill="url(#neonCyan)" filter="url(#cyanGlow)"/>
    </g>
    <g transform="translate(800, 120)">
      <circle class="particle" cx="0" cy="0" r="2.5" fill="url(#neonGreen)" filter="url(#cyanGlow)"/>
    </g>

    <circle class="particle" cx="150" cy="300" r="4" fill="url(#neonCyan)" filter="url(#cyanGlow)"/>
    <circle class="particle" cx="350" cy="350" r="3" fill="url(#neonPink)" filter="url(#neonGlow)"/>
    <circle class="particle" cx="600" cy="320" r="2" fill="url(#neonGreen)" filter="url(#cyanGlow)"/>

    <text x="80" y="140" class="title-main">VI</text>
    <text x="220" y="140" class="title-accent">KAS</text>

    <text x="80" y="180" class="subtitle">
      Build. Learn. Ship. — Backend • Security • Android
      <animate attributeName="opacity" values="0.7;1;0.7" dur="3s" repeatCount="indefinite"/>
    </text>

    <path stroke="url(#waveGradient)" stroke-width="3" fill="none" opacity="0.8" filter="url(#cyanGlow)">
      <animate attributeName="d" values="M50,320 Q300,300 600,315 T1150,305;M50,340 Q300,320 600,335 T1150,325;M50,320 Q300,300 600,315 T1150,305" dur="6s" repeatCount="indefinite"/>
    </path>

    <g transform="translate(80, 220)">
      <g class="chip">
        <rect width="200" height="40" rx="20" fill="rgba(10,10,15,0.7)" stroke="url(#neonCyan)" stroke-width="2"/>
        <text x="100" y="25" fill="url(#neonCyan)" text-anchor="middle" font-size="14" font-family="Courier New">Learning in public</text>
      </g>
      <g class="chip" transform="translate(220, 0)">
        <rect width="220" height="40" rx="20" fill="rgba(10,10,15,0.7)" stroke="url(#neonGreen)" stroke-width="2"/>
        <text x="110" y="25" fill="url(#neonGreen)" text-anchor="middle" font-size="14" font-family="Courier New">Backend + Security</text>
      </g>
      <g class="chip" transform="translate(460, 0)">
        <rect width="260" height="40" rx="20" fill="rgba(10,10,15,0.7)" stroke="url(#neonPurple)" stroke-width="2"/>
        <text x="130" y="25" fill="url(#neonPurple)" text-anchor="middle" font-size="14" font-family="Courier New">Android + AI (exploring)</text>
      </g>
    </g>

    <polygon points="1150,50 1180,50 1180,80" fill="url(#neonPink)" filter="url(#neonGlow)" class="pulse"/>
    <polygon points="20,400 50,400 50,430" fill="url(#neonCyan)" filter="url(#cyanGlow)" class="pulse"/>
    
    <rect x="30" y="420" width="1140" height="3" fill="url(#waveGradient)" rx="1.5" filter="url(#cyanGlow)">
      <animate attributeName="opacity" values="0.8;1;0.8" dur="2s" repeatCount="indefinite"/>
    </rect>
  </svg>
</div>

<p align="center">
  <a href="https://vikaslavaniya.pages.dev/">
    <img src="https://img.shields.io/badge/🌐_Portfolio-Visit_Now-111827?style=for-the-badge&logoColor=00FFFF&labelColor=0B0F19" alt="Portfolio" />
  </a>
  <a href="https://syntaxerror.pages.dev/">
    <img src="https://img.shields.io/badge/🎨_Studio-SyntaxError-0F172A?style=for-the-badge&logoColor=FF0080&labelColor=0B0F19" alt="Studio" />
  </a>
  <a href="https://www.linkedin.com/in/vikas-lavaniya-9b0771292">
    <img src="https://img.shields.io/badge/💼_LinkedIn-Connect-0A66C2?style=for-the-badge&logoColor=FFFFFF&labelColor=0B0F19" alt="LinkedIn" />
  </a>
</p>

<div align="center">

![Profile Views](https://komarev.com/ghpvc/?username=vikas7516&color=blueviolet&style=flat-square&label=Profile+Views)
![GitHub followers](https://img.shields.io/github/followers/vikas7516?style=social)
[![Typing SVG](https://readme-typing-svg.herokuapp.com/?lines=Backend+Developer;Security+Enthusiast;Android+Explorer;AI+Experimenter&font=Fira%20Code&center=true&width=380&height=50&color=00FFFF)](https://git.io/typing-svg)

</div>

---

## 🎮 Activity Matrix

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=vikas7516&show_icons=true&theme=synthwave&hide_border=true&bg_color=0D1117&title_color=FF0080&icon_color=00FFFF&text_color=FFFFFF" height="190"/>
<img src="https://github-readme-streak-stats.herokuapp.com?user=vikas7516&theme=neon-dark&hide_border=true&background=0D1117&stroke=00FFFF&ring=FF0080&fire=39FF14&currStreakLabel=00FFFF" height="190"/>

</div>

<div align="center">

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=vikas7516&layout=compact&theme=synthwave&hide_border=true&bg_color=0D1117&title_color=FF0080&text_color=FFFFFF" height="190"/>

</div>

---

## ⚡ System Status

| 🔥 Current Mission | 🎯 Active Quests |
|---------------------|-------------------|
| **Backend Development**: Node.js, Flask, REST APIs | ☐ Complete Google IT Support certification |
| **System Administration**: Linux, networking fundamentals | ☐ Build 3 production-ready REST APIs |
| **Cybersecurity**: TryHackMe labs, Wireshark analysis | ☐ Publish TryHackMe writeups |
| **Mobile Development**: Kotlin basics, Flutter exploration | ☐ Launch first Android app prototype |
| **AI Integration**: OpenAI API, automation workflows | ☐ Contribute to open source projects |

---

## 💻 Tech Stack Matrix

<div align="center">

**Languages**

<img src="https://img.shields.io/badge/JavaScript-23272A?style=for-the-badge&logo=javascript&logoColor=F7DF1E" />
<img src="https://img.shields.io/badge/Python-23272A?style=for-the-badge&logo=python&logoColor=3776AB" />
<img src="https://img.shields.io/badge/HTML5-23272A?style=for-the-badge&logo=html5&logoColor=E34F26" />
<img src="https://img.shields.io/badge/CSS3-23272A?style=for-the-badge&logo=css3&logoColor=1572B6" />
<img src="https://img.shields.io/badge/Kotlin-23272A?style=for-the-badge&logo=kotlin&logoColor=7F52FF" />

**Backend & Tools**

<img src="https://img.shields.io/badge/Node.js-111827?style=for-the-badge&logo=nodedotjs&logoColor=339933" />
<img src="https://img.shields.io/badge/Flask-0B0F19?style=for-the-badge&logo=flask&logoColor=FFFFFF" />
<img src="https://img.shields.io/badge/Git-111827?style=for-the-badge&logo=git&logoColor=F05032" />
<img src="https://img.shields.io/badge/Linux-0F172A?style=for-the-badge&logo=linux&logoColor=FCC624" />

**Security**

<img src="https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white" />
<img src="https://img.shields.io/badge/TryHackMe-212C42?style=for-the-badge&logo=tryhackme&logoColor=white" />

**AI & Productivity**

<img src="https://img.shields.io/badge/GitHub_Copilot-000000?style=for-the-badge&logo=githubcopilot&logoColor=white" />
<img src="https://img.shields.io/badge/OpenAI-412991?style=for-the-badge&logo=openai&logoColor=white" />

</div>

---

## 🚀 Philosophy

**Start small → Ship fast → Learn continuously**

---

## 🌐 Connect

<div align="center">

[![Portfolio](https://img.shields.io/badge/🌐_PORTFOLIO-VISIT_NOW-00FFFF?style=for-the-badge&logo=vercel&logoColor=white&labelColor=0D1117)](https://vikaslavaniya.pages.dev/)
[![Studio](https://img.shields.io/badge/🎨_STUDIO-SYNTAX_ERROR-FF0080?style=for-the-badge&logo=cloudflare&logoColor=white&labelColor=0D1117)](https://syntaxerror.pages.dev/)
[![LinkedIn](https://img.shields.io/badge/💼_LINKEDIN-CONNECT_NOW-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0D1117)](https://www.linkedin.com/in/vikas-lavaniya-9b0771292)

</div>

---

<div align="center">

**Thanks for exploring my digital space! ⚡**

</div>
