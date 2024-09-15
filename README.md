<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 450 350" width="450" height="350">
  <!-- Background -->
  <defs>
    <linearGradient id="tvGradient" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#2e2e2e;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#1a1a1a;stop-opacity:1" />
    </linearGradient>
    <filter id="f1" x="0" y="0" width="200%" height="200%">
      <feOffset result="offOut" in="SourceGraphic" dx="5" dy="5" />
      <feGaussianBlur result="blurOut" in="offOut" stdDeviation="10" />
      <feBlend in="SourceGraphic" in2="blurOut" mode="normal" />
    </filter>
  </defs>

  <!-- TV Frame -->
  <rect x="25" y="25" rx="30" ry="30" width="400" height="250" fill="url(#tvGradient)" stroke="#000" stroke-width="8" />

  <!-- TV Shadow -->
  <rect x="25" y="25" rx="30" ry="30" width="400" height="250" fill="none" filter="url(#f1)" />

  <!-- TV Screen (GIF will go here) -->
  <rect x="50" y="50" rx="20" ry="20" width="350" height="175" fill="black" stroke="#fff" stroke-width="4" />
  <!-- Use this line to insert your GIF -->
  <image xlink:href="readme1.gif" x="50" y="50" width="350" height="175" />

  <!-- Screen Glow Animation -->
  <rect x="50" y="50" rx="20" ry="20" width="350" height="175" fill="none">
    <animate attributeName="stroke" values="#fff;#888;#fff" dur="3s" repeatCount="indefinite" />
  </rect>

  <!-- Antenna -->
  <line x1="120" y1="20" x2="90" y2="0" stroke="#fff" stroke-width="5" />
  <line x1="280" y1="20" x2="310" y2="0" stroke="#fff" stroke-width="5" />

  <!-- Knobs -->
  <circle cx="100" cy="260" r="15" fill="#444" stroke="#000" stroke-width="4" />
  <circle cx="150" cy="260" r="15" fill="#444" stroke="#000" stroke-width="4" />
  <circle cx="200" cy="260" r="15" fill="#444" stroke="#000" stroke-width="4" />

  <!-- Animated Knobs Glow -->
  <circle cx="100" cy="260" r="15" fill="none" stroke="#fff" stroke-width="2">
    <animate attributeName="stroke" values="#fff;#555;#fff" dur="2s" repeatCount="indefinite" />
  </circle>
  <circle cx="150" cy="260" r="15" fill="none" stroke="#fff" stroke-width="2">
    <animate attributeName="stroke" values="#fff;#555;#fff" dur="2.5s" repeatCount="indefinite" />
  </circle>
  <circle cx="200" cy="260" r="15" fill="none" stroke="#fff" stroke-width="2">
    <animate attributeName="stroke" values="#fff;#555;#fff" dur="3s" repeatCount="indefinite" />
  </circle>

  <!-- TV Stand -->
  <rect x="175" y="275" width="100" height="25" fill="#333" stroke="#000" stroke-width="5" />
</svg>
