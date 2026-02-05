[index.html](https://github.com/user-attachments/files/25103408/index.html)
<!doctype html>
<html lang="es" class="h-full">
 <head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>3M3D Impresiones</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <script src="/_sdk/element_sdk.js"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&amp;family=Inter:wght@300;400;500;600;700&amp;display=swap" rel="stylesheet">
  <style>
    body {
      box-sizing: border-box;
    }
    
    .font-display {
      font-family: 'Orbitron', sans-serif;
    }
    
    .font-body {
      font-family: 'Inter', sans-serif;
    }
    
    .gradient-bg {
      background: linear-gradient(135deg, #0f172a 0%, #1e293b 50%, #0f172a 100%);
    }
    
    .glow-text {
      text-shadow: 0 0 30px rgba(59, 130, 246, 0.5), 0 0 60px rgba(59, 130, 246, 0.3);
    }
    
    .card-glow:hover {
      box-shadow: 0 0 30px rgba(59, 130, 246, 0.3), 0 4px 20px rgba(0, 0, 0, 0.3);
    }
    
    .grid-pattern {
      background-image: 
        linear-gradient(rgba(59, 130, 246, 0.1) 1px, transparent 1px),
        linear-gradient(90deg, rgba(59, 130, 246, 0.1) 1px, transparent 1px);
      background-size: 50px 50px;
    }
    
    .floating {
      animation: float 6s ease-in-out infinite;
    }
    
    @keyframes float {
      0%, 100% { transform: translateY(0px) rotate(0deg); }
      50% { transform: translateY(-20px) rotate(5deg); }
    }
    
    .pulse-glow {
      animation: pulseGlow 2s ease-in-out infinite;
    }
    
    @keyframes pulseGlow {
      0%, 100% { box-shadow: 0 0 20px rgba(34, 197, 94, 0.4); }
      50% { box-shadow: 0 0 40px rgba(34, 197, 94, 0.8); }
    }
    
    .scroll-smooth {
      scroll-behavior: smooth;
    }
  </style>
  <style>@view-transition { navigation: auto; }</style>
  <script src="/_sdk/data_sdk.js" type="text/javascript"></script>
 </head>
 <body class="h-full font-body gradient-bg text-white overflow-auto scroll-smooth">
  <div class="w-full h-full"><!-- Navigation -->
   <nav id="navbar" class="fixed top-0 left-0 right-0 z-50 backdrop-blur-md bg-slate-900/80 border-b border-blue-500/20">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
     <div class="flex justify-between items-center h-16">
      <div class="flex items-center gap-3"><img id="nav-logo" src="https://i.imgur.com/opOqCWR.png" alt="Logo" class="w-10 h-10 rounded-lg object-cover" loading="lazy" onerror="console.error('Logo failed:', this.src); this.style.display='none'"> <span id="nav-brand" class="font-display font-bold text-xl text-white">3M3D</span>
      </div>
      <div class="hidden md:flex items-center gap-8"><a href="#inicio" class="text-gray-300 hover:text-blue-400 transition-colors">Inicio</a> <a href="#servicios" class="text-gray-300 hover:text-blue-400 transition-colors">Servicios</a> <a href="#catalogo" class="text-gray-300 hover:text-blue-400 transition-colors">Catálogo</a> <a href="#galeria" class="text-gray-300 hover:text-blue-400 transition-colors">Galería</a> <a href="#contacto" class="text-gray-300 hover:text-blue-400 transition-colors">Contacto</a>
      </div><button id="mobile-menu-btn" class="md:hidden p-2 text-gray-300">
       <svg class="w-6 h-6" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
       </svg></button>
     </div>
    </div><!-- Mobile Menu -->
    <div id="mobile-menu" class="hidden md:hidden bg-slate-900/95 border-t border-blue-500/20">
     <div class="px-4 py-4 space-y-3"><a href="#inicio" class="block text-gray-300 hover:text-blue-400 transition-colors py-2">Inicio</a> <a href="#servicios" class="block text-gray-300 hover:text-blue-400 transition-colors py-2">Servicios</a> <a href="#catalogo" class="block text-gray-300 hover:text-blue-400 transition-colors py-2">Catálogo</a> <a href="#galeria" class="block text-gray-300 hover:text-blue-400 transition-colors py-2">Galería</a> <a href="#contacto" class="block text-gray-300 hover:text-blue-400 transition-colors py-2">Contacto</a>
     </div>
    </div>
   </nav><!-- Hero Section -->
   <section id="inicio" class="relative min-h-screen flex items-center justify-center grid-pattern pt-16">
    <div class="absolute inset-0 overflow-hidden">
     <div class="absolute top-20 left-10 w-72 h-72 bg-blue-500/20 rounded-full blur-3xl"></div>
     <div class="absolute bottom-20 right-10 w-96 h-96 bg-cyan-500/20 rounded-full blur-3xl"></div>
    </div>
    <div class="relative z-10 text-center px-4 max-w-5xl mx-auto">
     <div class="floating mb-8"><img id="hero-logo" src="https://i.imgur.com/opOqCWR.png" alt="Logo" class="w-32 h-32 mx-auto rounded-lg object-cover" loading="lazy" onerror="console.error('Logo failed:', this.src); this.style.display='none'">
     </div>
     <h1 id="hero-title" class="font-display font-black text-5xl md:text-7xl mb-6 glow-text bg-gradient-to-r from-blue-400 via-cyan-400 to-blue-400 bg-clip-text text-transparent">Impresión 3D de Alta Calidad</h1>
     <p id="hero-subtitle" class="text-xl md:text-2xl text-gray-300 mb-10 max-w-2xl mx-auto">Transformamos tus ideas en realidad con tecnología de punta y precisión milimétrica</p>
     <div class="flex flex-col sm:flex-row gap-4 justify-center"><a href="#contacto" class="px-8 py-4 bg-gradient-to-r from-blue-600 to-cyan-500 rounded-xl font-semibold text-lg hover:from-blue-500 hover:to-cyan-400 transition-all transform hover:scale-105 shadow-lg shadow-blue-500/30"> Solicitar Cotización </a> <a href="#catalogo" class="px-8 py-4 border-2 border-blue-500/50 rounded-xl font-semibold text-lg hover:bg-blue-500/10 transition-all"> Ver Catálogo </a>
     </div>
    </div>
    <div class="absolute bottom-10 left-1/2 transform -translate-x-1/2 animate-bounce">
     <svg class="w-8 h-8 text-blue-400" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 14l-7 7m0 0l-7-7m7 7V3" />
     </svg>
    </div>
   </section><!-- Servicios -->
   <section id="servicios" class="py-20 px-4 relative">
    <div class="max-w-6xl mx-auto">
     <div class="text-center mb-16">
      <h2 class="font-display font-bold text-4xl md:text-5xl mb-4 text-white">Nuestros Servicios</h2>
      <div class="w-24 h-1 bg-gradient-to-r from-blue-500 to-cyan-400 mx-auto rounded-full"></div>
     </div>
     <div class="grid md:grid-cols-3 gap-8">
      <div class="bg-slate-800/50 backdrop-blur-sm p-8 rounded-2xl border border-blue-500/20 card-glow transition-all duration-300 hover:-translate-y-2">
       <div class="w-16 h-16 bg-gradient-to-br from-blue-500 to-cyan-400 rounded-xl flex items-center justify-center mb-6">
        <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19.428 15.428a2 2 0 00-1.022-.547l-2.387-.477a6 6 0 00-3.86.517l-.318.158a6 6 0 01-3.86.517L6.05 15.21a2 2 0 00-1.806.547M8 4h8l-1 1v5.172a2 2 0 00.586 1.414l5 5c1.26 1.26.367 3.414-1.415 3.414H4.828c-1.782 0-2.674-2.154-1.414-3.414l5-5A2 2 0 009 10.172V5L8 4z" />
        </svg>
       </div>
       <h3 class="font-display font-bold text-2xl mb-4 text-white">Impresión 3D</h3>
       <p class="text-gray-400 leading-relaxed">Piezas en PLA, PETG y resina con alta precisión. Calidad profesional para tus proyectos.</p>
      </div>
      <div class="bg-slate-800/50 backdrop-blur-sm p-8 rounded-2xl border border-blue-500/20 card-glow transition-all duration-300 hover:-translate-y-2">
       <div class="w-16 h-16 bg-gradient-to-br from-purple-500 to-pink-400 rounded-xl flex items-center justify-center mb-6">
        <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 21a4 4 0 01-4-4V5a2 2 0 012-2h4a2 2 0 012 2v12a4 4 0 01-4 4zm0 0h12a2 2 0 002-2v-4a2 2 0 00-2-2h-2.343M11 7.343l1.657-1.657a2 2 0 012.828 0l2.829 2.829a2 2 0 010 2.828l-8.486 8.485M7 17h.01" />
        </svg>
       </div>
       <h3 class="font-display font-bold text-2xl mb-4 text-white">Diseño 3D</h3>
       <p class="text-gray-400 leading-relaxed">Modelamos tus ideas desde cero o mejoramos diseños existentes con software profesional.</p>
      </div>
      <div class="bg-slate-800/50 backdrop-blur-sm p-8 rounded-2xl border border-blue-500/20 card-glow transition-all duration-300 hover:-translate-y-2">
       <div class="w-16 h-16 bg-gradient-to-br from-orange-500 to-yellow-400 rounded-xl flex items-center justify-center mb-6">
        <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6V4m0 2a2 2 0 100 4m0-4a2 2 0 110 4m-6 8a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4m6 6v10m6-2a2 2 0 100-4m0 4a2 2 0 110-4m0 4v2m0-6V4" />
        </svg>
       </div>
       <h3 class="font-display font-bold text-2xl mb-4 text-white">Personalización</h3>
       <p class="text-gray-400 leading-relaxed">Llaveros, figuras, piezas especiales y regalos únicos personalizados para ti.</p>
      </div>
     </div>
    </div>
   </section><!-- Catálogo -->
   <section id="catalogo" class="py-20 px-4 bg-slate-900/50">
    <div class="max-w-6xl mx-auto">
     <div class="text-center mb-16">
      <h2 class="font-display font-bold text-4xl md:text-5xl mb-4 text-white">Productos Destacados</h2>
      <div class="w-24 h-1 bg-gradient-to-r from-blue-500 to-cyan-400 mx-auto rounded-full"></div>
     </div>
     <div class="grid md:grid-cols-3 gap-8">
      <div class="group bg-slate-800/50 backdrop-blur-sm rounded-2xl border border-blue-500/20 overflow-hidden card-glow transition-all duration-300 hover:-translate-y-2">
       <div class="aspect-square bg-gradient-to-br from-slate-700 to-slate-800 flex items-center justify-center relative overflow-hidden">
        <svg class="w-24 h-24 text-blue-400/50 group-hover:scale-110 transition-transform duration-300" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M12 18h.01M8 21h8a2 2 0 002-2V5a2 2 0 00-2-2H8a2 2 0 00-2 2v14a2 2 0 002 2z" />
        </svg>
        <div class="absolute inset-0 bg-gradient-to-t from-slate-900/80 to-transparent"></div>
       </div>
       <div class="p-6">
        <h3 class="font-semibold text-xl text-white mb-2">Soporte para Celular</h3>
        <p class="text-gray-400 mb-4">Diseño ergonómico y resistente</p>
        <div class="flex justify-between items-center"><span class="text-2xl font-bold text-cyan-400">$150 MXN</span> <a href="#contacto" class="px-4 py-2 bg-blue-600 rounded-lg text-sm hover:bg-blue-500 transition-colors">Pedir</a>
        </div>
       </div>
      </div>
      <div class="group bg-slate-800/50 backdrop-blur-sm rounded-2xl border border-blue-500/20 overflow-hidden card-glow transition-all duration-300 hover:-translate-y-2">
       <div class="aspect-square bg-gradient-to-br from-slate-700 to-slate-800 flex items-center justify-center relative overflow-hidden">
        <svg class="w-24 h-24 text-purple-400/50 group-hover:scale-110 transition-transform duration-300" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M14 10l-2 1m0 0l-2-1m2 1v2.5M20 7l-2 1m2-1l-2-1m2 1v2.5M14 4l-2-1-2 1M4 7l2-1M4 7l2 1M4 7v2.5M12 21l-2-1m2 1l2-1m-2 1v-2.5M6 18l-2-1v-2.5M18 18l2-1v-2.5" />
        </svg>
        <div class="absolute inset-0 bg-gradient-to-t from-slate-900/80 to-transparent"></div>
       </div>
       <div class="p-6">
        <h3 class="font-semibold text-xl text-white mb-2">Figura Decorativa</h3>
        <p class="text-gray-400 mb-4">Detalles de alta definición</p>
        <div class="flex justify-between items-center"><span class="text-2xl font-bold text-cyan-400">$300 MXN</span> <a href="#contacto" class="px-4 py-2 bg-blue-600 rounded-lg text-sm hover:bg-blue-500 transition-colors">Pedir</a>
        </div>
       </div>
      </div>
      <div class="group bg-slate-800/50 backdrop-blur-sm rounded-2xl border border-blue-500/20 overflow-hidden card-glow transition-all duration-300 hover:-translate-y-2">
       <div class="aspect-square bg-gradient-to-br from-slate-700 to-slate-800 flex items-center justify-center relative overflow-hidden">
        <svg class="w-24 h-24 text-orange-400/50 group-hover:scale-110 transition-transform duration-300" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M11 4a2 2 0 114 0v1a1 1 0 001 1h3a1 1 0 011 1v3a1 1 0 01-1 1h-1a2 2 0 100 4h1a1 1 0 011 1v3a1 1 0 01-1 1h-3a1 1 0 01-1-1v-1a2 2 0 10-4 0v1a1 1 0 01-1 1H7a1 1 0 01-1-1v-3a1 1 0 00-1-1H4a2 2 0 110-4h1a1 1 0 001-1V7a1 1 0 011-1h3a1 1 0 001-1V4z" />
        </svg>
        <div class="absolute inset-0 bg-gradient-to-t from-slate-900/80 to-transparent"></div>
       </div>
       <div class="p-6">
        <h3 class="font-semibold text-xl text-white mb-2">Pieza Personalizada</h3>
        <p class="text-gray-400 mb-4">Hecho a tu medida</p>
        <div class="flex justify-between items-center"><span class="text-2xl font-bold text-cyan-400">Cotización</span> <a href="#contacto" class="px-4 py-2 bg-blue-600 rounded-lg text-sm hover:bg-blue-500 transition-colors">Cotizar</a>
        </div>
       </div>
      </div>
     </div>
    </div>
   </section><!-- Galería -->
   <section id="galeria" class="py-20 px-4">
    <div class="max-w-6xl mx-auto">
     <div class="text-center mb-16">
      <h2 class="font-display font-bold text-4xl md:text-5xl mb-4 text-white">Galería de Trabajos</h2>
      <div class="w-24 h-1 bg-gradient-to-r from-blue-500 to-cyan-400 mx-auto rounded-full"></div>
      <p class="text-gray-400 mt-4">Algunos de nuestros proyectos destacados</p>
     </div>
     <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
      <div class="aspect-square bg-gradient-to-br from-blue-600/30 to-cyan-600/30 rounded-xl flex items-center justify-center border border-blue-500/20 hover:scale-105 transition-transform duration-300 cursor-pointer">
       <svg class="w-16 h-16 text-blue-400/60" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M4 16l4.586-4.586a2 2 0 012.828 0L16 16m-2-2l1.586-1.586a2 2 0 012.828 0L20 14m-6-6h.01M6 20h12a2 2 0 002-2V6a2 2 0 00-2-2H6a2 2 0 00-2 2v12a2 2 0 002 2z" />
       </svg>
      </div>
      <div class="aspect-square bg-gradient-to-br from-purple-600/30 to-pink-600/30 rounded-xl flex items-center justify-center border border-purple-500/20 hover:scale-105 transition-transform duration-300 cursor-pointer">
       <svg class="w-16 h-16 text-purple-400/60" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M4 16l4.586-4.586a2 2 0 012.828 0L16 16m-2-2l1.586-1.586a2 2 0 012.828 0L20 14m-6-6h.01M6 20h12a2 2 0 002-2V6a2 2 0 00-2-2H6a2 2 0 00-2 2v12a2 2 0 002 2z" />
       </svg>
      </div>
      <div class="aspect-square bg-gradient-to-br from-orange-600/30 to-yellow-600/30 rounded-xl flex items-center justify-center border border-orange-500/20 hover:scale-105 transition-transform duration-300 cursor-pointer">
       <svg class="w-16 h-16 text-orange-400/60" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M4 16l4.586-4.586a2 2 0 012.828 0L16 16m-2-2l1.586-1.586a2 2 0 012.828 0L20 14m-6-6h.01M6 20h12a2 2 0 002-2V6a2 2 0 00-2-2H6a2 2 0 00-2 2v12a2 2 0 002 2z" />
       </svg>
      </div>
      <div class="aspect-square bg-gradient-to-br from-green-600/30 to-teal-600/30 rounded-xl flex items-center justify-center border border-green-500/20 hover:scale-105 transition-transform duration-300 cursor-pointer">
       <svg class="w-16 h-16 text-green-400/60" fill="none" stroke="currentColor" viewbox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5" d="M4 16l4.586-4.586a2 2 0 012.828 0L16 16m-2-2l1.586-1.586a2 2 0 012.828 0L20 14m-6-6h.01M6 20h12a2 2 0 002-2V6a2 2 0 00-2-2H6a2 2 0 00-2 2v12a2 2 0 002 2z" />
       </svg>
      </div>
     </div>
     <p class="text-center mt-8 text-gray-500 text-sm">* Puedes reemplazar estas imágenes por fotos reales de tus impresiones</p>
    </div>
   </section><!-- Contacto -->
   <section id="contacto" class="py-20 px-4 bg-slate-900/50">
    <div class="max-w-4xl mx-auto">
     <div class="text-center mb-16">
      <h2 class="font-display font-bold text-4xl md:text-5xl mb-4 text-white">Contacto</h2>
      <div class="w-24 h-1 bg-gradient-to-r from-blue-500 to-cyan-400 mx-auto rounded-full"></div>
      <p class="text-gray-400 mt-4">¿Tienes un proyecto en mente? ¡Contáctanos!</p>
     </div>
     <form id="contact-form" class="bg-slate-800/50 backdrop-blur-sm p-8 md:p-12 rounded-2xl border border-blue-500/20">
      <div class="grid md:grid-cols-2 gap-6 mb-6">
       <div><label for="nombre" class="block text-sm font-medium text-gray-300 mb-2">Nombre</label> <input type="text" id="nombre" name="nombre" placeholder="Tu nombre" class="w-full bg-slate-700/50 border border-slate-600 rounded-xl px-4 py-3 text-white placeholder-gray-500 focus:outline-none focus:border-blue-500 focus:ring-1 focus:ring-blue-500 transition-colors">
       </div>
       <div><label for="email" class="block text-sm font-medium text-gray-300 mb-2">Correo Electrónico</label> <input type="email" id="email" name="email" placeholder="tu@correo.com" class="w-full bg-slate-700/50 border border-slate-600 rounded-xl px-4 py-3 text-white placeholder-gray-500 focus:outline-none focus:border-blue-500 focus:ring-1 focus:ring-blue-500 transition-colors">
       </div>
      </div>
      <div class="mb-6"><label for="proyecto" class="block text-sm font-medium text-gray-300 mb-2">Describe tu proyecto</label> <textarea id="proyecto" name="proyecto" rows="5" placeholder="Cuéntanos sobre tu idea o proyecto..." class="w-full bg-slate-700/50 border border-slate-600 rounded-xl px-4 py-3 text-white placeholder-gray-500 focus:outline-none focus:border-blue-500 focus:ring-1 focus:ring-blue-500 transition-colors resize-none"></textarea>
      </div><button type="submit" class="w-full py-4 bg-gradient-to-r from-blue-600 to-cyan-500 rounded-xl font-semibold text-lg hover:from-blue-500 hover:to-cyan-400 transition-all transform hover:scale-[1.02] shadow-lg shadow-blue-500/30"> Enviar Mensaje </button>
      <div id="form-message" class="hidden mt-4 p-4 rounded-xl text-center"></div>
     </form>
    </div>
   </section><!-- Footer -->
   <footer id="footer" class="py-8 px-4 border-t border-blue-500/20">
    <div class="max-w-6xl mx-auto text-center">
     <div class="flex items-center justify-center gap-3 mb-4"><img id="footer-logo" src="https://i.imgur.com/opOqCWR.png" alt="Logo" class="w-8 h-8 rounded-lg object-cover" loading="lazy" onerror="console.error('Logo failed:', this.src); this.style.display='none'"> <span id="footer-brand" class="font-display font-bold text-xl text-white">3M3D Impresiones</span>
     </div>
     <p class="text-gray-500">© 2026 3M3D Impresiones - Todos los derechos reservados</p>
    </div>
   </footer><!-- WhatsApp Button --> <a id="whatsapp-btn" href="https://wa.me/521234567890" target="_blank" rel="noopener noreferrer" class="fixed bottom-6 right-6 z-50 bg-green-500 text-white px-6 py-4 rounded-full shadow-lg flex items-center gap-3 hover:bg-green-400 transition-all transform hover:scale-105 pulse-glow">
    <svg class="w-6 h-6" fill="currentColor" viewbox="0 0 24 24"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347m-5.421 7.403h-.004a9.87 9.87 0 01-5.031-1.378l-.361-.214-3.741.982.998-3.648-.235-.374a9.86 9.86 0 01-1.51-5.26c.001-5.45 4.436-9.884 9.888-9.884 2.64 0 5.122 1.03 6.988 2.898a9.825 9.825 0 012.893 6.994c-.003 5.45-4.437 9.884-9.885 9.884m8.413-18.297A11.815 11.815 0 0012.05 0C5.495 0 .16 5.335.157 11.892c0 2.096.547 4.142 1.588 5.945L.057 24l6.305-1.654a11.882 11.882 0 005.683 1.448h.005c6.554 0 11.89-5.335 11.893-11.893a11.821 11.821 0 00-3.48-8.413z" />
    </svg><span class="font-semibold">WhatsApp</span> </a>
  </div>
  <script>
    const defaultConfig = {
      business_name: '3M3D',
      hero_title: 'Impresión 3D de Alta Calidad',
      hero_subtitle: 'Transformamos tus ideas en realidad con tecnología de punta y precisión milimétrica',
      whatsapp_number: '521234567890',
      logo_url: 'https://i.imgur.com/opOqCWR.png',
      primary_color: '#3b82f6',
      secondary_color: '#06b6d4',
      background_color: '#0f172a',
      text_color: '#ffffff',
      accent_color: '#22c55e'
    };

    let config = { ...defaultConfig };

    // Mobile menu toggle
    document.getElementById('mobile-menu-btn').addEventListener('click', () => {
      const menu = document.getElementById('mobile-menu');
      menu.classList.toggle('hidden');
    });

    // Close mobile menu when clicking a link
    document.querySelectorAll('#mobile-menu a').forEach(link => {
      link.addEventListener('click', () => {
        document.getElementById('mobile-menu').classList.add('hidden');
      });
    });

    // Form submission
    document.getElementById('contact-form').addEventListener('submit', (e) => {
      e.preventDefault();
      const messageDiv = document.getElementById('form-message');
      messageDiv.classList.remove('hidden', 'bg-red-500/20', 'text-red-400');
      messageDiv.classList.add('bg-green-500/20', 'text-green-400');
      messageDiv.textContent = '¡Mensaje enviado! Te contactaremos pronto.';
      e.target.reset();
      setTimeout(() => {
        messageDiv.classList.add('hidden');
      }, 5000);
    });

    async function onConfigChange(cfg) {
      config = { ...defaultConfig, ...cfg };
      
      // Update text content
      document.getElementById('nav-brand').textContent = config.business_name;
      document.getElementById('hero-title').textContent = config.hero_title;
      document.getElementById('hero-subtitle').textContent = config.hero_subtitle;
      document.getElementById('footer-brand').textContent = config.business_name + ' Impresiones';
      
      // Update logo images
      const navLogo = document.getElementById('nav-logo');
      const heroLogo = document.getElementById('hero-logo');
      const footerLogo = document.getElementById('footer-logo');
      
      navLogo.src = config.logo_url;
      heroLogo.src = config.logo_url;
      footerLogo.src = config.logo_url;
      
      // Update WhatsApp link
      const whatsappBtn = document.getElementById('whatsapp-btn');
      whatsappBtn.href = 'https://wa.me/' + config.whatsapp_number;
    }

    function mapToCapabilities(cfg) {
      return {
        recolorables: [
          {
            get: () => cfg.background_color || defaultConfig.background_color,
            set: (value) => {
              cfg.background_color = value;
              if (window.elementSdk) {
                window.elementSdk.setConfig({ background_color: value });
              }
            }
          },
          {
            get: () => cfg.primary_color || defaultConfig.primary_color,
            set: (value) => {
              cfg.primary_color = value;
              if (window.elementSdk) {
                window.elementSdk.setConfig({ primary_color: value });
              }
            }
          },
          {
            get: () => cfg.text_color || defaultConfig.text_color,
            set: (value) => {
              cfg.text_color = value;
              if (window.elementSdk) {
                window.elementSdk.setConfig({ text_color: value });
              }
            }
          },
          {
            get: () => cfg.accent_color || defaultConfig.accent_color,
            set: (value) => {
              cfg.accent_color = value;
              if (window.elementSdk) {
                window.elementSdk.setConfig({ accent_color: value });
              }
            }
          }
        ],
        borderables: [],
        fontEditable: undefined,
        fontSizeable: undefined
      };
    }

    function mapToEditPanelValues(cfg) {
      return new Map([
        ['business_name', cfg.business_name || defaultConfig.business_name],
        ['hero_title', cfg.hero_title || defaultConfig.hero_title],
        ['hero_subtitle', cfg.hero_subtitle || defaultConfig.hero_subtitle],
        ['whatsapp_number', cfg.whatsapp_number || defaultConfig.whatsapp_number],
        ['logo_url', cfg.logo_url || defaultConfig.logo_url]
      ]);
    }

    // Initialize SDK
    if (window.elementSdk) {
      window.elementSdk.init({
        defaultConfig,
        onConfigChange,
        mapToCapabilities,
        mapToEditPanelValues
      });
    } else {
      onConfigChange(defaultConfig);
    }
  </script>
 <script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'9c8a8a7577654778',t:'MTc3MDIxMjAxNy4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
