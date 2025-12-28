<p align="center">
  <svg width="100%" height="200">
    <defs>
      <linearGradient id="neonGrad" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stop-color="#00f2ff" />
        <stop offset="50%" stop-color="#ff00f2" />
        <stop offset="100%" stop-color="#00ff90" />
      </linearGradient>

      <filter id="neonGlow">
        <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
        <feMerge>
          <feMergeNode in="coloredBlur"/>
          <feMergeNode in="SourceGraphic"/>
        </feMerge>
      </filter>

      <style>
        @keyframes float {
          0% { transform: translateY(0px); opacity: 1; }
          50% { transform: translateY(-10px); opacity: 0.85; }
          100% { transform: translateY(0px); opacity: 1; }
        }

        @keyframes glitch {
          0% { transform: translate(0px); }
          20% { transform: translate(-2px, 1px); }
          40% { transform: translate(2px, -1px); }
          60% { transform: translate(-1px, 2px); }
          80% { transform: translate(1px, -2px); }
          100% { transform: translate(0px); }
        }
      </style>
    </defs>

    <circle cx="15%" cy="40%" r="25" fill="url(#neonGrad)" filter="url(#neonGlow)" style="animation: float 4s ease-in-out infinite;" />
    <circle cx="85%" cy="60%" r="20" fill="url(#neonGrad)" filter="url(#neonGlow)" style="animation: float 6s ease-in-out infinite reverse;" />
    <circle cx="50%" cy="30%" r="30" fill="url(#neonGrad)" filter="url(#neonGlow)" style="animation: float 5s ease-in-out infinite;" />

    <text x="50%" y="55%" text-anchor="middle" font-size="42" font-family="Orbitron, sans-serif"
          fill="url(#neonGrad)" filter="url(#neonGlow)"
          style="animation: glitch 2.5s infinite;">
      WELCOME TO MY GITHUB
    </text>
  </svg>
</p>
