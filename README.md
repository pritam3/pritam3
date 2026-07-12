## Hi there 👋

<!--
**pritam3/pritam3** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->


``` xml
<svg xmlns="[link removed]" viewBox="0 0 1180 610" width="100%" height="100%">
  <defs>
    <!-- Background & Noise Filters -->
    <filter id="dark-blur" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="40" />
    </filter>
    <filter id="glass-blur" x="0" y="0" width="1180" height="610">
      <feGaussianBlur stdDeviation="20" />
    </filter>
    <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="8" result="blur" />
      <feMerge>
        <feMergeNode in="blur" />
        <feMergeNode in="SourceGraphic" />
      </feMerge>
    </filter>
    
    <!-- Base Gradients -->
    <linearGradient id="bg-grad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#030712" />
      <stop offset="100%" stop-color="#0b1329" />
    </linearGradient>
    
    <linearGradient id="accent-grad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#7C3AED">
        <animate attributeName="stop-color" values="#7C3AED;#22D3EE;#10B981;#7C3AED" dur="8s" repeatCount="indefinite" />
      </stop>
      <stop offset="50%" stop-color="#22D3EE">
        <animate attributeName="stop-color" values="#22D3EE;#10B981;#7C3AED;#22D3EE" dur="8s" repeatCount="indefinite" />
      </stop>
      <stop offset="100%" stop-color="#10B981">
        <animate attributeName="stop-color" values="#10B981;#7C3AED;#22D3EE;#10B981" dur="8s" repeatCount="indefinite" />
      </stop>
    </linearGradient>

    <linearGradient id="ascii-grad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#22D3EE" />
      <stop offset="100%" stop-color="#7C3AED" />
    </linearGradient>

    <!-- Glass Panel Shimmer -->
    <linearGradient id="border-shimmer" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#ffffff" stop-opacity="0.15" />
      <stop offset="30%" stop-color="#ffffff" stop-opacity="0.02" />
      <stop offset="70%" stop-color="#ffffff" stop-opacity="0.02" />
      <stop offset="100%" stop-color="#7C3AED" stop-opacity="0.3" />
    </linearGradient>
  </defs>

  <!-- Canvas Background -->
  <rect width="1180" height="610" rx="16" fill="url(#bg-grad)" />

  <!-- Floating Radial Background Glows -->
  <circle cx="200" cy="150" r="250" fill="#7C3AED" fill-opacity="0.15" filter="url(#dark-blur)">
    <animateTransform attributeName="transform" type="translate" values="0,0; 40,-30; -20,20; 0,0" dur="12s" repeatCount="indefinite" />
  </circle>
  <circle cx="900" cy="450" r="300" fill="#22D3EE" fill-opacity="0.12" filter="url(#dark-blur)">
    <animateTransform attributeName="transform" type="translate" values="0,0; -50,40; 30,-20; 0,0" dur="15s" repeatCount="indefinite" />
  </circle>
  <circle cx="550" cy="300" r="200" fill="#10B981" fill-opacity="0.08" filter="url(#dark-blur)">
    <animateTransform attributeName="transform" type="translate" values="0,0; 20,50; -30,-30; 0,0" dur="10s" repeatCount="indefinite" />
  </circle>

  <!-- Moving Scanline Effect -->
  <line x1="0" y1="0" x2="1180" y2="0" stroke="#ffffff" stroke-opacity="0.02" stroke-width="2">
    <animate attributeName="y1" values="0;610" dur="4s" repeatCount="indefinite" />
    <animate attributeName="y2" values="0;610" dur="4s" repeatCount="indefinite" />
  </line>

  <!-- ================= LEFT SIDE: ASCII ART PORTRAIT ================= -->
  <g transform="translate(60, 60)">
    <!-- Subtle floating container for ASCII -->
    <g>
      <animateTransform attributeName="transform" type="translate" values="0,0; 0,-8; 0,0" dur="6s" repeatCount="indefinite" ease="sine" />
      
      <!-- Cyber Frame background -->
      <rect width="400" height="490" rx="12" fill="#0F172A" fill-opacity="0.3" stroke="url(#border-shimmer)" stroke-width="1" />
      
      <!-- ASCII Art Wrapper with Reveal Effect -->
      <g fill="url(#ascii-grad)" font-family="monospace" font-size="11" font-weight="bold" letter-spacing="2">
        <!-- Masked reveal mimicking line-by-line typing / scan block -->
        <text x="35" y="60">▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒</text>
        <text x="35" y="85">▒▒█▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀█▒▒</text>
        <text x="35" y="110">▒▒█  ████████  ████████  ██████  █▒▒</text>
        <text x="35" y="135">▒▒█  ██    ██  ██        ██  ██  █▒▒</text>
        <text x="35" y="160">▒▒█  ████████  ██████    ██████  █▒▒</text>
        <text x="35" y="185">▒▒█  ██    ██  ██        ██      █▒▒</text>
        <text x="35" y="210">▒▒█  ██    ██  ████████  ██      █▒▒</text>
        <text x="35" y="235">▒▒█                              █▒▒</text>
        <text x="35" y="260">▒▒█  ░░░░░░░  ░░░░░░░  ░░░░░░░   █▒▒</text>
        <text x="35" y="285">▒▒█  ░█░░░█░  ░█░░░░░  ░█░░░░░   █▒▒</text>
        <text x="35" y="310">▒▒█  ░█████░  ░████░░  ░█░░░░░   █▒▒</text>
        <text x="35" y="335">▒▒█  ░█░░░█░  ░█░░░░░  ░█░░░░░   █▒▒</text>
        <text x="35" y="360">▒▒█  ░█░░░█░  ░░░░░░░  ░░░░░░░   █▒▒</text>
        <text x="35" y="385">▒▒█                              █▒▒</text>
        <text x="35" y="410">▒▒█▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄█▒▒</text>
        <text x="35" y="435">▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒</text>

        <!-- Dynamic Typing Cover Reveal -->
        <rect x="30" y="40" width="340" height="410" fill="#0F172A">
          <animate attributeName="height" values="410; 410; 0; 0" keyTimes="0; 0.1; 0.6; 1" dur="4s" repeatCount="1" fill="freeze" />
        </rect>
      </g>
    </g>
  </g>

  <!-- ================= RIGHT SIDE: TERMINAL WINDOW ================= -->
  <g transform="translate(500, 60)">
    <!-- Main Window Glass Panel -->
    <rect width="620" height="490" rx="12" fill="#0F172A" fill-opacity="0.7" stroke="url(#border-shimmer)" stroke-width="1.5" />
    
    <!-- Window Header / Window Controls -->
    <circle cx="25" cy="24" r="6" fill="#ef4444" />
    <circle cx="45" cy="24" r="6" fill="#f59e0b" />
    <circle cx="65" cy="24" r="6" fill="#10b981" />
    <text x="310" y="28" fill="#94A3B8" font-family="monospace" font-size="13" text-anchor="middle" letter-spacing="1">developer@terminal:~</text>
    <line x1="0" y1="48" x2="620" y2="48" stroke="rgba(255,255,255,.08)" stroke-width="1" />

    <!-- Terminal Output Content -->
    <g font-family="monospace" font-size="16" fill="#F8FAFC">
      
      <!-- Greeting Sequence -->
      <g opacity="0">
        <animate attributeName="opacity" values="0;1" begin="0.5s" dur="0.3s" fill="freeze" />
        <text x="30" y="90" fill="#94A3B8">&gt; greeting.init()</text>
        <text x="30" y="120" font-size="26" font-weight="bold">Hi, I'm <tspan fill="url(#accent-grad)">Pritam Dhoke</tspan> 👋</text>
      </g>

      <!-- Animated Character-by-Character Phrases Loop -->
      <g opacity="0">
        <animate attributeName="opacity" values="0;1" begin="1.2s" dur="0.3s" fill="freeze" />
        <text x="30" y="165" fill="#94A3B8">&gt; Current Role:</text>
        
        <g font-size="20" font-weight="bold" fill="#22D3EE">
          <text x="175" y="165">
            <!-- Interchanging strings mimicking real terminal typing -->
            <tspan>Full Stack Engineer
              <animate attributeName="opacity" values="1;1;0;0;0;0;0;0" keyTimes="0;0.25;0.26;0.5;0.51;0.75;0.76;1" dur="10s" repeatCount="indefinite" />
            </tspan>
            <tspan x="175">Open Source Contributor
              <animate attributeName="opacity" values="0;0;1;1;0;0;0;0" keyTimes="0;0.25;0.26;0.5;0.51;0.75;0.76;1" dur="10s" repeatCount="indefinite" />
            </tspan>
            <tspan x="175">AI System Specialist
              <animate attributeName="opacity" values="0;0;0;0;1;1;0;0" keyTimes="0;0.25;0.26;0.5;0.51;0.75;0.76;1" dur="10s" repeatCount="indefinite" />
            </tspan>
            <tspan x="175">UI/UX Visionary
              <animate attributeName="opacity" values="0;0;0;0;0;0;1;1" keyTimes="0;0.25;0.26;0.5;0.51;0.75;0.76;1" dur="10s" repeatCount="indefinite" />
            </tspan>
          </text>
          
          <!-- Blinking Terminal Cursor -->
          <rect x="445" y="148" width="10" height="20" fill="#22D3EE">
            <animate attributeName="x" values="395;395;445;445;395;395;360;360" keyTimes="0;0.25;0.26;0.5;0.51;0.75;0.76;1" dur="10s" repeatCount="indefinite" />
            <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite" />
          </rect>
        </g>
      </g>

      <!-- Sequential Metadata Reveal Section -->
      <!-- Item 1: Location -->
      <g opacity="0">
        <animate attributeName="opacity" values="0;1" begin="2.0s" dur="0.4s" fill="freeze" />
        <text x="30" y="215" fill="#94A3B8">📍 Location:</text>
        <text x="175" y="215" fill="#F8FAFC">Asia / Calcutta</text>
      </g>
      
      <!-- Item 2: Focus -->
      <g opacity="0">
        <animate attributeName="opacity" values="0;1" begin="2.3s" dur="0.4s" fill="freeze" />
        <text x="30" y="245" fill="#94A3B8">🚀 Core Focus:</text>
        <text x="175" y="245" fill="#F8FAFC">Next-Gen Architecture &amp; Automation</text>
      </g>

      <!-- Item 3: Email -->
      <g opacity="0">
        <animate attributeName="opacity" values="0;1" begin="2.6s" dur="0.4s" fill="freeze" />
        <text x="30" y="275" fill="#94A3B8">📧 Email:</text>
        <text x="175" y="275" fill="#22D3EE" decoration="underline">pritamdhoke3@gmail.com</text>
      </g>

      <!-- ================= SKILLS PILLS ================= -->
      <g opacity="0" transform="translate(30, 315)">
        <animate attributeName="opacity" values="0;1" begin="3.2s" dur="0.5s" fill="freeze" />
        <text x="0" y="15" fill="#94A3B8" font-size="14">&gt; identity.stack()</text>
        
        <!-- Row 1 Tech Pills -->
        <g transform="translate(0, 35)">
          <!-- React -->
          <g transform="translate(0, 0)">
            <rect width="75" height="30" rx="15" fill="#0F172A" stroke="#7C3AED" stroke-opacity="0.4" stroke-width="1" />
            <text x="37" y="20" font-size="12" fill="#F8FAFC" text-anchor="middle">React</text>
          </g>
          <!-- Next.js -->
          <g transform="translate(85, 0)">
            <rect width="85" height="30" rx="15" fill="#0F172A" stroke="#22D3EE" stroke-opacity="0.4" stroke-width="1" />
            <text x="42" y="20" font-size="12" fill="#F8FAFC" text-anchor="middle">Next.js</text>
          </g>
          <!-- Node.js -->
          <g transform="translate(180, 0)">
            <rect width="85" height="30" rx="15" fill="#0F172A" stroke="#10B981" stroke-opacity="0.4" stroke-width="1" />
            <text x="42" y="20" font-size="12" fill="#F8FAFC" text-anchor="middle">Node.js</text>
          </g>
          <!-- TypeScript -->
          <g transform="translate(275, 0)">
            <rect width="100" height="30" rx="15" fill="#0F172A" stroke="#7C3AED" stroke-opacity="0.4" stroke-width="1" />
            <text x="50" y="20" font-size="12" fill="#F8FAFC" text-anchor="middle">TypeScript</text>
          </g>
          <!-- Python -->
          <g transform="translate(385, 0)">
            <rect width="80" height="30" rx="15" fill="#0F172A" stroke="#22D3EE" stroke-opacity="0.4" stroke-width="1" />
            <text x="40" y="20" font-size="12" fill="#F8FAFC" text-anchor="middle">Python</text>
          </g>
        </g>

        <!-- Row 2 Tech Pills -->
        <g transform="translate(0, 80)">
          <!-- Docker -->
          <g transform="translate(0, 0)">
            <rect width="85" height="30" rx="15" fill="#0F172A" stroke="#10B981" stroke-opacity="0.4" stroke-width="1" />
            <text x="42" y="20" font-size="12" fill="#F8FAFC" text-anchor="middle">Docker</text>
          </g>
          <!-- Postgres -->
          <g transform="translate(95, 0)">
            <rect width="95" height="30" rx="15" fill="#0F172A" stroke="#7C3AED" stroke-opacity="0.4" stroke-width="1" />
            <text x="47" y="20" font-size="12" fill="#F8FAFC" text-anchor="middle">PostgreSQL</text>
          </g>
          <!-- AWS -->
          <g transform="translate(200, 0)">
            <rect width="65" height="30" rx="15" fill="#0F172A" stroke="#22D3EE" stroke-opacity="0.4" stroke-width="1" />
            <text x="32" y="20" font-size="12" fill="#F8FAFC" text-anchor="middle">AWS</text>
          </g>
          <!-- Git -->
          <g transform="translate(275, 0)">
            <rect width="60" height="30" rx="15" fill="#0F172A" stroke="#10B981" stroke-opacity="0.4" stroke-width="1" />
            <text x="30" y="20" font-size="12" fill="#F8FAFC" text-anchor="middle">Git</text>
          </g>
          <!-- Figma -->
          <g transform="translate(345, 0)">
            <rect width="75" height="30" rx="15" fill="#0F172A" stroke="#7C3AED" stroke-opacity="0.4" stroke-width="1" />
            <text x="37" y="20" font-size="12" fill="#F8FAFC" text-anchor="middle">Figma</text>
          </g>
        </g>
      </g>

      <!-- ================= SOCIAL ICONS CONNECTIONS ================= -->
      <g opacity="0" transform="translate(30, 445)">
        <animate attributeName="opacity" values="0;1" begin="3.8s" dur="0.5s" fill="freeze" />
        
        <!-- GitHub -->
        <g transform="translate(0,0)" filter="url(#glow)">
          <circle cx="15" cy="15" r="15" fill="#1e293b" />
          <path d="M15,5 C9.5,5 5,9.5 5,15 C5,19.4 7.8,23.1 11.8,24.5 C12.3,24.6 12.5,24.3 12.5,24 C12.5,23.7 12.5,22.9 12.5,22 C9.7,22.6 9.1,20.7 9.1,20.7 C8.7,19.6 8,19.3 8,19.3 C7.1,18.7 8.1,18.7 8.1,18.7 C9.1,18.8 9.6,19.8 9.6,19.8 C10.5,21.3 11.9,20.9 12.5,20.6 C12.6,19.9 12.9,19.5 13.2,19.2 C11,19 8.6,18.1 8.6,14.3 C8.6,13.2 9,12.3 9.7,11.6 C9.6,11.3 9.2,10.3 9.8,8.9 C9.8,8.9 10.7,8.6 12.7,10 C13.5,9.8 14.4,9.7 15,9.7 C15.6,9.7 16.5,9.8 17.3,10 C19.3,8.6 20.2,8.9 20.2,8.9 C20.8,10.3 20.4,11.3 20.3,11.6 C21,12.3 21.4,13.2 21.4,14.3 C21.4,18.2 19,19 16.8,19.2 C17.2,19.5 17.5,20.2 17.5,21.2 C17.5,22.7 17.5,23.8 17.5,24 C17.5,24.3 17.7,24.6 18.2,24.5 C22.2,23.1 25,19.4 25,15 C25,9.5 20.5,5 15,5 Z" fill="#F8FAFC"/>
        </g>
        
        <!-- LinkedIn -->
        <g transform="translate(45,0)">
          <circle cx="15" cy="15" r="15" fill="#1e293b" />
          <path d="M10,10 H13 V20 H10 Z M11.5,5 A1.5,1.5 0 1 1 11.5,8 A1.5,1.5 0 1 1 11.5,5 M15,10 H18 V11.5 C18.5,10.5 19.5,9.8 21,9.8 C24,9.8 25,11.5 25,14.5 V20 H22 V15 C22,13.5 21.5,12.5 20.5,12.5 C19.5,12.5 19,13.2 19,14.5 V20 H16 Z" fill="#94A3B8"/>
        </g>

        <!-- Twitter / X -->
        <g transform="translate(90,0)">
          <circle cx="15" cy="15" r="15" fill="#1e293b" />
          <path d="M18.2,14.2 L24.5,7 H23 L17.6,13.2 L13.2,7 H8 L14.6,16.5 L8,24 H9.5 L15.2,17.5 L19.8,24 H25 L18.2,14.2 Z M16,16.6 L15.3,15.7 L10,8.2 H12.3 L16.6,14.3 L17.3,15.2 L23,23.2 H20.7 L16,16.6 Z" fill="#94A3B8"/>
        </g>
      </g>

    </g>
  </g>
</svg>

```

