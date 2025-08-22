<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Schauna V. Bandekar - Art Director Portfolio</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Lato:wght@400;700&family=Playfair+Display:wght@700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <style>
        body {
            font-family: 'Lato', sans-serif;
            background-color: #0c0a18;
            background-image: radial-gradient(circle at 1px 1px, rgba(255,255,255,0.05) 1px, transparent 0);
            background-size: 20px 20px;
        }
        h1, h2, h3, h4, .font-display {
            font-family: 'Playfair Display', serif;
        }
        .glassmorphism {
            background: rgba(23, 16, 54, 0.4);
            backdrop-filter: blur(15px);
            -webkit-backdrop-filter: blur(15px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s ease;
        }
        .glassmorphism:hover {
            background: rgba(23, 16, 54, 0.6);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        .section-title {
            position: relative;
            padding-bottom: 0.75rem;
            margin-bottom: 3rem;
        }
        .section-title::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 4px;
            background: linear-gradient(90deg, #a855f7, #22d3ee);
            border-radius: 2px;
        }
        .gradient-text {
            background: -webkit-linear-gradient(45deg, #a855f7, #22d3ee);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        /* Scroll Animation */
        .reveal {
            position: relative;
            transform: translateY(100px);
            opacity: 0;
            transition: 1s all ease;
        }
        .reveal.active {
            transform: translateY(0);
            opacity: 1;
        }
    </style>
</head>
<body class="bg-gray-900 text-gray-200 leading-relaxed">

    <!-- Header -->
    <header class="bg-black/30 backdrop-blur-sm sticky top-0 z-50 border-b border-white/10">
        <nav class="container mx-auto px-6 py-4 flex justify-between items-center">
            <a href="#" class="text-2xl font-bold text-white tracking-wider font-display">SVB.</a>
            <div class="hidden md:flex space-x-8 items-center">
                <a href="#about" class="hover:text-cyan-400 transition-colors duration-300">About</a>
                <a href="#portfolio" class="hover:text-cyan-400 transition-colors duration-300">Portfolio</a>
                <a href="#skills" class="hover:text-cyan-400 transition-colors duration-300">Skills</a>
                <a href="#contact" class="hover:text-cyan-400 transition-colors duration-300">Contact</a>
            </div>
            <button id="mobile-menu-button" class="md:hidden text-white focus:outline-none">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24" xmlns="http://www.w3.org/2000/svg"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path></svg>
            </button>
        </nav>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden px-6 pb-4">
            <a href="#about" class="block py-2 hover:text-cyan-400 transition-colors duration-300">About</a>
            <a href="#portfolio" class="block py-2 hover:text-cyan-400 transition-colors duration-300">Portfolio</a>
            <a href="#skills" class="block py-2 hover:text-cyan-400 transition-colors duration-300">Skills</a>
            <a href="#contact" class="block py-2 hover:text-cyan-400 transition-colors duration-300">Contact</a>
        </div>
    </header>

    <!-- Main Content -->
    <main class="container mx-auto px-6 py-12">

        <!-- Hero Section -->
        <section id="home" class="min-h-screen flex items-center">
            <div class="grid md:grid-cols-2 gap-12 items-center">
                <div class="text-center md:text-left">
                    <p class="text-xl md:text-2xl gradient-text font-semibold mb-4 font-display">Schauna V. Bandekar</p>
                    <h1 class="text-4xl md:text-6xl font-extrabold mb-6 text-white leading-tight">
                        Art Director & Creative Visualizer
                    </h1>
                    <p class="text-gray-300 max-w-xl mx-auto md:mx-0 mb-8">
                        A visual storyteller crafting captivating and emotionally resonant sets for the screen through a passion for design, color, and narrative.
                    </p>
                    <div class="flex justify-center md:justify-start space-x-4">
                        <a href="#portfolio" class="bg-gradient-to-r from-purple-500 to-cyan-500 hover:from-purple-600 hover:to-cyan-600 text-white font-bold py-3 px-6 rounded-lg transition-all transform hover:scale-105 duration-300">
                            View Portfolio
                        </a>
                        <a href="https://www.instagram.com/schaunavbandekar/" target="_blank" rel="noopener noreferrer" class="bg-white/10 hover:bg-white/20 text-white font-bold py-3 px-6 rounded-lg transition-colors duration-300">
                            Instagram
                        </a>
                    </div>
                </div>
                <div class="flex justify-center">
                    <div class="w-80 h-96 rounded-2xl overflow-hidden shadow-2xl rotate-3 border-4 border-white/10 transform hover:rotate-0 hover:scale-105 transition-transform duration-500">
                        <!-- 
                            IMAGE INSTRUCTION: 
                            1. Save your image file in the same folder as this index.html file.
                            2. Rename the image file to something simple, like 'profile.jpg'.
                            3. Change the src="./profile.jpg" below to match your new file name.
                        -->
                        <img src="./schauna-bandekar.jpg" alt="Schauna V. Bandekar" class="w-full h-full object-cover" onerror="this.onerror=null;this.src='https://placehold.co/400x500/1e293b/94a3b8?text=Schauna+V.+Bandekar';">
                    </div>
                </div>
            </div>
        </section>

        <!-- About Section -->
        <section id="about" class="py-24 reveal">
            <h2 class="text-4xl font-bold text-center section-title text-white">About Me</h2>
            <div class="max-w-4xl mx-auto glassmorphism p-8 md:p-12 rounded-2xl">
                <h3 class="text-3xl font-bold text-white mb-4 font-display">Dear Creative Director / Hiring Manager,</h3>
                <p class="text-gray-300 mb-4 italic text-lg">
                    As a visual storyteller with a deep-rooted passion for design, color theory, and visual narrative, I’ve spent the last few years immersing myself in the art of creating captivating and emotionally resonant sets for screen.
                </p>
                <p class="text-gray-300 mb-6">
                    Working in various roles — from Assistant Art Director to Set Dresser to independently leading art direction — I’ve built a strong foundation in managing large-scale productions, understanding the visual language of brands, and collaborating across departments to bring concepts to life. Whether it’s the corporate finesse needed for Bank of Baroda and Tata, the emotional vibrance in Swami Samarth music videos, or the modern edge for Flipkart Mini Ads, I bring adaptability and visual intent to every frame.
                </p>
                 <p class="text-gray-300 font-semibold">
                    I welcome the opportunity to bring my creative vision and production experience to your team.
                </p>
            </div>
        </section>

        <!-- Portfolio Highlights Section -->
        <section id="portfolio" class="py-24 reveal">
            <h2 class="text-4xl font-bold text-center section-title text-white">Portfolio Highlights</h2>
            
            <!-- Commercials & Ads -->
            <h3 class="text-3xl font-bold gradient-text mb-8 font-display">🎥 Commercials & Ads</h3>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 mb-16">
                <!-- Project Cards for Ads -->
                <div class="glassmorphism rounded-lg p-6"><h4 class="text-xl font-bold mb-1 text-white">Bank of Baroda</h4><p class="text-gray-400 mb-4">Set Dresser</p><a href="https://www.instagram.com" target="_blank" rel="noopener noreferrer" class="font-semibold text-cyan-400 hover:underline">Watch on Instagram <i class="fas fa-arrow-right ml-1"></i></a></div>
                <div class="glassmorphism rounded-lg p-6"><h4 class="text-xl font-bold mb-1 text-white">Atlys Visa</h4><p class="text-gray-400 mb-4">Associate Art Director</p><a href="https://www.youtube.com" target="_blank" rel="noopener noreferrer" class="font-semibold text-cyan-400 hover:underline">Watch on YouTube <i class="fas fa-arrow-right ml-1"></i></a></div>
                <div class="glassmorphism rounded-lg p-6"><h4 class="text-xl font-bold mb-1 text-white">Surf Excel</h4><p class="text-gray-400 mb-4">Assistant Art Director</p><a href="https://www.youtube.com" target="_blank" rel="noopener noreferrer" class="font-semibold text-cyan-400 hover:underline">Watch on YouTube <i class="fas fa-arrow-right ml-1"></i></a></div>
                <div class="glassmorphism rounded-lg p-6"><h4 class="text-xl font-bold mb-1 text-white">Tata</h4><p class="text-gray-400 mb-4">Associate Art Director</p><a href="https://www.instagram.com" target="_blank" rel="noopener noreferrer" class="font-semibold text-cyan-400 hover:underline">Watch on Instagram <i class="fas fa-arrow-right ml-1"></i></a></div>
                <div class="glassmorphism rounded-lg p-6"><h4 class="text-xl font-bold mb-1 text-white">Flipkart Mini Ads</h4><p class="text-gray-400 mb-4">Associate Art Director</p><a href="https://www.instagram.com" target="_blank" rel="noopener noreferrer" class="font-semibold text-cyan-400 hover:underline">Watch on Instagram <i class="fas fa-arrow-right ml-1"></i></a></div>
                <div class="glassmorphism rounded-lg p-6"><h4 class="text-xl font-bold mb-1 text-white">Baskin Robbins</h4><p class="text-gray-400 mb-4">Associate Art Assistant</p><a href="https://www.instagram.com" target="_blank" rel="noopener noreferrer" class="font-semibold text-cyan-400 hover:underline">Watch on Instagram <i class="fas fa-arrow-right ml-1"></i></a></div>
            </div>

            <!-- Films & Short Films -->
            <h3 class="text-3xl font-bold gradient-text mb-8 font-display">🎬 Films & Short Films</h3>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8 mb-16">
                 <div class="glassmorphism rounded-lg overflow-hidden group"><img src="https://placehold.co/600x400/172554/94a3b8?text=Nails" alt="Nails Short Film" class="w-full h-48 object-cover transition-transform duration-300 group-hover:scale-105"><div class="p-6"><h4 class="text-xl font-bold mb-1 text-white">“Nails” – Short Film</h4><p class="text-gray-400 mb-2">Assistant Art Director</p><p class="text-sm text-gray-500 mb-4">🎞 Screened at Red Sea & Bangalore Film Festivals</p><a href="#" class="font-semibold text-cyan-400 hover:underline">Watch Trailer <i class="fas fa-arrow-right ml-1"></i></a></div></div>
                 <div class="glassmorphism rounded-lg overflow-hidden group"><img src="https://placehold.co/600x400/172554/94a3b8?text=Nakshikantha" alt="Nakshikantha Short Film" class="w-full h-48 object-cover transition-transform duration-300 group-hover:scale-105"><div class="p-6"><h4 class="text-xl font-bold mb-1 text-white">“Nakshikantha” – Short Film</h4><p class="text-gray-400 mb-4">Assistant Art Director</p<a href="https://www.youtube.com" target="_blank" rel="noopener noreferrer" class="font-semibold text-cyan-400 hover:underline">Watch on YouTube <i class="fas fa-arrow-right ml-1"></i></a></div></div>
                 <div class="glassmorphism rounded-lg overflow-hidden group"><img src="https://placehold.co/600x400/172554/94a3b8?text=Paying+Guest" alt="Paying Guest Short Film" class="w-full h-48 object-cover transition-transform duration-300 group-hover:scale-105"><div class="p-6"><h4 class="text-xl font-bold mb-1 text-white">“Paying Guest” – Short Film</h4><p class="text-gray-400 mb-4">Art Director</p><a href="https://www.instagram.com" target="_blank" rel="noopener noreferrer" class="font-semibold text-cyan-400 hover:underline">Watch on Instagram <i class="fas fa-arrow-right ml-1"></i></a></div></div>
                 <div class="glassmorphism rounded-lg overflow-hidden group"><img src="https://placehold.co/600x400/172554/94a3b8?text=Rangasthala" alt="Rangasthala Film" class="w-full h-48 object-cover transition-transform duration-300 group-hover:scale-105"><div class="p-6"><h4 class="text-xl font-bold mb-1 text-white">“Rangasthala” – Kannada Film</h4><p class="text-gray-400 mb-4">Assistant Art Director</p><a href="https://www.instagram.com" target="_blank" rel="noopener noreferrer" class="font-semibold text-cyan-400 hover:underline">Watch on Instagram <i class="fas fa-arrow-right ml-1"></i></a></div></div>
            </div>
        </section>
        
        <!-- Skills & Education Section -->
        <section id="skills" class="py-24 reveal">
             <h2 class="text-4xl font-bold text-center section-title text-white">Expertise</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-16">
                <div>
                    <h3 class="text-3xl font-bold gradient-text mb-8 font-display">Skills & Tools</h3>
                    <ul class="space-y-4 text-gray-300">
                        <li class="glassmorphism p-4 rounded-lg flex items-start"><i class="fas fa-palette mt-1 mr-4 text-cyan-400"></i><div><strong class="font-semibold text-white">Art Direction:</strong> Pre-visualization, Concept Design, Moodboards</div></li>
                        <li class="glassmorphism p-4 rounded-lg flex items-start"><i class="fas fa-couch mt-1 mr-4 text-cyan-400"></i><div><strong class="font-semibold text-white">Set Dressing & Styling:</strong> Props, Furniture, Space Planning</div></li>
                        <li class="glassmorphism p-4 rounded-lg flex items-start"><i class="fas fa-drafting-compass mt-1 mr-4 text-cyan-400"></i><div><strong class="font-semibold text-white">Production Design:</strong> Set Construction Supervision, Look & Feel</div></li>
                        <li class="glassmorphism p-4 rounded-lg flex items-start"><i class="fas fa-tools mt-1 mr-4 text-cyan-400"></i><div><strong class="font-semibold text-white">Software:</strong> Adobe Photoshop, SketchUp, AutoCAD, Canva</div></li>
                    </ul>
                </div>
                 <div>
                    <h3 class="text-3xl font-bold gradient-text mb-8 font-display">Education & Training</h3>
                    <ul class="space-y-4 text-gray-300">
                        <li class="glassmorphism p-4 rounded-lg flex items-start"><i class="fas fa-graduation-cap mt-1 mr-4 text-cyan-400"></i><div><strong class="font-semibold text-white">B.A. in Visual Communication</strong><br>XYZ University – Mumbai</div></li>
                        <li class="glassmorphism p-4 rounded-lg flex items-start"><i class="fas fa-award mt-1 mr-4 text-cyan-400"></i><div><strong class="font-semibold text-white">Certified in Production Design</strong><br>FTII Workshop – Pune</div></li>
                    </ul>
                </div>
            </div>
        </section>


        <!-- Contact Section -->
        <section id="contact" class="py-24 reveal">
            <div class="text-center max-w-2xl mx-auto">
                <h2 class="text-4xl font-bold mb-4 section-title text-white">Let's Create Together</h2>
                <p class="text-gray-400 text-lg mx-auto mb-12">
                    I'm always open to discussing new projects, creative ideas, or opportunities to be part of an engaging story. Feel free to reach out for collaborations or inquiries.
                </p>
                <div class="flex flex-col sm:flex-row justify-center items-center gap-8 mb-12 text-lg">
                    <a href="mailto:schaunabandekar@gmail.com" class="flex items-center gap-3 hover:text-cyan-400 transition-colors">
                        <i class="fas fa-envelope text-cyan-400"></i>
                        schaunabandekar@gmail.com
                    </a>
                    <span class="hidden sm:block text-gray-600">|</span>
                    <a href="tel:+919930501938" class="flex items-center gap-3 hover:text-cyan-400 transition-colors">
                        <i class="fas fa-phone text-cyan-400"></i>
                        +91 99305 01938
                    </a>
                </div>
                <a href="mailto:schaunabandekar@gmail.com" class="inline-block bg-gradient-to-r from-purple-500 to-cyan-500 hover:from-purple-600 hover:to-cyan-600 text-white font-bold py-4 px-10 rounded-lg transition-all transform hover:scale-105 duration-300 text-lg">
                    Say Hello
                </a>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="border-t border-white/10 mt-16">
        <div class="container mx-auto px-6 py-8 text-center text-gray-400">
            <div class="flex justify-center space-x-6 mb-4">
                <a href="https://www.instagram.com/schaunavbandekar/" target="_blank" rel="noopener noreferrer" class="hover:text-cyan-400 transition-colors">
                    <i class="fab fa-instagram text-2xl"></i>
                </a>
                 <a href="mailto:schaunabandekar@gmail.com" class="hover:text-cyan-400 transition-colors">
                    <i class="fas fa-envelope text-2xl"></i>
                </a>
            </div>
            <p>&copy; 2024 Schauna V. Bandekar. All Rights Reserved.</p>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        const mobileMenuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');

        mobileMenuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Close mobile menu when a link is clicked
        const mobileMenuLinks = mobileMenu.querySelectorAll('a');
        mobileMenuLinks.forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });
        
        // Scroll Reveal Animation
        function reveal() {
            var reveals = document.querySelectorAll(".reveal");
            for (var i = 0; i < reveals.length; i++) {
                var windowHeight = window.innerHeight;
                var elementTop = reveals[i].getBoundingClientRect().top;
                var elementVisible = 150;
                if (elementTop < windowHeight - elementVisible) {
                    reveals[i].classList.add("active");
                } else {
                    reveals[i].classList.remove("active");
                }
            }
        }
        window.addEventListener("scroll", reveal);
        // To check the scroll position on page load
        reveal();
    </script>

</body>
</html>
