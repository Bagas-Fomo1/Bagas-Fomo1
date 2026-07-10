<svg width="900" height="160" viewBox="0 0 900 160" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <style>
      .base { font-family: 'Courier New', monospace; font-weight: bold; }
      .title { font-size: 46px; }
      .sub { font-size: 16px; letter-spacing: 2px; }
    </style>
    <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#000000"/>
      <stop offset="50%" stop-color="#1a0505"/>
      <stop offset="100%" stop-color="#8B0000"/>
    </linearGradient>
  </defs>

  <rect width="900" height="160" fill="url(#bg)"/>

  <!-- scanline sweep -->
  <rect x="0" y="0" width="900" height="2" fill="#ffffff" opacity="0.06">
    <animate attributeName="y" values="0;160;0" dur="3.5s" repeatCount="indefinite"/>
  </rect>

  <!-- red channel -->
  <text x="450" y="75" text-anchor="middle" class="base title" fill="#ff1a1a" opacity="0.85">
    KEPO YA MBUD
    <animateTransform attributeName="transform" type="translate"
      values="0 0; -3 0; 2 0; -1 0; 0 0" dur="0.35s" repeatCount="indefinite"/>
  </text>

  <!-- cyan channel (dim, biar tetap red-dominant) -->
  <text x="450" y="75" text-anchor="middle" class="base title" fill="#00e5ff" opacity="0.35">
    KEPO YA MBUD
    <animateTransform attributeName="transform" type="translate"
      values="0 0; 3 0; -2 0; 1 0; 0 0" dur="0.3s" repeatCount="indefinite"/>
  </text>

  <!-- base white text -->
  <text x="450" y="75" text-anchor="middle" class="base title" fill="#f5f5f5">
    KEPO YA MBUD
  </text>

  <!-- subtitle -->
  <text x="450" y="105" text-anchor="middle" class="base sub" fill="#ff4d4d">
    [ ROOT ACCESS GRANTED ]
    <animate attributeName="opacity" values="1;0.4;1" dur="1.2s" repeatCount="indefinite"/>
  </text>

  <!-- glitch bands -->
  <rect x="0" y="45" width="900" height="6" fill="#ff1a1a" opacity="0.4">
    <animate attributeName="y" values="45;95;35;80;45" dur="1.6s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.4;0;0.3;0;0.4" dur="1.6s" repeatCount="indefinite"/>
  </rect>
  <rect x="0" y="100" width="900" height="4" fill="#00e5ff" opacity="0.3">
    <animate attributeName="y" values="100;60;110;40;100" dur="2s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.3;0;0.2;0;0.3" dur="2s" repeatCount="indefinite"/>
  </rect>

  <!-- flicker overlay -->
  <rect width="900" height="160" fill="#000000">
    <animate attributeName="opacity" values="0;0;0.15;0;0;0.1;0" dur="2.5s" repeatCount="indefinite"/>
  </rect>
</svg>
