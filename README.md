<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>3D Artist & Game Animator Portfolio</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
  <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/feather-icons/dist/feather.min.js"></script>
  <script src="https://unpkg.com/feather-icons"></script>
  <script src="https://cdn.jsdelivr.net/npm/vanta@latest/dist/vanta.globe.min.js"></script>
  <style>
    .hero-section {
      height: 100vh;
      position: relative;
      overflow: hidden;
    }
    .portfolio-item {
      transition: all 0.3s ease;
    }
    .portfolio-item:hover {
      transform: translateY(-10px);
      box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1),
                  0 10px 10px -5px rgba(0, 0, 0, 0.04);
    }
    .skill-bar {
      height: 6px;
      border-radius: 3px;
    }
    .nav-link {
      position: relative;
    }
    .nav-link:after {
      content: '';
      position: absolute;
      width: 0;
      height: 2px;
      bottom: 0;
      left: 0;
      background-color: #3b82f6;
      transition: width 0.3s ease;
    }
    .nav-link:hover:after {
      width: 100%;
    }
  </style>
</head>
<body class="bg-gray-900 text-white">
  <!-- Hero Section -->
  <section id="hero" class="hero-section flex items-center justify-center">
    <div id="vanta-bg" class="absolute inset-0"></div>
    <div class="relative z-10 text-center px-4">
      <h1 class="text-5xl md:text-7xl font-bold mb-4" data-aos="fade-down">Bram Verschaeve</h1>
      <div class="text-xl md:text-2xl mb-8" data-aos="fade-up" data-aos-delay="100">
        <span class="text-blue-400">3D Generalist</span> • 
        <span class="text-purple-400">Game Animator</span> • 
        <span class="text-green-400">Designer</span>
      </div>
      <div class="flex justify-center space-x-4" data-aos="fade-up" data-aos-delay="200">
        <a href="#work" class="px-6 py-3 bg-blue-600 hover:bg-blue-700 rounded-full font-medium transition">View Work</a>
        <a href="#contact" class="px-6 py-3 bg-transparent border-2 border-white hover:bg-white hover:text-gray-900 rounded-full font-medium transition">Contact Me</a>
      </div>
    </div>
  </section>

  <!-- Navigation -->
  <nav class="sticky top-0 bg-gray-900 bg-opacity-90 backdrop-filter backdrop-blur-lg z-50 shadow-lg">
    <div class="w-full px-6 py-4 mx-auto">
      <div class="flex justify-between items-center">
        <div class="text-2xl font-bold">BV</div>
        <div class="hidden md:flex space-x-8">
          <a href="#work" class="nav-link">Work</a>
          <a href="#about" class="nav-link">About</a>
          <a href="#skills" class="nav-link">Skills</a>
          <a href="#contact" class="nav-link">Contact</a>
        </div>
        <button class="md:hidden focus:outline-none">
          <i data-feather="menu"></i>
        </button>
      </div>
    </div>
  </nav>

  <!-- Work Section -->
  <section id="work" class="py-20 bg-gray-800">
    <div class="w-full px-6 mx-auto">
      <h2 class="text-4xl font-bold mb-16 text-center" data-aos="fade-up">Featured Projects</h2>
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        <!-- Project 1 -->
        <div class="portfolio-item bg-gray-700 rounded-xl overflow-hidden" data-aos="fade-up">
          <div class="h-64 bg-gradient-to-r from-blue-500 to-purple-600 flex items-center justify-center">
            <i data-feather="box" class="w-20 h-20"></i>
          </div>
          <div class="p-6">
            <h3 class="text-2xl font-bold mb-2">Character Design</h3>
            <p class="text-gray-300 mb-4">High-poly 3D character with detailed textures and rigging for game animation.</p>
            <div class="flex space-x-2">
              <span class="px-3 py-1 bg-gray-600 rounded-full text-sm">Blender</span>
              <span class="px-3 py-1 bg-gray-600 rounded-full text-sm">ZBrush</span>
              <span class="px-3 py-1 bg-gray-600 rounded-full text-sm">Substance</span>
            </div>
          </div>
        </div>
        <!-- Project 2 -->
        <div class="portfolio-item bg-gray-700 rounded-xl overflow-hidden" data-aos="fade-up" data-aos-delay="100">
          <div class="h-64 bg-gradient-to-r from-purple-500 to-pink-600 flex items-center justify-center">
            <i data-feather="film" class="w-20 h-20"></i>
          </div>
          <div class="p-6">
            <h3 class="text-2xl font-bold mb-2">Game Animation</h3>
            <p class="text-gray-300 mb-4">Fluid combat animations for an action RPG game with motion capture integration.</p>
            <div class="flex space-x-2">
              <span class="px-3 py-1 bg-gray-600 rounded-full text-sm">Maya</span>
              <span class="px-3 py-1 bg-gray-600 rounded-full text-sm">MotionBuilder</span>
              <span class="px-3 py-1 bg-gray-600 rounded-full text-sm">Unity</span>
            </div>
          </div>
        </div>
        <!-- Project 3 -->
        <div class="portfolio-item bg-gray-700 rounded-xl overflow-hidden" data-aos="fade-up" data-aos-delay="200">
          <div class="h-64 bg-gradient-to-r from-green-500 to-teal-600 flex items-center justify-center">
            <i data-feather="layout" class="w-20 h-20"></i>
          </div>
          <div class="p-6">
            <h3 class="text-2xl font-bold mb-2">Environment Art</h3>
            <p class="text-gray-300 mb-4">Modular sci-fi environment with dynamic lighting and particle effects.</p>
            <div class="flex space-x-2">
              <span class="px-3 py-1 bg-gray-600 rounded-full text-sm">Unreal Engine</span>
              <span class="px-3 py-1 bg-gray-600 rounded-full text-sm">Substance</span>
              <span class="px-3 py-1 bg-gray-600 rounded-full text-sm">Quixel</span>
            </div>
          </div>
        </div>
      </div>
      <div class="text-center mt-12" data-aos="fade-up">
        <a href="#" class="inline-flex items-center px-6 py-3 border-2 border-white rounded-full font-medium hover:bg-white hover:text-gray-900 transition">
          View All Projects
          <i data-feather="arrow-right" class="ml-2"></i>
        </a>
      </div>
    </div>
  </section>

  <!-- About Section -->
  <section id="about" class="py-20 bg-gray-900">
    <div class="w-full px-6 mx-auto">
      <div class="flex flex-col lg:flex-row items-center">
        <div class="lg:w-1/2 mb-12 lg:mb-0" data-aos="fade-right">
          <div class="relative">
            <div class="w-64 h-64 bg-blue-500 rounded-full mx-auto lg:mx-0"></div>
            <div class="absolute -bottom-4 -right-4 bg-purple-500 w-32 h-32 rounded-full"></div>
          </div>
        </div>
        <div class="lg:w-1/2 lg:pl-12" data-aos="fade-left">
          <h2 class="text-4xl font-bold mb-6">About Me</h2>
          <p class="text-gray-300 mb-6">
            I'm a passionate 3D artist and game animator with over 5 years of experience creating immersive digital experiences. 
            My journey began with traditional art and evolved into mastering 3D modeling, animation, and game design.
          </p>
          <p class="text-gray-300 mb-8">
            I specialize in bringing characters and worlds to life through meticulous attention to detail and 
            a deep understanding of movement and storytelling in interactive media.
          </p>
          <div class="flex space-x-4">
            <a href="#" class="w-10 h-10 bg-gray-700 hover:bg-blue-600 rounded-full flex items-center justify-center transition"><i data-feather="linkedin"></i></a>
            <a href="#" class="w-10 h-10 bg-gray-700 hover:bg-purple-600 rounded-full flex items-center justify-center transition"><i data-feather="instagram"></i></a>
            <a href="#" class="w-10 h-10 bg-gray-700 hover:bg-gray-600 rounded-full flex items-center justify-center transition"><i data-feather="github"></i></a>
            <a href="#" class="w-10 h-10 bg-gray-700 hover:bg-blue-400 rounded-full flex items-center justify-center transition"><i data-feather="twitter"></i></a>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Skills Section -->
  <section id="skills" class="py-20 bg-gray-800">
    <div class="w-full px-6 mx-auto">
      <h2 class="text-4xl font-bold mb-16 text-center" data-aos="fade-up">My Skills</h2>
      <!-- skill bars (same as before)... -->
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="py-20 bg-gray-900">
    <div class="w-full px-6 mx-auto">
      <h2 class="text-4xl font-bold mb-16 text-center" data-aos="fade-up">Get In Touch</h2>
      <!-- contact info & form (same as before)... -->
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-gray-800 py-8 text-center">
    <p class="text-gray-400">&copy; 2025 Bram Verschaeve. All rights reserved.</p>
  </footer>

  <script>
    AOS.init();
    feather.replace();
    VANTA.GLOBE({
      el: "#vanta-bg",
      mouseControls: true,
      touchControls: true,
      minHeight: 200.00,
      minWidth: 200.00,
      scale: 1.00,
      scaleMobile: 1.00,
      color: 0x3b82f6,
      backgroundColor: 0x111827
    })
  </script>
</body>
</html>
