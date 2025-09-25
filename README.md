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
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
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
    <!-- Hero Section with Vanta.js Background -->
    <section id="hero" class="hero-section flex items-center justify-center w-full">
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
    <nav class="sticky top-0 bg-gray-900 bg-opacity-90 backdrop-filter backdrop-blur-lg z-50 shadow-lg w-full">
        <div class="max-w-7xl mx-auto px-6 py-4">
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
    <section id="work" class="py-20 bg-gray-800 w-full">
        <div class="max-w-7xl mx-auto px-6">
            <!-- your work content -->
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 bg-gray-900 w-full">
        <div class="max-w-7xl mx-auto px-6">
            <!-- about content -->
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-20 bg-gray-800 w-full">
        <div class="max-w-7xl mx-auto px-6">
            <!-- skills content -->
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-gray-900 w-full">
        <div class="max-w-7xl mx-auto px-6">
            <!-- contact content -->
        </div>
    </section>

    <!-- Footer -->
    <footer class="py-12 bg-gray-950 w-full">
        <div class="max-w-7xl mx-auto px-6">
            <!-- footer content -->
        </div>
    </footer>

    <script>
        // Initialize Vanta.js background
        VANTA.GLOBE({
            el: "#vanta-bg",
            mouseControls: true,
            touchControls: true,
            gyroControls: false,
            minHeight: 200.00,
            minWidth: 200.00,
            scale: 1.00,
            scaleMobile: 1.00,
            color: 0x3b82f6,
            backgroundColor: 0x111827,
            size: 0.8
        });

        // Initialize AOS animations
        AOS.init({
            duration: 800,
            easing: 'ease-in-out',
            once: true
        });

        // Initialize Feather Icons
        feather.replace();
    </script>
</body>
</html>
