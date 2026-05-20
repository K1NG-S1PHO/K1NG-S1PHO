<svg width="100%" height="160" viewBox="0 0 1200 160" xmlns="http://www.w3.org/2000/svg">

  <defs>
    <linearGradient id="auraGradient" x1="0" y1="0" x2="1200" y2="0">
      <stop offset="0%" stop-color="#050008"/>
      <stop offset="25%" stop-color="#2a0066"/>
      <stop offset="50%" stop-color="#8a2be2"/>
      <stop offset="75%" stop-color="#2a0066"/>
      <stop offset="100%" stop-color="#050008"/>
    </linearGradient>

    <filter id="auraGlow">
      <feGaussianBlur stdDeviation="10" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>

  <!-- outer pressure field -->
  <path d="M0 80
           C150 10, 300 150, 450 80
           C600 10, 750 150, 900 80
           C1050 10, 1200 150, 1200 80"
        stroke="url(#auraGradient)"
        stroke-width="4"
        fill="none"
        filter="url(#auraGlow)">

    <animate attributeName="opacity"
             values="0.6;1;0.6"
             dur="4s"
             repeatCount="indefinite"/>
  </path>

  <!-- inner energy vein -->
  <path d="M0 95
           C150 40, 300 170, 450 95
           C600 40, 750 170, 900 95
           C1050 40, 1200 170, 1200 95"
        stroke="#8a2be2"
        stroke-width="1.5"
        opacity="0.7">

    <animate attributeName="opacity"
             values="0.3;0.9;0.3"
             dur="3s"
             repeatCount="indefinite"/>
  </path>

</svg>
