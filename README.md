# Vikas — Build. Learn. Ship. ⚡

<div align="center">
  <svg width="100%" height="280" viewBox="0 0 1200 400" xmlns="http://www.w3.org/2000/svg">
    <defs>
      <linearGradient id="bgGradient" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" stop-color="#0B0F19">
          <animate attributeName="stop-color" values="#0B0F19;#1a1a2e;#16213e;#0B0F19" dur="8s" repeatCount="indefinite"/>
        </stop>
        <stop offset="50%" stop-color="#111827">
          <animate attributeName="stop-color" values="#111827;#0f3460;#533483;#111827" dur="10s" repeatCount="indefinite"/>
        </stop>
        <stop offset="100%" stop-color="#1F2937">
          <animate attributeName="stop-color" values="#1F2937;#0e4b99;#2a1810;#1F2937" dur="12s" repeatCount="indefinite"/>
        </stop>
      </linearGradient>

      <linearGradient id="accentGradient" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stop-color="#8A2BE2">
          <animate attributeName="stop-color" values="#8A2BE2;#FF6B6B;#4ECDC4;#45B7D1;#8A2BE2" dur="6s" repeatCount="indefinite"/>
        </stop>
        <stop offset="33%" stop-color="#00E5FF">
          <animate attributeName="stop-color" values="#00E5FF;#96CEB4;#FFEAA7;#DDA0DD;#00E5FF" dur="8s" repeatCount="indefinite"/>
        </stop>
        <stop offset="66%" stop-color="#22C55E">
          <animate attributeName="stop-color" values="#22C55E;#FD79A8;#FDCB6E;#6C5CE7;#22C55E" dur="10s" repeatCount="indefinite"/>
        </stop>
        <stop offset="100%" stop-color="#F97316">
          <animate attributeName="stop-color" values="#F97316;#A29BFE;#FD79A8;#00CEC9;#F97316" dur="7s" repeatCount="indefinite"/>
        </stop>
      </linearGradient>

      <radialGradient id="glow1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stop-color="#8A2BE2" stop-opacity="0.4">
          <animate attributeName="stop-opacity" values="0.4;0.8;0.2;0.6;0.4" dur="4s" repeatCount="indefinite"/>
        </stop>
        <stop offset="100%" stop-color="#8A2BE2" stop-opacity="0"/>
      </radialGradient>

      <radialGradient id="glow2" cx="50%" cy="50%" r="60%">
        <stop offset="0%" stop-color="#00E5FF" stop-opacity="0.3">
          <animate attributeName="stop-opacity" values="0.3;0.7;0.1;0.5;0.3" dur="5s" repeatCount="indefinite"/>
        </stop>
        <stop offset="100%" stop-color="#00E5FF" stop-opacity="0"/>
      </radialGradient>

      <filter id="glow" x="-50%" y="-50%" width="200%" height="200%">
        <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
        <feMerge>
          <feMergeNode in="coloredBlur"/>
          <feMergeNode in="SourceGraphic"/>
        </feMerge>
      </filter>

      <filter id="shadow" x="-50%" y="-50%" width="200%" height="200%">
        <feDropShadow dx="0" dy="4" stdDeviation="8" flood-color="#000" flood-opacity="0.3"/>
      </filter>

      <style>
        .title-main { 
          font: 700 52px 'Segoe UI', Inter, sans-serif; 
          fill: #E5E7EB; 
          filter: url(#glow);
        }
        .title-accent { 
          font: 700 52px 'Segoe UI', Inter, sans-serif; 
          fill: url(#accentGradient); 
        }
        .tagline { 
          font: 400 18px 'Segoe UI', Inter, sans-serif; 
          fill: #9CA3AF; 
        }
        .chip {
          transition: transform 0.3s ease;
        }
        .chip:hover {
          transform: translateY(-2px);
        }
        .particle {
          animation: float 6s ease-in-out infinite;
        }
        .pulse {
          animation: pulse 4s ease-in-out infinite;
        }
        @keyframes float {
          0%, 100% { transform: translateY(0); opacity: 0.6; }
          50% { transform: translateY(-20px); opacity: 0.8; }
        }
        @keyframes pulse {
          0%, 100% { opacity: 0.6; }
          50% { opacity: 1; }
        }
      </style>
    </defs>

    <!-- Background -->
    <rect width="1200" height="400" fill="url(#bgGradient)" rx="20"/>

    <!-- Particles -->
    <g class="particles">
      <circle class="particle" cx="150" cy="80" r="2" fill="#8A2BE2" opacity="0.6"/>
      <circle class="particle" cx="300" cy="120" r="1.5" fill="#00E5FF" opacity="0.4"/>
      <circle class="particle" cx="450" cy="90" r="3" fill="#22C55E" opacity="0.5"/>
      <circle class="particle" cx="600" cy="110" r="2.5" fill="#F97316" opacity="0.6"/>
      <circle class="particle" cx="750" cy="85" r="2" fill="#8A2BE2" opacity="0.4"/>
      <circle class="particle" cx="900" cy="100" r="1.5" fill="#00E5FF" opacity="0.5"/>
    </g>

    <!-- Ambient Glows -->
    <circle cx="950" cy="100" r="180" fill="url(#glow1)" class="pulse"/>
    <circle cx="200" cy="280" r="200" fill="url(#glow2)" class="pulse"/>

    <!-- Wave -->
    <path stroke="url(#accentGradient)" stroke-width="4" fill="none" opacity="0.9">
      <animate attributeName="d" values="M40,280 Q300,260 600,275 T1160,260;M40,300 Q300,280 600,295 T1160,280;M40,280 Q300,260 600,275 T1160,260" dur="8s" repeatCount="indefinite"/>
    </path>

    <!-- Title -->
    <text x="70" y="150" class="title-main">Vi</text>
    <text x="140" y="150" class="title-accent">kas</text>

    <!-- Tagline -->
    <text x="70" y="190" class="tagline">
      Build. Learn. Ship. — Backend • Security • Android
      <animate attributeName="opacity" values="0.7;1;0.7" dur="4s" repeatCount="indefinite"/>
    </text>

    <!-- Chips -->
    <g transform="translate(70, 240)">
      <g class="chip">
        <rect width="180" height="32" rx="16" fill="rgba(15,18,32,0.8)" stroke="#06B6D4" stroke-width="1"/>
        <text x="90" y="20" fill="#CFFAFE" text-anchor="middle" font-size="12" font-family="Segoe UI">Learning in public</text>
      </g>
      <g class="chip" transform="translate(200,0)">
        <rect width="180" height="32" rx="16" fill="rgba(15,18,32,0.8)" stroke="#22C55E" stroke-width="1"/>
        <text x="90" y="20" fill="#DCFCE7" text-anchor="middle" font-size="12" font-family="Segoe UI">Backend + Security</text>
      </g>
      <g class="chip" transform="translate(400,0)">
        <rect width="200" height="32" rx="16" fill="rgba(15,18,32,0.8)" stroke="#8B5CF6" stroke-width="1"/>
        <text x="100" y="20" fill="#EDE9FE" text-anchor="middle" font-size="12" font-family="Segoe UI">Android + AI (exploring)</text>
      </g>
    </g>

    <!-- Bottom Line -->
    <rect x="70" y="380" width="1060" height="2" fill="url(#accentGradient)" opacity="0.6" rx="1">
      <animate attributeName="opacity" values="0.6;1;0.6" dur="3s" repeatCount="indefinite"/>
    </rect>
  </svg>
</div>

<p align="center">
  <a href="https://vikaslavaniya.pages.dev/">
    <img src="https://img.shields.io/badge/🌐_Portfolio-Visit_Now-111827?style=for-the-badge&logo=vercel&logoColor=00E5FF&labelColor=0B0F19" alt="Portfolio" />
  </a>
  <a href="https://syntaxerror.pages.dev/">
    <img src="https://img.shields.io/badge/🎨_Studio-SyntaxError-0F172A?style=for-the-badge&logo=cloudflarepages&logoColor=F97316&labelColor=0B0F19" alt="Studio" />
  </a>
  <a href="https://www.linkedin.com/in/vikas-lavaniya-9b0771292">
    <img src="https://img.shields.io/badge/💼_LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0B0F19" alt="LinkedIn" />
  </a>
</p>

![Profile Views](https://komarev.com/ghpvc/?username=vikas7516&color=8A2BE2&style=flat-square&label=Profile+Views)
![GitHub followers](https://img.shields.io/github/followers/vikas7516?style=social)

---

## 📊 Activity Highlights

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=vikas7516&show_icons=true&hide_title=true&count_private=true&theme=tokyonight&bg_color=0B0F19&title_color=8A2BE2&text_color=E5E7EB&icon_color=00E5FF&hide_border=true" height="180" alt="GitHub stats" />
  <img src="https://github-readme-streak-stats.herokuapp.com?user=vikas7516&theme=tokyonight&background=0B0F19&ring=8A2BE2&fire=22C55E&currStreakLabel=00E5FF&sideNums=E5E7EB&sideLabels=9CA3AF&dates=6B7280&hide_border=true" height="180" alt="GitHub streak" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=vikas7516&layout=compact&langs_count=10&theme=tokyonight&bg_color=0B0F19&title_color=8A2BE2&text_color=E5E7EB&hide_border=true" height="180" alt="Top languages" />
</p>

---

## 🚀 Current Focus

| 📚 Learning Journey | 🎯 Goals |
|---------------------|----------|
| **Backend Development**: Node.js, Flask, REST APIs | ☐ Complete Google IT Support certification |
| **System Administration**: Linux, networking fundamentals | ☐ Build 3 production-ready REST APIs |
| **Cybersecurity**: TryHackMe labs, Wireshark analysis | ☐ Publish TryHackMe writeups |
| **Mobile Development**: Kotlin basics, Flutter exploration | ☐ Launch first Android app prototype |
| **AI Integration**: OpenAI API, automation workflows | ☐ Contribute to open source projects |

---

## 🛠️ Tech Arsenal

<div align="center">

**Languages & Frameworks**

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

**Security & Analysis**

<img src="https://img.shields.io/badge/Wireshark-0B2942?style=for-the-badge&logo=wireshark&logoColor=4BC0F8" />
<img src="https://img.shields.io/badge/TryHackMe-0F0F0F?style=for-the-badge&logo=tryhackme&logoColor=C11111" />

**AI & Productivity**

<img src="https://img.shields.io/badge/GitHub_Copilot-111827?style=for-the-badge&logo=githubcopilot&logoColor=FFFFFF" />
<img src="https://img.shields.io/badge/OpenAI_API-0F172A?style=for-the-badge&logo=openai&logoColor=412991" />

</div>

---

## 🎨 How I Work

**Philosophy**: *Start small → Ship fast → Learn continuously*

---

## 🌐 Connect & Collaborate

<div align="center">

[![Portfolio](https://img.shields.io/badge/🌐_Portfolio-Visit_Now-111827?style=for-the-badge&logo=vercel&logoColor=00E5FF)](https://vikaslavaniya.pages.dev/)
[![Studio](https://img.shields.io/badge/🎨_Studio-SyntaxError-0F172A?style=for-the-badge&logo=cloudflarepages&logoColor=F97316)](https://syntaxerror.pages.dev/)
[![LinkedIn](https://img.shields.io/badge/💼_LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vikas-lavaniya-9b0771292)

</div>

---

<div align="center">

**Thanks for visiting! 🚀**

</div>
