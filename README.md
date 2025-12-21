<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600">
  <defs>
    <!-- Gradients -->
    <linearGradient id="skyGradient" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#0f172a;stop-opacity:1" />
      <stop offset="50%" style="stop-color:#1e293b;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#334155;stop-opacity:1" />
    </linearGradient>
    
    <linearGradient id="snowGradient" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" style="stop-color:#f1f5f9;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#cbd5e1;stop-opacity:1" />
    </linearGradient>
    
    <radialGradient id="moonGradient" cx="40%" cy="40%">
      <stop offset="0%" style="stop-color:#fef3c7;stop-opacity:1" />
      <stop offset="60%" style="stop-color:#fde68a;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#fbbf24;stop-opacity:1" />
    </radialGradient>
    
    <linearGradient id="aurora1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#10b981;stop-opacity:0"/>
      <stop offset="20%" style="stop-color:#34d399;stop-opacity:0.6"/>
      <stop offset="40%" style="stop-color:#6ee7b7;stop-opacity:0.8"/>
      <stop offset="60%" style="stop-color:#34d399;stop-opacity:0.6"/>
      <stop offset="80%" style="stop-color:#10b981;stop-opacity:0.4"/>
      <stop offset="100%" style="stop-color:#10b981;stop-opacity:0"/>
    </linearGradient>
    
    <linearGradient id="aurora2" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#8b5cf6;stop-opacity:0"/>
      <stop offset="20%" style="stop-color:#a78bfa;stop-opacity:0.5"/>
      <stop offset="40%" style="stop-color:#c4b5fd;stop-opacity:0.7"/>
      <stop offset="60%" style="stop-color:#a78bfa;stop-opacity:0.5"/>
      <stop offset="80%" style="stop-color:#8b5cf6;stop-opacity:0.3"/>
      <stop offset="100%" style="stop-color:#8b5cf6;stop-opacity:0"/>
    </linearGradient>
    
    <linearGradient id="aurora3" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#06b6d4;stop-opacity:0"/>
      <stop offset="30%" style="stop-color:#22d3ee;stop-opacity:0.4"/>
      <stop offset="50%" style="stop-color:#67e8f9;stop-opacity:0.6"/>
      <stop offset="70%" style="stop-color:#22d3ee;stop-opacity:0.4"/>
      <stop offset="100%" style="stop-color:#06b6d4;stop-opacity:0"/>
    </linearGradient>
    
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    
    <filter id="softGlow">
      <feGaussianBlur stdDeviation="5" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
  </defs>
  
  <!-- Night sky background -->
  <rect width="1200" height="600" fill="url(#skyGradient)"/>
  
  <!-- Stars -->
  <circle cx="100" cy="80" r="1.5" fill="#ffffff">
    <animate attributeName="opacity" values="0.3;1;0.3" dur="3s" repeatCount="indefinite"/>
  </circle>
  <circle cx="250" cy="120" r="1" fill="#ffffff">
    <animate attributeName="opacity" values="0.5;1;0.5" dur="4s" repeatCount="indefinite"/>
  </circle>
  <circle cx="400" cy="90" r="2" fill="#ffffff">
    <animate attributeName="opacity" values="0.4;1;0.4" dur="3.5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="550" cy="110" r="1.5" fill="#ffffff">
    <animate attributeName="opacity" values="0.6;1;0.6" dur="2.8s" repeatCount="indefinite"/>
  </circle>
  <circle cx="700" cy="70" r="1" fill="#ffffff">
    <animate attributeName="opacity" values="0.3;1;0.3" dur="4.2s" repeatCount="indefinite"/>
  </circle>
  <circle cx="850" cy="100" r="2" fill="#ffffff">
    <animate attributeName="opacity" values="0.5;1;0.5" dur="3.3s" repeatCount="indefinite"/>
  </circle>
  <circle cx="1000" cy="85" r="1.5" fill="#ffffff">
    <animate attributeName="opacity" values="0.4;1;0.4" dur="3.8s" repeatCount="indefinite"/>
  </circle>
  <circle cx="1100" cy="95" r="1" fill="#ffffff">
    <animate attributeName="opacity" values="0.6;1;0.6" dur="2.5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="180" cy="150" r="1" fill="#ffffff">
    <animate attributeName="opacity" values="0.5;1;0.5" dur="3.6s" repeatCount="indefinite"/>
  </circle>
  <circle cx="920" cy="130" r="1.5" fill="#ffffff">
    <animate attributeName="opacity" values="0.4;1;0.4" dur="3.2s" repeatCount="indefinite"/>
  </circle>
  
  <!-- Sparkle stars -->
  <g transform="translate(320, 60)">
    <path d="M 0,-4 L 0.5,-1 L 4,0 L 0.5,1 L 0,4 L -0.5,1 L -4,0 L -0.5,-1 Z" fill="#fef3c7" filter="url(#glow)">
      <animateTransform attributeName="transform" type="rotate" values="0;360" dur="15s" repeatCount="indefinite" additive="sum"/>
      <animate attributeName="opacity" values="0.6;1;0.6" dur="2.5s" repeatCount="indefinite"/>
    </path>
  </g>
  <g transform="translate(800, 110)">
    <path d="M 0,-3.5 L 0.5,-0.9 L 3.5,0 L 0.5,0.9 L 0,3.5 L -0.5,0.9 L -3.5,0 L -0.5,-0.9 Z" fill="#fef3c7" filter="url(#glow)">
      <animateTransform attributeName="transform" type="rotate" values="0;360" dur="18s" repeatCount="indefinite" additive="sum"/>
      <animate attributeName="opacity" values="0.4;1;0.4" dur="3s" repeatCount="indefinite"/>
    </path>
  </g>
  
  <!-- Full Moon -->
  <circle cx="1000" cy="120" r="60" fill="url(#moonGradient)" filter="url(#softGlow)">
    <animate attributeName="opacity" values="0.9;1;0.9" dur="5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="985" cy="110" r="12" fill="#f59e0b" opacity="0.3"/>
  <circle cx="1010" cy="135" r="8" fill="#f59e0b" opacity="0.3"/>
  <circle cx="995" cy="125" r="6" fill="#f59e0b" opacity="0.25"/>
  
  <!-- Northern Lights / Aurora Borealis -->
  <g opacity="0.7">
    <!-- First aurora wave -->
    <path d="M 0,180 Q 200,150 400,170 T 800,160 T 1200,180" 
          fill="url(#aurora1)" filter="url(#softGlow)">
      <animate attributeName="d" 
               values="M 0,180 Q 200,150 400,170 T 800,160 T 1200,180;
                       M 0,170 Q 200,140 400,160 T 800,150 T 1200,170;
                       M 0,180 Q 200,150 400,170 T 800,160 T 1200,180"
               dur="8s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.6;0.8;0.6" dur="6s" repeatCount="indefinite"/>
    </path>
    
    <!-- Second aurora wave -->
    <path d="M 0,220 Q 300,190 600,210 T 1200,220" 
          fill="url(#aurora2)" filter="url(#softGlow)">
      <animate attributeName="d" 
               values="M 0,220 Q 300,190 600,210 T 1200,220;
                       M 0,210 Q 300,180 600,200 T 1200,210;
                       M 0,220 Q 300,190 600,210 T 1200,220"
               dur="10s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.5;0.7;0.5" dur="7s" repeatCount="indefinite"/>
    </path>
    
    <!-- Third aurora wave -->
    <path d="M 0,200 Q 250,170 500,190 T 1000,180 T 1200,200" 
          fill="url(#aurora3)" filter="url(#softGlow)">
      <animate attributeName="d" 
               values="M 0,200 Q 250,170 500,190 T 1000,180 T 1200,200;
                       M 0,190 Q 250,160 500,180 T 1000,170 T 1200,190;
                       M 0,200 Q 250,170 500,190 T 1000,180 T 1200,200"
               dur="12s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0.4;0.6;0.4" dur="8s" repeatCount="indefinite"/>
    </path>
    
    <!-- Aurora curtain effects -->
    <rect x="200" y="150" width="3" height="100" fill="#34d399" opacity="0.3">
      <animate attributeName="opacity" values="0.2;0.4;0.2" dur="3s" repeatCount="indefinite"/>
      <animate attributeName="height" values="100;120;100" dur="4s" repeatCount="indefinite"/>
    </rect>
    <rect x="450" y="160" width="3" height="90" fill="#a78bfa" opacity="0.3">
      <animate attributeName="opacity" values="0.2;0.4;0.2" dur="3.5s" repeatCount="indefinite"/>
      <animate attributeName="height" values="90;110;90" dur="4.5s" repeatCount="indefinite"/>
    </rect>
    <rect x="700" y="155" width="3" height="95" fill="#22d3ee" opacity="0.3">
      <animate attributeName="opacity" values="0.2;0.4;0.2" dur="3.2s" repeatCount="indefinite"/>
      <animate attributeName="height" values="95;115;95" dur="4.2s" repeatCount="indefinite"/>
    </rect>
    <rect x="950" y="165" width="3" height="85" fill="#6ee7b7" opacity="0.3">
      <animate attributeName="opacity" values="0.2;0.4;0.2" dur="3.8s" repeatCount="indefinite"/>
      <animate attributeName="height" values="85;105;85" dur="4.8s" repeatCount="indefinite"/>
    </rect>
  </g>
  
  <!-- Snow-covered ground with hills -->
  <path d="M 0,450 Q 200,430 400,450 T 800,445 T 1200,450 L 1200,600 L 0,600 Z" 
        fill="url(#snowGradient)"/>
  
  <!-- Snow texture details -->
  <ellipse cx="150" cy="465" rx="80" ry="15" fill="#e2e8f0" opacity="0.5"/>
  <ellipse cx="400" cy="460" rx="100" ry="20" fill="#e2e8f0" opacity="0.4"/>
  <ellipse cx="650" cy="468" rx="90" ry="18" fill="#e2e8f0" opacity="0.5"/>
  <ellipse cx="900" cy="462" rx="85" ry="16" fill="#e2e8f0" opacity="0.4"/>
  <ellipse cx="1100" cy="470" rx="95" ry="19" fill="#e2e8f0" opacity="0.5"/>
  
  <!-- Distant snow hills -->
  <path d="M 0,420 Q 300,390 600,415 T 1200,420 L 1200,600 L 0,600 Z" 
        fill="#cbd5e1" opacity="0.6"/>
  
  <!-- Tent 1 (Left) -->
  <g transform="translate(200, 480)">
    <!-- Tent body -->
    <path d="M 0,-50 L 40,0 L -40,0 Z" fill="#f97316"/>
    <path d="M 0,-50 L 40,0 L 0,0 Z" fill="#ea580c"/>
    <!-- Tent door -->
    <path d="M -8,0 L 0,-25 L 8,0 Z" fill="#7c2d12" opacity="0.6"/>
    <!-- Tent pole -->
    <line x1="0" y1="-50" x2="0" y2="0" stroke="#78350f" stroke-width="2"/>
    <!-- Tent glow from inside -->
    <circle cx="0" cy="-15" r="8" fill="#fbbf24" opacity="0.4">
      <animate attributeName="opacity" values="0.3;0.5;0.3" dur="4s" repeatCount="indefinite"/>
    </circle>
  </g>
  
  <!-- Tent 2 (Center) -->
  <g transform="translate(500, 490)">
    <path d="M 0,-45 L 35,0 L -35,0 Z" fill="#0ea5e9"/>
    <path d="M 0,-45 L 35,0 L 0,0 Z" fill="#0284c7"/>
    <path d="M -6,0 L 0,-22 L 6,0 Z" fill="#075985" opacity="0.6"/>
    <line x1="0" y1="-45" x2="0" y2="0" stroke="#0c4a6e" stroke-width="2"/>
    <circle cx="0" cy="-13" r="7" fill="#fbbf24" opacity="0.4">
      <animate attributeName="opacity" values="0.3;0.5;0.3" dur="3.5s" repeatCount="indefinite"/>
    </circle>
  </g>
  
  <!-- Tent 3 (Right) -->
  <g transform="translate(850, 485)">
    <path d="M 0,-48 L 38,0 L -38,0 Z" fill="#10b981"/>
    <path d="M 0,-48 L 38,0 L 0,0 Z" fill="#059669"/>
    <path d="M -7,0 L 0,-24 L 7,0 Z" fill="#065f46" opacity="0.6"/>
    <line x1="0" y1="-48" x2="0" y2="0" stroke="#064e3b" stroke-width="2"/>
    <circle cx="0" cy="-14" r="7.5" fill="#fbbf24" opacity="0.4">
      <animate attributeName="opacity" values="0.3;0.5;0.3" dur="4.5s" repeatCount="indefinite"/>
    </circle>
  </g>
  
  <!-- Small tent (far right) -->
  <g transform="translate(1050, 495)">
    <path d="M 0,-35 L 25,0 L -25,0 Z" fill="#8b5cf6"/>
    <path d="M 0,-35 L 25,0 L 0,0 Z" fill="#7c3aed"/>
    <path d="M -5,0 L 0,-18 L 5,0 Z" fill="#5b21b6" opacity="0.6"/>
    <circle cx="0" cy="-10" r="5" fill="#fbbf24" opacity="0.4">
      <animate attributeName="opacity" values="0.3;0.5;0.3" dur="4.2s" repeatCount="indefinite"/>
    </circle>
  </g>
  
  <!-- Polar Bear -->
  <g>
    <animateTransform attributeName="transform" type="translate"
                      values="300,520; 350,515; 400,520; 450,515; 500,520; 550,515; 600,520; 550,525; 500,520; 450,525; 400,520; 350,525; 300,520"
                      dur="40s" repeatCount="indefinite"/>
    
    <!-- Bear body -->
    <ellipse cx="0" cy="0" rx="45" ry="28" fill="#f8fafc">
      <animate attributeName="ry" values="28;30;28" dur="3s" repeatCount="indefinite"/>
    </ellipse>
    
    <!-- Bear back leg (left) -->
    <ellipse cx="-25" cy="18" rx="12" ry="20" fill="#f1f5f9"/>
    
    <!-- Bear back leg (right) -->
    <ellipse cx="25" cy="18" rx="12" ry="20" fill="#f8fafc"/>
    
    <!-- Bear front leg (left) -->
    <ellipse cx="-15" cy="20" rx="10" ry="18" fill="#f1f5f9">
      <animate attributeName="cy" values="20;22;20" dur="1.5s" repeatCount="indefinite"/>
    </ellipse>
    
    <!-- Bear front leg (right) -->
    <ellipse cx="15" cy="20" rx="10" ry="18" fill="#f8fafc">
      <animate attributeName="cy" values="20;22;20" dur="1.5s" begin="0.75s" repeatCount="indefinite"/>
    </ellipse>
    
    <!-- Bear head -->
    <circle cx="35" cy="-8" r="22" fill="#f8fafc">
      <animate attributeName="cy" values="-8;-9;-8" dur="3s" repeatCount="indefinite"/>
    </circle>
    
    <!-- Bear snout -->
    <ellipse cx="48" cy="-6" rx="10" ry="8" fill="#f1f5f9">
      <animate attributeName="cy" values="-6;-7;-6" dur="3s" repeatCount="indefinite"/>
    </ellipse>
    
    <!-- Bear nose -->
    <ellipse cx="53" cy="-5" rx="4" ry="3" fill="#1e293b">
      <animate attributeName="cy" values="-5;-6;-5" dur="3s" repeatCount="indefinite"/>
    </ellipse>
    
    <!-- Bear ear (left) -->
    <circle cx="25" cy="-22" r="8" fill="#f1f5f9">
      <animate attributeName="cy" values="-22;-23;-22" dur="3s" repeatCount="indefinite"/>
    </circle>
    
    <!-- Bear ear (right) -->
    <circle cx="42" cy="-24" r="8" fill="#f8fafc">
      <animate attributeName="cy" values="-24;-25;-24" dur="3s" repeatCount="indefinite"/>
    </circle>
    
    <!-- Bear eye -->
    <circle cx="40" cy="-12" r="2.5" fill="#1e293b">
      <animate attributeName="cy" values="-12;-13;-12" dur="3s" repeatCount="indefinite"/>
    </circle>
    
    <!-- Bear tail -->
    <circle cx="-40" cy="5" r="8" fill="#f1f5f9">
      <animate attributeName="r" values="8;9;8" dur="2s" repeatCount="indefinite"/>
    </circle>
  </g>
  
  <!-- Snowflakes falling -->
  <g opacity="0.7">
    <circle cx="100" cy="300" r="2" fill="#ffffff">
      <animate attributeName="cy" values="300;600" dur="8s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;1;1;0" dur="8s" repeatCount="indefinite"/>
    </circle>
    <circle cx="300" cy="250" r="1.5" fill="#ffffff">
      <animate attributeName="cy" values="250;600" dur="10s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;1;1;0" dur="10s" repeatCount="indefinite"/>
    </circle>
    <circle cx="500" cy="280" r="2" fill="#ffffff">
      <animate attributeName="cy" values="280;600" dur="9s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;1;1;0" dur="9s" repeatCount="indefinite"/>
    </circle>
    <circle cx="700" cy="320" r="1.5" fill="#ffffff">
      <animate attributeName="cy" values="320;600" dur="11s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;1;1;0" dur="11s" repeatCount="indefinite"/>
    </circle>
    <circle cx="900" cy="290" r="2" fill="#ffffff">
      <animate attributeName="cy" values="290;600" dur="8.5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;1;1;0" dur="8.5s" repeatCount="indefinite"/>
    </circle>
    <circle cx="1100" cy="310" r="1.5" fill="#ffffff">
      <animate attributeName="cy" values="310;600" dur="10.5s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="0;1;1;0" dur="10.5s" repeatCount="indefinite"/>
    </circle>
  </g>
  
  <!-- Welcome message -->
  <text x="600" y="560" font-family="Georgia, serif" font-size="36" font-weight="normal" 
        fill="#f8fafc" text-anchor="middle" filter="url(#glow)">
    Welcome to the Arctic ❄️
    <animate attributeName="opacity" values="0;1;1;1;0" dur="10s" repeatCount="indefinite"/>
  </text>
</svg>

# Hi, I'm Harry 👋

#### Full-Stack Developer | Transforming Vision into Scalable Solutions | Expertise in AI ( Automation, Improvement, and Innovation ), Back-end, Front-end, Database (SQL/NoSQL), Cross-functional Collaboration.

### Contact Me:
<a href="https://www.linkedin.com/in/harryji/" rel="nofollow"><img  src="https://img.shields.io/badge/Harry-blue?style=flat&logo=linkedin&labelColor=blue"></a>
<a href="mailto:jiharry@hotmail.com/" rel="nofollow"><img src="https://img.shields.io/badge/Harry-c0392b?style=flat&labelColor=c0392b&logo=gmail&logoColor=white"></a>
![anoname_lg_vwx2315w_23_in_curved_monitor_in_the_style_of_psych_d770ae27-f31b-4135-acbc-e7c84936e6f6](https://github.com/harryji168/harryji168/assets/21187699/02e4b1bc-5624-4567-adb7-444af0f84d7f)
