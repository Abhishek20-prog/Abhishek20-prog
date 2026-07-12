<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1180 610" width="100%" height="100%">
  <defs>
    <style>
      @text { font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace; }
      .sans { font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif; }
      .bold { font-weight: 700; }
      .medium { font-weight: 500; }
      
       
      .text-primary { fill: #F8FAFC; }
      .text-muted { fill: #94A3B8; }
      
      /* Typing & Cursor Animations */
      .cursor { animation: blink 0.8s infinite; }
      @keyframes blink { 0%, 100% { opacity: 1; } 50% { opacity: 0; } }
      
      /* Micro-animations */
      .glow-pulse { animation: pulse 4s ease-in-out infinite; }
      @keyframes pulse { 0%, 100% { opacity: 0.15; } 50% { opacity: 0.3; } }
    </style>

    <radialGradient id="bg-glow-1" cx="20%" cy="30%" r="50%">
      <stop offset="0%" stop-color="#7C3AED" stop-opacity="0.25" />
      <stop offset="100%" stop-color="#030712" stop-opacity="0" />
    </radialGradient>
    <radialGradient id="bg-glow-2" cx="80%" cy="70%" r="60%">
      <stop offset="0%" stop-color="#06B6D4" stop-opacity="0.2" />
      <stop offset="100%" stop-color="#030712" stop-opacity="0" />
    </radialGradient>
    <radialGradient id="bg-glow-3" cx="50%" cy="50%" r="40%">
      <stop offset="0%" stop-color="#10B981" stop-opacity="0.1" />
      <stop offset="100%" stop-color="#030712" stop-opacity="0" />
    </radialGradient>

    <linearGradient id="accent-grad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#7C3AED" />
      <stop offset="50%" stop-color="#22D3EE" />
      <stop offset="100%" stop-color="#10B981" />
      <animateTransform attributeName="gradientTransform" type="rotate" from="0 0.5 0.5" to="360 0.5 0.5" dur="12s" repeatCount="indefinite" />
    </linearGradient>

    <linearGradient id="ascii-grad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#22D3EE" />
      <stop offset="100%" stop-color="#7C3AED" />
      <animateTransform attributeName="gradientTransform" type="translate" from="0,-0.5" to="0,0.5" dur="6s" autoreverse="true" repeatCount="indefinite" />
    </linearGradient>

    <linearGradient id="border-shimmer" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#ffffff" stop-opacity="0.03" />
      <stop offset="30%" stop-color="#ffffff" stop-opacity="0.05" />
      <stop offset="50%" stop-color="#22D3EE" stop-opacity="0.4" />
      <stop offset="70%" stop-color="#ffffff" stop-opacity="0.05" />
      <stop offset="100%" stop-color="#ffffff" stop-opacity="0.03" />
    </linearGradient>

    <filter id="blur-glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="40" result="blur" />
      <feComposite in="SourceGraphic" in2="blur" operator="over" />
    </filter>
    <filter id="subtle-shadow">
      <feDropShadow dx="0" dy="8" stdDeviation="16" flood-color="#000000" flood-opacity="0.5" />
    </filter>
    
    <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
      <path d="M 40 0 L 0 0 0 40" fill="none" stroke="#ffffff" stroke-opacity="0.015" stroke-width="1" />
    </pattern>
  </defs>

  <rect width="1180" height="610" fill="#030712" rx="24" />
  
  <rect width="1180" height="610" fill="url(#bg-glow-1)" rx="24" />
  <rect width="1180" height="610" fill="url(#bg-glow-2)" rx="24" />
  <rect width="1180" height="610" fill="url(#bg-glow-3)" rx="24" class="glow-pulse" />
  
  <rect width="1180" height="610" fill="url(#grid)" rx="24" />

  <g fill="#22D3EE" opacity="0.3">
    <circle r="1.5"><animateMotion dur="9s" repeatCount="indefinite" path="M100,500 C150,420 250,480 300,400 T500,300" /></circle>
    <circle r="1"><animateMotion dur="14s" repeatCount="indefinite" path="M900,100 C800,200 850,300 700,400 T500,500" /></circle>
    <circle r="2"><animateMotion dur="11s" repeatCount="indefinite" path="M400,150 C500,80 600,200 750,100 T1000,200" /></circle>
  </g>

  <line x1="0" y1="0" x2="1180" y2="0" stroke="#ffffff" stroke-opacity="0.02" stroke-width="2">
    <animate attributeName="y" from="0" to="610" dur="8s" repeatCount="indefinite" />
  </line>

  <g transform="translate(40, 40)" filter="url(#subtle-shadow)">
    <rect width="1100" height="530" rx="16" fill="none" stroke="url(#border-shimmer)" stroke-width="1.5" />
    <rect width="1100" height="530" rx="16" fill="#0F172A" fill-opacity="0.4" />

    <g transform="translate(20, 20)">
      <g>
        <animateTransform attributeName="transform" type="translate" values="0,0; 0,-8; 0,0" dur="6s" repeatCount="indefinite" ease-in-out="true"/>
        
        <rect width="400" height="490" rx="12" fill="#0F172A" fill-opacity="0.5" stroke="rgba(255,255,255,0.06)" stroke-width="1" />
        
        <g fill="url(#ascii-grad)" font-family="ui-monospace, monospace" font-size="11" font-weight="bold" letter-spacing="2">
          <text x="40" y="70" opacity="0"><animate attributeName="opacity" to="0.85" begin="0.1s" dur="0.4s" fill="freeze" />■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■</text>
          <text x="40" y="90" opacity="0"><animate attributeName="opacity" to="0.85" begin="0.2s" dur="0.4s" fill="freeze" />■■▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒■■</text>
          <text x="40" y="110" opacity="0"><animate attributeName="opacity" to="0.85" begin="0.3s" dur="0.4s" fill="freeze" />■▒▒                    ▒▒■</text>
          <text x="40" y="130" opacity="0"><animate attributeName="opacity" to="0.85" begin="0.4s" dur="0.4s" fill="freeze" />■▒   ■■■■■        ■■■■■   ▒■</text>
          <text x="40" y="150" opacity="0"><animate attributeName="opacity" to="0.85" begin="0.5s" dur="0.4s" fill="freeze" />■▒  ■■████■■    ■■████■■  ▒■</text>
          <text x="40" y="170" opacity="0"><animate attributeName="opacity" to="0.85" begin="0.6s" dur="0.4s" fill="freeze" />■▒ ▒███▓▓███▒  ▒███▓▓███▒ ▒■</text>
          <text x="40" y="190" opacity="0"><animate attributeName="opacity" to="0.85" begin="0.7s" dur="0.4s" fill="freeze" />■▒ ▒██▓▒▒▓██▒  ▒██▓▒▒▓██▒ ▒■</text>
          <text x="40" y="210" opacity="0"><animate attributeName="opacity" to="0.85" begin="0.8s" dur="0.4s" fill="freeze" />■▒  ■██▓▓██■    ■██▓▓██■  ▒■</text>
          <text x="40" y="230" opacity="0"><animate attributeName="opacity" to="0.85" begin="0.9s" dur="0.4s" fill="freeze" />■▒    ■■■■        ■■■■    ▒■</text>
          <text x="40" y="250" opacity="0"><animate attributeName="opacity" to="0.85" begin="1.0s" dur="0.4s" fill="freeze" />■▒          ▒▒          ▒■</text>
          <text x="40" y="270" opacity="0"><animate attributeName="opacity" to="0.85" begin="1.1s" dur="0.4s" fill="freeze" />■▒        ▒████▒        ▒■</text>
          <text x="40" y="290" opacity="0"><animate attributeName="opacity" to="0.85" begin="1.2s" dur="0.4s" fill="freeze" />■▒       ▒██████▒       ▒■</text>
          <text x="40" y="310" opacity="0"><animate attributeName="opacity" to="0.85" begin="1.3s" dur="0.4s" fill="freeze" />■▒  ▒▒  ▒██■  ■██▒  ▒▒  ▒■</text>
          <text x="40" y="330" opacity="0"><animate attributeName="opacity" to="0.85" begin="1.4s" dur="0.4s" fill="freeze" />■▒  ▒██████▒  ▒██████▒  ▒■</text>
          <text x="40" y="350" opacity="0"><animate attributeName="opacity" to="0.85" begin="1.5s" dur="0.4s" fill="freeze" />■▒   ▒████▒    ▒████▒   ▒■</text>
          <text x="40" y="370" opacity="0"><animate attributeName="opacity" to="0.85" begin="1.6s" dur="0.4s" fill="freeze" />■▒▒   ▒▒▒        ▒▒▒   ▒▒■</text>
          <text x="40" y="390" opacity="0"><animate attributeName="opacity" to="0.85" begin="1.7s" dur="0.4s" fill="freeze" />■■▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒■■</text>
          <text x="40" y="410" opacity="0"><animate attributeName="opacity" to="0.85" begin="1.8s" dur="0.4s" fill="freeze" />■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■■</text>
        </g>
        
        <g transform="translate(40, 440)">
          <circle cx="10" cy="12" r="4" fill="#10B981" />
          <text x="25" y="16" fill="#94A3B8" font-family="ui-monospace, monospace" font-size="11" letter-spacing="1">SYSTEM: ACTIVE</text>
        </g>
      </g>
    </g>

    <g transform="translate(450, 20)">
      <rect width="630" height="490" rx="12" fill="#0F172A" fill-opacity="0.7" stroke="rgba(255,255,255,0.06)" stroke-width="1" />
      
      <circle cx="25" cy="24" r="6" fill="#EF4444" opacity="0.8"/>
      <circle cx="45" cy="24" r="6" fill="#F59E0B" opacity="0.8"/>
      <circle cx="65" cy="24" r="6" fill="#10B981" opacity="0.8"/>
      <text x="315" y="28" fill="#475569" font-family="ui-monospace, monospace" font-size="11" text-anchor="middle" letter-spacing="1">abhishek@node-core:~</text>
      <line x1="0" y1="48" x2="630" y2="48" stroke="rgba(255,255,255,0.06)" stroke-width="1" />

      <g transform="translate(30, 85)" font-family="ui-monospace, SFMono-Regular, monospace">
        
        <g>
          <text x="0" y="0" fill="#94A3B8" font-size="15" class="sans">Hi 👋 I'm</text>
          <text x="85" y="2" fill="url(#accent-grad)" font-size="28" font-weight="700" class="sans">Abhishek Kumar</text>
        </g>

        <g transform="translate(0, 45)">
          <text x="0" y="0" fill="#F8FAFC" font-size="16" font-weight="600" class="sans">
            <animate attributeName="textContent" 
                     values="&gt; Full Stack Developer; &gt; Frontend Engineer; &gt; UI/UX Architect; &gt; Open Source Contributor; &gt; Full Stack Developer" 
                     dur="12s" repeatCount="indefinite" />
          </text>
          <text x="210" y="-1" fill="#22D3EE" font-size="18" class="cursor" font-weight="bold">_</text>
        </g>

        <g transform="translate(0, 95)" font-size="13" fill="#94A3B8" class="sans">
          <g opacity="0"><animate attributeName="opacity" to="1" begin="0.6s" dur="0.4s" fill="freeze"/>
            <text x="0" y="0" fill="#52525B" font-family="ui-monospace, monospace">●</text>
            <text x="20" y="0" font-weight="bold" fill="#64748B">LOCATION:</text>
            <text x="140" y="0" fill="#F8FAFC">Delhi, India</text>
          </g>
          
          <g opacity="0"><animate attributeName="opacity" to="1" begin="0.9s" dur="0.4s" fill="freeze"/>
            <text x="0" y="28" fill="#52525B" font-family="ui-monospace, monospace">●</text>
            <text x="20" y="28" font-weight="bold" fill="#64748B">EDUCATION:</text>
            <text x="140" y="28" fill="#F8FAFC">Engineering Student</text>
          </g>
          
          <g opacity="0"><animate attributeName="opacity" to="1" begin="1.2s" dur="0.4s" fill="freeze"/>
            <text x="0" y="56" fill="#52525B" font-family="ui-monospace, monospace">●</text>
            <text x="20" y="56" font-weight="bold" fill="#64748B">CURRENT FOCUS:</text>
            <text x="140" y="56" fill="#22D3EE" font-weight="600">Advanced Systems, Web Dev &amp; Physics</text>
          </g>
          
          <g opacity="0"><animate attributeName="opacity" to="1" begin="1.5s" dur="0.4s" fill="freeze"/>
            <text x="0" y="84" fill="#52525B" font-family="ui-monospace, monospace">●</text>
            <text x="20" y="84" font-weight="bold" fill="#64748B">EMAIL:</text>
            <text x="140" y="84" fill="#F8FAFC">abhishek@example.com</text>
          </g>
        </g>

        <g transform="translate(0, 230)" opacity="0">
          <animate attributeName="opacity" to="1" begin="1.8s" dur="0.5s" fill="freeze"/>
          <text x="0" y="0" fill="#64748B" font-size="11" font-weight="bold" letter-spacing="1.5">STACK MATRIX</text>
          
          <g transform="translate(0, 15)">
            <g transform="translate(0,0)">
              <rect width="78" height="28" rx="6" fill="#1E293B" stroke="rgba(34,211,238,0.2)" stroke-width="1"/>
              <text x="39" y="18" fill="#F8FAFC" font-size="12" font-weight="bold" text-anchor="middle" class="sans">React</text>
            </g>
            <g transform="translate(90,0)">
              <rect width="120" height="28" rx="6" fill="#1E293B" stroke="rgba(255,255,255,0.05)" stroke-width="1"/>
              <text x="60" y="18" fill="#F8FAFC" font-size="12" font-weight="bold" text-anchor="middle" class="sans">Next.js</text>
            </g>
            <g transform="translate(222,0)">
              <rect width="95" height="28" rx="6" fill="#1E293B" stroke="rgba(255,255,255,0.05)" stroke-width="1"/>
              <text x="47.5" y="18" fill="#F8FAFC" font-size="12" font-weight="bold" text-anchor="middle" class="sans">Tailwind</text>
            </g>
            <g transform="translate(329,0)">
              <rect width="115" height="28" rx="6" fill="#1E293B" stroke="rgba(16,185,129,0.2)" stroke-width="1"/>
              <text x="57.5" y="18" fill="#10B981" font-size="12" font-weight="bold" text-anchor="middle" class="sans">TypeScript</text>
            </g>
            <g transform="translate(456,0)">
              <rect width="65" height="28" rx="6" fill="#1E293B" stroke="rgba(255,255,255,0.05)" stroke-width="1"/>
              <text x="32.5" y="18" fill="#F8FAFC" font-size="12" font-weight="bold" text-anchor="middle" class="sans">Git</text>
            </g>
          </g>
        </g>

        <g transform="translate(0, 345)" opacity="0">
          <animate attributeName="opacity" to="1" begin="2.2s" dur="0.5s" fill="freeze"/>
          <text x="0" y="0" fill="#64748B" font-size="11" font-weight="bold" letter-spacing="1.5">CONNECT VIA SECURE NODE</text>
          
          <g transform="translate(0, 15)">
            <g transform="translate(0,0)">
              <circle cx="16" cy="16" r="16" fill="#1E293B" stroke="rgba(255,255,255,0.08)" stroke-width="1"/>
              <path d="M16 6a10 10 0 0 0-3.16 19.49c.5.1.68-.22.68-.48v-1.7c-2.78.6-3.37-1.34-3.37-1.34-.46-1.16-1.11-1.47-1.11-1.47-.9-.62.07-.6.07-.6 1 .07 1.53 1.03 1.53 1.03.9 1.52 2.34 1.08 2.91.83.1-.65.35-1.09.63-1.34-2.22-.25-4.55-1.11-4.55-4.94 0-1.1.39-1.99 1.03-2.69-.1-.25-.45-1.27.1-2.64 0 0 .84-.27 2.75 1.02a9.58 9.58 0 0 1 5 0c1.91-1.3 2.75-1.02 2.75-1.02.55 1.37.2 2.39.1 2.64.64.7 1.03 1.6 1.03 2.69 0 3.84-2.34 4.68-4.57 4.93.36.31.68.92.68 1.85V25c0 .27.18.59.69.48A10 10 0 0 0 16 6z" fill="#F8FAFC" transform="translate(0,0) scale(1)"/>
            </g>
            <g transform="translate(45,0)">
              <circle cx="16" cy="16" r="16" fill="#1E293B" stroke="rgba(255,255,255,0.08)" stroke-width="1"/>
              <path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z" fill="#94A3B8" transform="translate(4,4) scale(0.67)"/>
            </g>
            <g transform="translate(90,0)">
              <circle cx="16" cy="16" r="16" fill="#1E293B" stroke="rgba(255,255,255,0.08)" stroke-width="1"/>
              <path d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z" fill="#94A3B8" transform="translate(4,4) scale(0.67)"/>
            </g>
          </g>
        </g>

      </g>
    </g>
  </g>
</svg>