### 2\. light.svg

``` xml
<svg xmlns="[link removed]" viewBox="0 0 1180 610" width="100%" height="100%">
  <defs>
    <!-- Background & Blur Filters -->
    <filter id="light-blur" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="50" />
    </filter>
    <filter id="glow-soft" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="5" result="blur" />
      <feMerge>
        <feMergeNode in="blur" />
        <feMergeNode in="SourceGraphic" />
      </feMerge>
    </filter>
    
    <!-- Base Gradients -->
    <linearGradient id="bg-grad-light" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#FFFFFF" />
      <stop offset="100%" stop-color="#F1F5F9" />
    </linearGradient>
    
    <linearGradient id="accent-grad-light" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#2563EB">
        <animate attributeName="stop-color" values="#2563EB;#06B6D4;#10B981;#2563EB" dur="8s" repeatCount="indefinite" />
      </stop>
      <stop offset="50%" stop-color="#06B6D4">
        <animate attributeName="stop-color" values="#06B6D4;#10B981;#2563EB;#06B6D4" dur="8s" repeatCount="indefinite" />
      </stop>
      <stop offset="100%" stop-color="#10B981">
        <animate attributeName="stop-color" values="#10B981;#2563EB;#06B6D4;#10B981" dur="8s" repeatCount="indefinite" />
      </stop>
    </linearGradient>

    <linearGradient id="ascii-grad-light" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#2563EB" />
      <stop offset="100%" stop-color="#06B6D4" />
    </linearGradient>

    <!-- Glass Panel Border -->
    <linearGradient id="border-shimmer-light" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0F172A" stop-opacity="0.12" />
      <stop offset="100%" stop-color="#2563EB" stop-opacity="0.15" />
    </linearGradient>
  </defs>

  <!-- Canvas Background -->
  <rect width="1180" height="610" rx="16" fill="url(#bg-grad-light)" stroke="#E2E8F0" stroke-width="1" />

  <!-- Soft Dynamic Background Radials -->
  <circle cx="150" cy="150" r="280" fill="#2563EB" fill-opacity="0.04" filter="url(#light-blur)">
    <animateTransform attributeName="transform" type="translate" values="0,0; 30,-20; -10,10; 0,0" dur="14s" repeatCount="indefinite" />
  </circle>
  <circle cx="950" cy="400" r="250" fill="#06B6D4" fill-opacity="0.05" filter="url(#light-blur)">
    <animateTransform attributeName="transform" type="translate" values="0,0; -40,30; 20,-10; 0,0" dur="16s" repeatCount="indefinite" />
  </circle>

  <!-- Subtle Scanline Sweep -->
  <line x1="0" y1="0" x2="1180" y2="0" stroke="#000000" stroke-opacity="0.01" stroke-width="1.5">
    <animate attributeName="y1" values="0;610" dur="5s" repeatCount="indefinite" />
    <animate attributeName="y2" values="0;610" dur="5s" repeatCount="indefinite" />
  </line>

  <!-- ================= LEFT SIDE: ASCII ART PORTRAIT ================= -->
  <g transform="translate(60, 60)">
    <g>
      <animateTransform attributeName="transform" type="translate" values="0,0; 0,-6; 0,0" dur="6s" repeatCount="indefinite" ease="sine" />
      
      <!-- Frame Wrapper -->
      <rect width="400" height="490" rx="12" fill="#F8FAFC" fill-opacity="0.8" stroke="url(#border-shimmer-light)" stroke-width="1" />
      
      <!-- ASCII Art Grid Layer -->
      <g fill="url(#ascii-grad-light)" font-family="monospace" font-size="11" font-weight="bold" letter-spacing="2">
        <text x="35" y="60">▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒</text>
        <text x="35" y="85">▒▒█▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀▀█▒▒</text>
        <text x="35" y="110">▒▒█  ████████  ████████  ██████  █▒▒</text>
        <text x="35" y="135">▒▒█  ██    ██  ██        ██  ██  █▒▒</text>
        <text x="35" y="160">▒▒█  ████████  ██████    ██████  █▒▒</text>
        <text x="35" y="185">▒▒█  ██    ██  ██        ██      █▒▒</text>
        <text x="35" y="210">▒▒█  ██    ██  ████████  ██      █▒▒</text>
        <text x="35" y="235">▒▒█                              █▒▒</text>
        <text x="35" y="260">▒▒█  ░░░░░░░  ░░░░░░░  ░░░░░░░   █▒▒</text>
        <text x="35" y="285">▒▒█  ░█░░░█░  ░█░░░░░  ░█░░░░░   █▒▒</text>
        <text x="35" y="310">▒▒█  ░█████░  ░████░░  ░█░░░░░   █▒▒</text>
        <text x="35" y="335">▒▒█  ░█░░░█░  ░█░░░░░  ░█░░░░░   █▒▒</text>
        <text x="35" y="360">▒▒█  ░█░░░█░  ░░░░░░░  ░░░░░░░   █▒▒</text>
        <text x="35" y="385">▒▒█                              █▒▒</text>
        <text x="35" y="410">▒▒█▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄▄█▒▒</text>
        <text x="35" y="435">▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒</text>

        <!-- Sequential Type Block Uncover -->
        <rect x="30" y="40" width="340" height="410" fill="#F8FAFC">
          <animate attributeName="height" values="410; 410; 0; 0" keyTimes="0; 0.1; 0.6; 1" dur="4s" repeatCount="1" fill="freeze" />
        </rect>
      </g>
    </g>
  </g>

  <!-- ================= RIGHT SIDE: TERMINAL WINDOW ================= -->
  <g transform="translate(500, 60)">
    <!-- Main Glass Window -->
    <rect width="620" height="490" rx="12" fill="#F8FAFC" fill-opacity="0.85" stroke="url(#border-shimmer-light)" stroke-width="1.5" />
    
    <!-- Window Head Header System -->
    <circle cx="25" cy="24" r="6" fill="#ef4444" />
    <circle cx="45" cy="24" r="6" fill="#f59e0b" />
    <circle cx="65" cy="24" r="6" fill="#10b981" />
    <text x="310" y="28" fill="#475569" font-family="monospace" font-size="13" text-anchor="middle" letter-spacing="1">developer@terminal:~</text>
    <line x1="0" y1="48" x2="620" y2="48" stroke="rgba(15,23,42,.06)" stroke-width="1" />

    <!-- Text Interface Content Layer -->
    <g font-family="monospace" font-size="16" fill="#0F172A">
      
      <!-- greeting.init() output block -->
      <g opacity="0">
        <animate attributeName="opacity" values="0;1" begin="0.5s" dur="0.3s" fill="freeze" />
        <text x="30" y="90" fill="#475569">&gt; greeting.init()</text>
        <text x="30" y="120" font-size="26" font-weight="bold">Hi, I'm <tspan fill="url(#accent-grad-light)">Pritam Dhoke</tspan> 👋</text>
      </g>

      <!-- Rotating Dynamic Typing Frame Component -->
      <g opacity="0">
        <animate attributeName="opacity" values="0;1" begin="1.2s" dur="0.3s" fill="freeze" />
        <text x="30" y="165" fill="#475569">&gt; Current Role:</text>
        
        <g font-size="20" font-weight="bold" fill="#2563EB">
          <text x="175" y="165">
            <tspan>Full Stack Engineer
              <animate attributeName="opacity" values="1;1;0;0;0;0;0;0" keyTimes="0;0.25;0.26;0.5;0.51;0.75;0.76;1" dur="10s" repeatCount="indefinite" />
            </tspan>
            <tspan x="175">Open Source Contributor
              <animate attributeName="opacity" values="0;0;1;1;0;0;0;0" keyTimes="0;0.25;0.26;0.5;0.51;0.75;0.76;1" dur="10s" repeatCount="indefinite" />
            </tspan>
            <tspan x="175">AI System Specialist
              <animate attributeName="opacity" values="0;0;0;0;1;1;0;0" keyTimes="0;0.25;0.26;0.5;0.51;0.75;0.76;1" dur="10s" repeatCount="indefinite" />
            </tspan>
            <tspan x="175">UI/UX Visionary
              <animate attributeName="opacity" values="0;0;0;0;0;0;1;1" keyTimes="0;0.25;0.26;0.5;0.51;0.75;0.76;1" dur="10s" repeatCount="indefinite" />
            </tspan>
          </text>
          
          <!-- Blinking Cursor element -->
          <rect x="445" y="148" width="10" height="20" fill="#2563EB">
            <animate attributeName="x" values="395;395;445;445;395;395;360;360" keyTimes="0;0.25;0.26;0.5;0.51;0.75;0.76;1" dur="10s" repeatCount="indefinite" />
            <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite" />
          </rect>
        </g>
      </g>

      <!-- Sequential Details Line Disclosures -->
      <g opacity="0">
        <animate attributeName="opacity" values="0;1" begin="2.0s" dur="0.4s" fill="freeze" />
        <text x="30" y="215" fill="#475569">📍 Location:</text>
        <text x="175" y="215" fill="#0F172A">Asia / Calcutta</text>
      </g>
      
      <g opacity="0">
        <animate attributeName="opacity" values="0;1" begin="2.3s" dur="0.4s" fill="freeze" />
        <text x="30" y="245" fill="#475569">🚀 Core Focus:</text>
        <text x="175" y="245" fill="#0F172A">Next-Gen Architecture &amp; Automation</text>
      </g>

      <g opacity="0">
        <animate attributeName="opacity" values="0;1" begin="2.6s" dur="0.4s" fill="freeze" />
        <text x="30" y="275" fill="#475569">📧 Email:</text>
        <text x="175" y="275" fill="#2563EB" decoration="underline">pritamdhoke3@gmail.com</text>
      </g>

      <!-- ================= SKILLS MATRIX SECTION ================= -->
      <g opacity="0" transform="translate(30, 315)">
        <animate attributeName="opacity" values="0;1" begin="3.2s" dur="0.5s" fill="freeze" />
        <text x="0" y="15" fill="#475569" font-size="14">&gt; identity.stack()</text>
        
        <!-- Row 1 Pills -->
        <g transform="translate(0, 35)">
          <g transform="translate(0, 0)">
            <rect width="75" height="30" rx="15" fill="#E2E8F0" stroke="#2563EB" stroke-opacity="0.2" stroke-width="1" />
            <text x="37" y="20" font-size="12" fill="#0F172A" text-anchor="middle">React</text>
          </g>
          <g transform="translate(85, 0)">
            <rect width="85" height="30" rx="15" fill="#E2E8F0" stroke="#06B6D4" stroke-opacity="0.2" stroke-width="1" />
            <text x="42" y="20" font-size="12" fill="#0F172A" text-anchor="middle">Next.js</text>
          </g>
          <g transform="translate(180, 0)">
            <rect width="85" height="30" rx="15" fill="#E2E8F0" stroke="#10B981" stroke-opacity="0.2" stroke-width="1" />
            <text x="42" y="20" font-size="12" fill="#0F172A" text-anchor="middle">Node.js</text>
          </g>
          <g transform="translate(275, 0)">
            <rect width="100" height="30" rx="15" fill="#E2E8F0" stroke="#2563EB" stroke-opacity="0.2" stroke-width="1" />
            <text x="50" y="20" font-size="12" fill="#0F172A" text-anchor="middle">TypeScript</text>
          </g>
          <g transform="translate(385, 0)">
            <rect width="80" height="30" rx="15" fill="#E2E8F0" stroke="#06B6D4" stroke-opacity="0.2" stroke-width="1" />
            <text x="40" y="20" font-size="12" fill="#0F172A" text-anchor="middle">Python</text>
          </g>
        </g>

        <!-- Row 2 Pills -->
        <g transform="translate(0, 80)">
          <g transform="translate(0, 0)">
            <rect width="85" height="30" rx="15" fill="#E2E8F0" stroke="#10B981" stroke-opacity="0.2" stroke-width="1" />
            <text x="42" y="20" font-size="12" fill="#0F172A" text-anchor="middle">Docker</text>
          </g>
          <g transform="translate(95, 0)">
            <rect width="95" height="30" rx="15" fill="#E2E8F0" stroke="#2563EB" stroke-opacity="0.2" stroke-width="1" />
            <text x="47" y="20" font-size="12" fill="#0F172A" text-anchor="middle">PostgreSQL</text>
          </g>
          <g transform="translate(200, 0)">
            <rect width="65" height="30" rx="15" fill="#E2E8F0" stroke="#06B6D4" stroke-opacity="0.2" stroke-width="1" />
            <text x="32" y="20" font-size="12" fill="#0F172A" text-anchor="middle">AWS</text>
          </g>
          <g transform="translate(275, 0)">
            <rect width="60" height="30" rx="15" fill="#E2E8F0" stroke="#10B981" stroke-opacity="0.2" stroke-width="1" />
            <text x="30" y="20" font-size="12" fill="#0F172A" text-anchor="middle">Git</text>
          </g>
          <g transform="translate(345, 0)">
            <rect width="75" height="30" rx="15" fill="#E2E8F0" stroke="#2563EB" stroke-opacity="0.2" stroke-width="1" />
            <text x="37" y="20" font-size="12" fill="#0F172A" text-anchor="middle">Figma</text>
          </g>
        </g>
      </g>

      <!-- ================= LINK SECTIONS LINKS ================= -->
      <g opacity="0" transform="translate(30, 445)">
        <animate attributeName="opacity" values="0;1" begin="3.8s" dur="0.5s" fill="freeze" />
        
        <!-- GitHub -->
        <g transform="translate(0,0)" filter="url(#glow-soft)">
          <circle cx="15" cy="15" r="15" fill="#CBD5E1" />
          <path d="M15,5 C9.5,5 5,9.5 5,15 C5,19.4 7.8,23.1 11.8,24.5 C12.3,24.6 12.5,24.3 12.5,24 C12.5,23.7 12.5,22.9 12.5,22 C9.7,22.6 9.1,20.7 9.1,20.7 C8.7,19.6 8,19.3 8,19.3 C7.1,18.7 8.1,18.7 8.1,18.7 C9.1,18.8 9.6,19.8 9.6,19.8 C10.5,21.3 11.9,20.9 12.5,20.6 C12.6,19.9 12.9,19.5 13.2,19.2 C11,19 8.6,18.1 8.6,14.3 C8.6,13.2 9,12.3 9.7,11.6 C9.6,11.3 9.2,10.3 9.8,8.9 C9.8,8.9 10.7,8.6 12.7,10 C13.5,9.8 14.4,9.7 15,9.7 C15.6,9.7 16.5,9.8 17.3,10 C19.3,8.6 20.2,8.9 20.2,8.9 C20.8,10.3 20.4,11.3 20.3,11.6 C21,12.3 21.4,13.2 21.4,14.3 C21.4,18.2 19,19 16.8,19.2 C17.2,19.5 17.5,20.2 17.5,21.2 C17.5,22.7 17.5,23.8 17.5,24 C17.5,24.3 17.7,24.6 18.2,24.5 C22.2,23.1 25,19.4 25,15 C25,9.5 20.5,5 15,5 Z" fill="#0F172A"/>
        </g>
        
        <!-- LinkedIn -->
        <g transform="translate(45,0)">
          <circle cx="15" cy="15" r="15" fill="#CBD5E1" />
          <path d="M10,10 H13 V20 H10 Z M11.5,5 A1.5,1.5 0 1 1 11.5,8 A1.5,1.5 0 1 1 11.5,5 M15,10 H18 V11.5 C18.5,10.5 19.5,9.8 21,9.8 C24,9.8 25,11.5 25,14.5 V20 H22 V15 C22,13.5 21.5,12.5 20.5,12.5 C19.5,12.5 19,13.2 19,14.5 V20 H16 Z" fill="#475569"/>
        </g>

        <!-- Twitter / X -->
        <g transform="translate(90,0)">
          <circle cx="15" cy="15" r="15" fill="#CBD5E1" />
          <path d="M18.2,14.2 L24.5,7 H23 L17.6,13.2 L13.2,7 H8 L14.6,16.5 L8,24 H9.5 L15.2,17.5 L19.8,24 H25 L18.2,14.2 Z M16,16.6 L15.3,15.7 L10,8.2 H12.3 L16.6,14.3 L17.3,15.2 L23,23.2 H20.7 L16,16.6 Z" fill="#475569"/>
        </g>
      </g>

    </g>
  </g>
</svg>

```
