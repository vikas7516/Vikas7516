Vikas — Build. Learn. Ship. ⚡
Crafting simple, useful software and learning in public. Focus on web dev, IT support, and cybersecurity—with experiments in Android and AI tooling.

<p align="center"> <svg width="100%" height="230" viewBox="0 0 1200 360" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Vikas — Build. Learn. Ship."> <defs> <!-- Gradients --> <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1"> <stop offset="0%" stop-color="#0B0F19"/> <stop offset="100%" stop-color="#111827"/> </linearGradient> <linearGradient id="accent" x1="0" y1="0" x2="1" y2="0"> <stop offset="0%" stop-color="#8A2BE2"/> <stop offset="50%" stop-color="#00E5FF"/> <stop offset="100%" stop-color="#22C55E"/> </linearGradient> <radialGradient id="glow1" cx="80%" cy="15%" r="40%"> <stop offset="0%" stop-color="#8A2BE2" stop-opacity="0.35"/> <stop offset="100%" stop-color="#8A2BE2" stop-opacity="0"/> </radialGradient> <radialGradient id="glow2" cx="15%" cy="85%" r="45%"> <stop offset="0%" stop-color="#00E5FF" stop-opacity="0.25"/> <stop offset="100%" stop-color="#00E5FF" stop-opacity="0"/> </radialGradient>
text
  <!-- Soft shadow -->
  <filter id="soft">
    <feGaussianBlur stdDeviation="18" result="blur"/>
    <feMerge>
      <feMergeNode in="blur"/>
      <feMergeNode in="SourceGraphic"/>
    </feMerge>
  </filter>

  <!-- Inner glow for tags -->
  <filter id="innerGlow" x="-50%" y="-50%" width="200%" height="200%">
    <feOffset dx="0" dy="0"/>
    <feGaussianBlur stdDeviation="2" result="glow"/>
    <feComposite in2="SourceAlpha" operator="arithmetic" k2="-1" k3="1" />
    <feColorMatrix type="matrix" values="0 0 0 0 0.55  0 0 0 0 0.8  0 0 0 0 1  0 0 0 0.8 0"/>
    <feMerge>
      <feMergeNode/>
      <feMergeNode in="SourceGraphic"/>
    </feMerge>
  </filter>

  <!-- Tag styles via <style> -->
  <style>
    .title { font: 700 46px 'Segoe UI', Inter, Roboto, Arial, sans-serif; fill: #E5E7EB; }
    .tagline { font: 400 20px 'Segoe UI', Inter, Roboto, Arial, sans-serif; fill: #9CA3AF; }
    .chip text { font: 600 13px 'Segoe UI', Inter, Roboto, Arial, sans-serif; }
    .chip rect { rx: 14; ry: 14; }
    .chip:hover { filter: url(#innerGlow); }
    .chip rect.bg { fill: #0B1220; opacity: 0.85; }
    .chip rect.stroke-purple { stroke: #8B5CF6; stroke-width: 1.2; }
    .chip rect.stroke-cyan { stroke: #06B6D4; stroke-width: 1.2; }
    .chip rect.stroke-green { stroke: #22C55E; stroke-width: 1.2; }
    .chip text.purple { fill: #EDE9FE; }
    .chip text.cyan { fill: #CFFAFE; }
    .chip text.green { fill: #DCFCE7; }
    .chip { transition: transform 250ms ease, opacity 250ms ease; }
    .chip:hover { transform: translateY(-2px) scale(1.02); opacity: 1; }
    .float-slow { animation: float1 6s ease-in-out infinite; }
    .float-mid { animation: float2 7.5s ease-in-out infinite; }
    .float-fast { animation: float3 5.5s ease-in-out infinite; }
    @keyframes float1 { 0% { transform: translateY(0) } 50% { transform: translateY(-6px) } 100% { transform: translateY(0) } }
    @keyframes float2 { 0% { transform: translateY(0) } 50% { transform: translateY(-10px) } 100% { transform: translateY(0) } }
    @keyframes float3 { 0% { transform: translateY(0) } 50% { transform: translateY(-4px) } 100% { transform: translateY(0) } }
    .divider { opacity: 0.8; }
  </style>
</defs>

<!-- Background panel -->
<rect width="1200" height="300" fill="url(#bg)" rx="16"/>

<!-- Ambient glows -->
<circle cx="980" cy="70" r="220" fill="url(#glow1)" filter="url(#soft)"/>
<circle cx="160" cy="250" r="240" fill="url(#glow2)" filter="url(#soft)"/>

<!-- Accent wave -->
<path d="M40,240 C200,180 420,230 620,205 C820,180 1020,225 1160,190" stroke="url(#accent)" stroke-width="3" fill="none" opacity="0.85"/>

<!-- Header text -->
<text x="60" y="130" class="title">Vikas</text>
<text x="60" y="172" class="tagline">Build. Learn. Ship. — Backend -  Security -  Android (exploring)</text>

<!-- Tag chips row with spacing -->
<g transform="translate(60, 200)">
  <!-- chip 1 -->
  <g class="chip float-slow">
    <rect class="bg" width="188" height="34"/>
    <rect class="stroke-cyan" width="188" height="34" fill="transparent"/>
    <text class="cyan" x="14" y="22">Learning in public</text>
  </g>

  <!-- spacer -->
  <g transform="translate(208,0)"></g>

  <!-- chip 2 -->
  <g class="chip float-mid" transform="translate(208,0)">
    <rect class="bg" width="196" height="34"/>
    <rect class="stroke-green" width="196" height="34" fill="transparent"/>
    <text class="green" x="14" y="22">Backend + Security</text>
  </g>

  <!-- spacer -->
  <g transform="translate(424,0)"></g>

  <!-- chip 3 -->
  <g class="chip float-fast" transform="translate(424,0)">
    <rect class="bg" width="220" height="34"/>
    <rect class="stroke-purple" width="220" height="34" fill="transparent"/>
    <text class="purple" x="14" y="22">Android + AI (exploring)</text>
  </g>
</g>

<!-- subtle divider -->
<path class="divider" d="M60,260 L1140,260" stroke="#1F2937" stroke-width="1"/>
</svg> </p> <p align="center"> <a href="https://vikaslavaniya.pages.dev/"> <img src="https://img.shields.io/badge/Portfolio-Visit-111827?style=for-the-badge&logo=firefoxbrowser&logoColor=00E5FF&labelColor=0B0F19&color=111827" alt="Portfolio" /> </a> <a href="https://syntaxerror.pages.dev/"> <img src="https://img.shields.io/badge/Studio-SyntaxError-0F172A?style=for-the-badge&logo=cloudflarepages&logoColor=F97316&labelColor=0B0F19&color=0F172A" alt="Studio" /> </a> <a href="https://www.linkedin.com/in/vikas-lavaniya-9b0771292"> <img src="https://img.shields.io/badge/LinkedIn-Vikas%20Lavaniya-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0B0F19" alt="LinkedIn" /> </a> </p>
Snapshot 🌈
Student dev shipping small, honest projects and notes.

Learning backend fundamentals, networks, and security labs.

Documenting progress to stay accountable and improve.

What I’m Learning Now 📚
Node.js + Flask: REST, routing, simple auth.

Linux + networking: ports, packets, CLI tooling.

TryHackMe beginner rooms: write-ups and takeaways.

Android + Kotlin: UI basics and tiny prototypes.

Stack & Tools 🎒
<p align="left"> <img src="https://img.shields.io/badge/HTML-23272A?style=for-the-badge&logo=html5&logoColor=E34F26" /> <img src="https://img.shields.io/badge/CSS-23272A?style=for-the-badge&logo=css3&logoColor=1572B6" /> <img src="https://img.shields.io/badge/JavaScript-23272A?style=for-the-badge&logo=javascript&logoColor=F7DF1E" /> <img src="https://img.shields.io/badge/Python-23272A?style=for-the-badge&logo=python&logoColor=3776AB" /> <img src="https://img.shields.io/badge/Node.js-111827?style=for-the-badge&logo=nodedotjs&logoColor=00DC82" /> <img src="https://img.shields.io/badge/Flask-0B0F19?style=for-the-badge&logo=flask&logoColor=FFFFFF" /> <img src="https://img.shields.io/badge/Linux-0F172A?style=for-the-badge&logo=linux&logoColor=FCC624" /> <img src="https://img.shields.io/badge/Git-111827?style=for-the-badge&logo=git&logoColor=F05032" /> <img src="https://img.shields.io/badge/Wireshark-0B2942?style=for-the-badge&logo=wireshark&logoColor=4BC0F8" /> <img src="https://img.shields.io/badge/TryHackMe-0F0F0F?style=for-the-badge&logo=tryhackme&logoColor=E62E2E" /> <img src="https://img.shields.io/badge/Kotlin-111827?style=for-the-badge&logo=kotlin&logoColor=7F52FF" /> </p>
Languages: JavaScript, Python, HTML, CSS

Backend: Node.js, Flask

Platforms: Linux, Git/GitHub

Security: Wireshark(basic), TryHackMe

AI helpers: Copilot, Cursor, OpenAI API(exploring)

Current Goals 🎯
Finish Google IT Support certification.

Ship 2–3 tiny backend APIs with clean docs.

Publish short TryHackMe notes in /notes.

Activity Highlights 📈
<p align="center"> <img src="https://github-readme-stats.vercel.app/api?username=vikas7516&show_icons=true&hide_title=true&count_private=true&theme=tokyonight&bg_color=0B0F19&title_color=8A2BE2&text_color=E5E7EB&icon_color=00E5FF&hide_border=true" height="150" alt="GitHub stats" /> <img src="https://github-readme-streak-stats.herokuapp.com?user=vikas7516&theme=tokyonight&background=0B0F19&ring=8A2BE2&fire=22C55E&currStreakLabel=00E5FF&sideNums=E5E7EB&sideLabels=9CA3AF&dates=6B7280&hide_border=true" height="150" alt="GitHub streak" /> </p> <p align="center"> <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=vikas7516&layout=compact&langs_count=8&theme=tokyonight&bg_color=0B0F19&title_color=8A2BE2&text_color=E5E7EB&hide_border=true" height="150" alt="Top languages" /> </p>
How I Work 🧠
Start small → ship early → iterate.

Prefer clarity over complexity.

Learn by breaking and fixing.

Connect 🌐
Portfolio: https://vikaslavaniya.pages.dev/

Studio: https://syntaxerror.pages.dev/

LinkedIn: https://www.linkedin.com/in/vikas-lavaniya-9b0771292
