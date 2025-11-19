<svg xmlns="http://www.w3.org/2000/svg" width="100%" height="220" viewBox="0 0 1200 220" preserveAspectRatio="xMidYMid meet" role="img" aria-label="Hero — SURYA PRAKASH">
  <defs>
    <linearGradient id="bg" x1="0" x2="1">
      <stop offset="0" stop-color="#000A0F"/>
      <stop offset="1" stop-color="#00060A"/>
    </linearGradient>

    <filter id="softGlow" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="6" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <filter id="textGlow" x="-100%" y="-100%" width="300%" height="300%">
      <feGaussianBlur stdDeviation="3" result="g1"/>
      <feColorMatrix in="g1" type="matrix" values="0 0 0 0 0
                                                    0 0 0 0 1
                                                    0 0 0 0 1
                                                    0 0 0 0.75 0" result="g2"/>
      <feMerge>
        <feMergeNode in="g2"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <style type="text/css"><![CDATA[
      .title { font-family: 'Orbitron','Exo 2', 'Segoe UI', Roboto, system-ui, sans-serif; font-weight:700; fill:#dffcff; font-size:48px; letter-spacing:6px; }
      .sub { font-family: 'Segoe UI', Roboto, system-ui, sans-serif; font-weight:500; fill:#aeefff; font-size:14px; letter-spacing:1px; opacity:0.95; }
      .hud-line { stroke:#00F7FF; stroke-opacity:0.16; stroke-width:1.6; filter:url(#softGlow); }
      .silhouette { stroke:#00F7FF; stroke-opacity:0.12; stroke-width:1.2; fill:none; }
    ]]></style>
  </defs>

  <rect x="0" y="0" width="1200" height="220" fill="url(#bg)"/>

  <g opacity="0.04" stroke="#00F7FF">
    <defs>
      <pattern id="grid" width="24" height="24" patternUnits="userSpaceOnUse">
        <path d="M 24 0 L 0 0 0 24" stroke="#00F7FF" stroke-width="0.5" stroke-opacity="0.45"/>
      </pattern>
    </defs>
    <rect x="20" y="10" width="760" height="190" fill="url(#grid)"/>
  </g>

  <g transform="translate(40,36)">
    <text class="title" x="0" y="40" filter="url(#textGlow)" style="fill:#bffcff">SURYA PRAKASH</text>

    <g transform="translate(0,60)">
      <text class="sub" x="0" y="0">AI Engineer</text>
      <text class="sub" x="0" y="24">Full Stack Developer</text>
      <text class="sub" x="0" y="48">Machine Learning &amp; Data Engineering</text>
      <text class="sub" x="0" y="72">Python | Django | C++ | MongoDB</text>
    </g>

    <line x1="0" x2="720" y1="160" y2="160" class="hud-line" stroke-linecap="round" />
  </g>

  <g transform="translate(920,12) scale(1)" opacity="0.95">
    <path class="silhouette" d="M40 20 C 70 10, 100 10, 120 40 C 140 70, 130 110, 100 130 C 70 150, 30 150, 10 120 C -10 90, 10 40, 40 20 Z" />
    <g stroke="#00F7FF" stroke-opacity="0.06" stroke-width="1">
      <path d="M4 110 L 116 18" />
      <path d="M16 120 L 110 30" />
    </g>
  </g>
</svg>

<div style="height:18px;"></div>

<svg xmlns="http://www.w3.org/2000/svg" width="100%" height="420" viewBox="0 0 1200 420" preserveAspectRatio="xMidYMid meet" role="img" aria-label="Information Orb — rotating holographic display">
  <defs>
    <radialGradient id="coreGlow" cx="50%" cy="50%">
      <stop offset="0%" stop-color="#00F7FF" stop-opacity="0.18"/>
      <stop offset="55%" stop-color="#00F7FF" stop-opacity="0.06"/>
      <stop offset="100%" stop-color="#000000" stop-opacity="0"/>
    </radialGradient>

    <linearGradient id="ringGrad" x1="0" x2="1">
      <stop offset="0" stop-color="#00F7FF" stop-opacity="0.12"/>
      <stop offset="1" stop-color="#0277BD" stop-opacity="0.06"/>
    </linearGradient>

    <style type="text/css"><![CDATA[
      .orb-bg { fill: #000A0F; }
      .orbit-ring { fill:none; stroke:url(#ringGrad); stroke-width:1.2; stroke-linecap:round; }
      .node { font-family: 'Segoe UI', Roboto, system-ui, sans-serif; font-size:12px; fill:#dffcff; letter-spacing:0.6px; }
      .nodeLabel { fill:#bffcff; font-size:11px; opacity:0.95; }
      .center-metrics { font-family: 'Orbitron','Exo 2', 'Segoe UI', sans-serif; fill:#e6ffff; text-anchor:middle; }
      .core { fill:url(#coreGlow); }
      @keyframes rotateCW { from { transform: rotate(0deg); } to { transform: rotate(360deg); } }
      @keyframes rotateCCW { from { transform: rotate(0deg); } to { transform: rotate(-360deg); } }
      .orbit-outer { transform-origin: 600px 210px; animation: rotateCW 26s linear infinite; }
      .orbit-mid   { transform-origin: 600px 210px; animation: rotateCCW 18s linear infinite; }
      .orbit-inner { transform-origin: 600px 210px; animation: rotateCW 12s linear infinite; }
      .orbit-slow  { transform-origin: 600px 210px; animation: rotateCCW 40s linear infinite; }
      .nodeCircle { fill:#00F7FF; opacity:0.12; stroke:#00F7FF; stroke-width:0.6; filter:drop-shadow(0 0 6px rgba(0,247,255,0.12)); }
      .wireframe { stroke:#00F7FF; stroke-opacity:0.06; stroke-width:0.8; fill:none; }
    ]]></style>
  </defs>

  <rect x="0" y="0" width="1200" height="420" class="orb-bg"/>

  <g transform="translate(40,20)" opacity="0.035" stroke="#00F7FF">
    <path d="M0 360 L1160 360" stroke-width="1"/>
    <path d="M0 320 L1160 320" stroke-width="0.6"/>
  </g>

  <g transform="translate(0,0)">
    <g transform="translate(600,210)">
      <circle r="56" class="core"/>
      <circle r="44" fill="none" stroke="#00F7FF" stroke-opacity="0.12" stroke-width="1.2"/>
      <text x="0" y="-6" class="center-metrics" font-size="16">Public Repos: 28</text>
      <text x="0" y="16" class="center-metrics" font-size="12" fill="#bffcff">Total Commits: 3,412</text>
    </g>

    <g stroke="#00F7FF" stroke-opacity="0.06" stroke-width="0.9">
      <circle cx="600" cy="210" r="120" class="wireframe" />
      <circle cx="600" cy="210" r="180" class="wireframe" />
      <circle cx="600" cy="210" r="240" class="wireframe" />
      <ellipse cx="600" cy="210" rx="312" ry="40" class="wireframe" transform="rotate(22 600 210)"/>
    </g>

    <g class="orbit-outer">
      <g transform="translate(600,210)">
        <g transform="translate(240,0)">
          <circle r="8" class="nodeCircle"/>
          <text x="18" y="5" class="nodeLabel">MongoDB</text>
        </g>
        <g transform="rotate(40) translate(240,0)">
          <circle r="6.5" class="nodeCircle"/>
          <text x="18" y="5" class="nodeLabel">CSS</text>
        </g>
        <g transform="rotate(80) translate(240,0)">
          <circle r="6.5" class="nodeCircle"/>
          <text x="18" y="5" class="nodeLabel">HTML</text>
        </g>
        <g transform="rotate(120) translate(240,0)">
          <circle r="7.2" class="nodeCircle"/>
          <text x="18" y="5" class="nodeLabel">JavaScript</text>
        </g>
        <g transform="rotate(160) translate(240,0)">
          <circle r="6" class="nodeCircle"/>
          <text x="18" y="5" class="nodeLabel">C++</text>
        </g>
        <g transform="rotate(200) translate(240,0)">
          <circle r="6.5" class="nodeCircle"/>
          <text x="18" y="5" class="nodeLabel">Django</text>
        </g>
        <g transform="rotate(240) translate(240,0)">
          <circle r="7.8" class="nodeCircle"/>
          <text x="18" y="5" class="nodeLabel">Python</text>
        </g>
        <g transform="rotate(280) translate(240,0)">
          <circle r="5.8" class="nodeCircle"/>
          <text x="18" y="5" class="nodeLabel">SQLite</text>
        </g>
      </g>
    </g>

    <g class="orbit-mid">
      <g transform="translate(600,210)">
        <g transform="translate(180,0)">
          <circle r="5.5" class="nodeCircle"/>
          <text x="14" y="4" class="nodeLabel">Git</text>
        </g>
        <g transform="rotate(60) translate(180,0)">
          <circle r="5.5" class="nodeCircle"/>
          <text x="14" y="4" class="nodeLabel">Linux</text>
        </g>
        <g transform="rotate(120) translate(180,0)">
          <circle r="6.2" class="nodeCircle"/>
          <text x="14" y="4" class="nodeLabel">VS Code</text>
        </g>
        <g transform="rotate(180) translate(180,0)">
          <circle r="5.5" class="nodeCircle"/>
          <text x="14" y="4" class="nodeLabel">NumPy</text>
        </g>
        <g transform="rotate(240) translate(180,0)">
          <circle r="5.5" class="nodeCircle"/>
          <text x="14" y="4" class="nodeLabel">Pandas</text>
        </g>
        <g transform="rotate(300) translate(180,0)">
          <circle r="5.5" class="nodeCircle"/>
          <text x="14" y="4" class="nodeLabel">Matplotlib</text>
        </g>
      </g>
    </g>

    <g class="orbit-inner">
      <g transform="translate(600,210)">
        <g transform="translate(120,0)">
          <circle r="4.6" class="nodeCircle"/>
          <text x="12" y="4" class="nodeLabel">Stack</text>
        </g>
        <g transform="rotate(120) translate(120,0)">
          <circle r="4.6" class="nodeCircle"/>
          <text x="12" y="4" class="nodeLabel">DevOps</text>
        </g>
        <g transform="rotate(240) translate(120,0)">
          <circle r="4.6" class="nodeCircle"/>
          <text x="12" y="4" class="nodeLabel">DataEng</text>
        </g>
      </g>
    </g>

    <g class="orbit-slow">
      <g transform="translate(600,210)">
        <g transform="translate(312,0)">
          <circle r="3.6" class="nodeCircle"/>
          <text x="10" y="4" class="nodeLabel">CI</text>
        </g>
      </g>
    </g>
  </g>
</svg>

<div style="height:18px;"></div>

<svg xmlns="http://www.w3.org/2000/svg" width="100%" height="260" viewBox="0 0 1200 260" preserveAspectRatio="xMidYMid meet" role="img" aria-label="My GitHub Contribution Activity">
  <defs>
    <linearGradient id="barGrad" x1="0" x2="0" y1="0" y2="1">
      <stop offset="0" stop-color="#00F7FF" stop-opacity="0.98"/>
      <stop offset="1" stop-color="#0277BD" stop-opacity="0.8"/>
    </linearGradient>

    <style type="text/css"><![CDATA[
      .bg { fill:#000A0F; }
      .grid-line { stroke:#0277BD; stroke-opacity:0.08; stroke-width:1; }
      .dateLabel { fill:#92fbff; font-size:12px; font-family:'Segoe UI', Roboto, system-ui, sans-serif; text-anchor:middle; opacity:0.95; }
      .bar { fill:url(#barGrad); filter: drop-shadow(0 0 6px rgba(0,247,255,0.08)); }
      .title { font-family: 'Orbitron','Exo 2','Segoe UI', sans-serif; font-size:18px; fill:#dffcff; }
      .axis { stroke:#00F7FF; stroke-opacity:0.06; stroke-width:1; }
    ]]></style>
  </defs>

  <rect x="0" y="0" width="1200" height="260" class="bg"/>

  <text x="40" y="34" class="title">My GitHub Contribution Activity</text>

  <g transform="translate(40,60)">
    <g>
      <line x1="0" y1="0" x2="1120" y2="0" class="grid-line"/>
      <line x1="0" y1="36" x2="1120" y2="36" class="grid-line"/>
      <line x1="0" y1="72" x2="1120" y2="72" class="grid-line"/>
      <line x1="0" y1="108" x2="1120" y2="108" class="grid-line"/>
      <line x1="0" y1="144" x2="1120" y2="144" class="grid-line"/>
    </g>

    <line x1="0" y1="0" x2="0" y2="160" class="axis"/>

    <g transform="translate(0,0)">
      <rect x="0" y="110" width="64" height="50" class="bar" rx="5" ry="5" />
      <text class="dateLabel" x="32" y="146">2025-11-06</text>
      <text class="dateLabel" x="32" y="102" style="font-size:11px; opacity:0.9;">2</text>
    </g>

    <g transform="translate(80,0)">
      <rect x="0" y="62" width="64" height="98" class="bar" rx="5" ry="5" />
      <text class="dateLabel" x="32" y="146">2025-11-07</text>
      <text class="dateLabel" x="32" y="54" style="font-size:11px; opacity:0.9;">5</text>
    </g>

    <g transform="translate(160,0)">
      <rect x="0" y="92" width="64" height="68" class="bar" rx="5" ry="5" />
      <text class="dateLabel" x="32" y="146">2025-11-08</text>
      <text class="dateLabel" x="32" y="84" style="font-size:11px; opacity:0.9;">3</text>
    </g>

    <g transform="translate(240,0)">
      <rect x="0" y="140" width="64" height="20" class="bar" rx="5" ry="5" opacity="0.06"/>
      <text class="dateLabel" x="32" y="146">2025-11-09</text>
      <text class="dateLabel" x="32" y="134" style="font-size:11px; opacity:0.7;">0</text>
    </g>

    <g transform="translate(320,0)">
      <rect x="0" y="76" width="64" height="84" class="bar" rx="5" ry="5" />
      <text class="dateLabel" x="32" y="146">2025-11-10</text>
      <text class="dateLabel" x="32" y="68" style="font-size:11px; opacity:0.9;">4</text>
    </g>

    <g transform="translate(400,0)">
      <rect x="0" y="46" width="64" height="114" class="bar" rx="5" ry="5" />
      <text class="dateLabel" x="32" y="146">2025-11-11</text>
      <text class="dateLabel" x="32" y="38" style="font-size:11px; opacity:0.9;">6</text>
    </g>

    <g transform="translate(480,0)">
      <rect x="0" y="128" width="64" height="32" class="bar" rx="5" ry="5" />
      <text class="dateLabel" x="32" y="146">2025-11-12</text>
      <text class="dateLabel" x="32" y="120" style="font-size:11px; opacity:0.9;">1</text>
    </g>

    <g transform="translate(560,0)">
      <rect x="0" y="140" width="64" height="20" class="bar" rx="5" ry="5" opacity="0.06"/>
      <text class="dateLabel" x="32" y="146">2025-11-13</text>
      <text class="dateLabel" x="32" y="134" style="font-size:11px; opacity:0.7;">0</text>
    </g>

    <g transform="translate(640,0)">
      <rect x="0" y="92" width="64" height="68" class="bar" rx="5" ry="5" />
      <text class="dateLabel" x="32" y="146">2025-11-14</text>
      <text class="dateLabel" x="32" y="84" style="font-size:11px; opacity:0.9;">3</text>
    </g>

    <g transform="translate(720,0)">
      <rect x="0" y="110" width="64" height="50" class="bar" rx="5" ry="5" />
      <text class="dateLabel" x="32" y="146">2025-11-15</text>
      <text class="dateLabel" x="32" y="102" style="font-size:11px; opacity:0.9;">2</text>
    </g>

    <g transform="translate(800,0)">
      <rect x="0" y="140" width="64" height="20" class="bar" rx="5" ry="5" opacity="0.06"/>
      <text class="dateLabel" x="32" y="146">2025-11-16</text>
      <text class="dateLabel" x="32" y="134" style="font-size:11px; opacity:0.7;">0</text>
    </g>

    <g transform="translate(880,0)">
      <rect x="0" y="76" width="64" height="84" class="bar" rx="5" ry="5" />
      <text class="dateLabel" x="32" y="146">2025-11-17</text>
      <text class="dateLabel" x="32" y="68" style="font-size:11px; opacity:0.9;">4</text>
    </g>

    <g transform="translate(960,0)">
      <rect x="0" y="22" width="64" height="138" class="bar" rx="5" ry="5" />
      <text class="dateLabel" x="32" y="146">2025-11-18</text>
      <text class="dateLabel" x="32" y="14" style="font-size:11px; opacity:0.95;">7</text>
    </g>

    <g transform="translate(1040,0)">
      <rect x="0" y="62" width="64" height="98" class="bar" rx="5" ry="5" />
      <text class="dateLabel" x="32" y="146">2025-11-19</text>
      <text class="dateLabel" x="32" y="54" style="font-size:11px; opacity:0.9;">5</text>
    </g>
  </g>

  <line x1="40" x2="1160" y1="234" y2="234" stroke="#00F7FF" stroke-opacity="0.06" stroke-width="1" />
</svg>

<div style="height:18px;"></div>

<svg xmlns="http://www.w3.org/2000/svg" width="100%" height="120" viewBox="0 0 1200 120" preserveAspectRatio="xMidYMid meet" role="img" aria-label="Connect With Me">
  <defs>
    <style type="text/css"><![CDATA[
      .bg { fill:#000A0F; }
      .title { font-family: 'Orbitron','Exo 2','Segoe UI', sans-serif; font-size:16px; fill:#dffcff; }
      .btn { font-family:'Segoe UI', Roboto, system-ui, sans-serif; font-size:13px; fill:#dffcff; text-anchor:middle; cursor:pointer; }
      .rect { fill:none; stroke:#00F7FF; stroke-width:1.2; rx:6; ry:6; opacity:0.9; }
      .rect:hover { filter: drop-shadow(0 0 8px rgba(0,247,255,0.14)); }
      a { text-decoration: none; }
    ]]></style>
  </defs>

  <rect class="bg" width="1200" height="120"/>

  <text x="40" y="36" class="title">Connect With Me</text>

  <g transform="translate(40,50)">
    <a xlink:href="https://www.linkedin.com/in/surya-prakash" target="_blank" rel="noopener noreferrer">
      <rect class="rect" x="0" y="0" width="210" height="40"></rect>
      <text class="btn" x="105" y="26">LinkedIn</text>
    </a>

    <a xlink:href="https://github.com/Surya-ux-max" target="_blank" rel="noopener noreferrer" transform="translate(240,0)">
      <g transform="translate(240,0)">
        <rect class="rect" x="0" y="0" width="210" height="40"></rect>
        <text class="btn" x="105" y="26">GitHub</text>
      </g>
    </a>

    <a xlink:href="https://surya-ux-max.dev" target="_blank" rel="noopener noreferrer" transform="translate(480,0)">
      <g transform="translate(480,0)">
        <rect class="rect" x="0" y="0" width="210" height="40"></rect>
        <text class="btn" x="105" y="26">Portfolio Website</text>
      </g>
    </a>

    <a xlink:href="mailto:surya.prakash@example.com" transform="translate(720,0)">
      <g transform="translate(720,0)">
        <rect class="rect" x="0" y="0" width="210" height="40"></rect>
        <text class="btn" x="105" y="26">Email</text>
      </g>
    </a>
  </g>
</svg>

<div style="color:#9feffb; font-family: 'Segoe UI', Roboto, system-ui, sans-serif; font-size:13px; margin-top:10px;">
  LinkedIn: https://www.linkedin.com/in/surya-prakash  
  GitHub: https://github.com/Surya-ux-max  
  Portfolio: https://surya-ux-max.dev  
  Email: surya.prakash@example.com
</div>

<div style="margin-top:14px; color:#7feff8; font-family: 'Segoe UI', Roboto, system-ui, sans-serif; font-size:12px;">
  Design: Dark HUD — neon cyan accents. Orb rotation is implemented with CSS-only animation inside SVG. No external scripts.
</div>
