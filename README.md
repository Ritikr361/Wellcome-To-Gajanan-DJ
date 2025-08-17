<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GAJANAN SOUND & DJ - Premier Event Production</title>
    <!-- Tailwind CSS for a modern, responsive design -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Custom fonts for a unique look -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700;900&family=VT323&display=swap" rel="stylesheet">
    <!-- Font Awesome for a wide range of icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <!-- AOS (Animate On Scroll) for dynamic content loading -->
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <style>
        /* Base styling for dark theme and fonts */
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #1a1a1a; /* Dark gray background */
            color: #e2e8f0; /* Light text color */
        }
        .font-vt323 {
            font-family: 'VT323', monospace;
        }
        html {
            scroll-behavior: smooth;
        }
        /* Gradient for buttons and highlights */
        .btn-gradient {
            background-image: linear-gradient(to right, #00ffff, #ff00ff);
        }
        .btn-gradient:hover {
            background-image: linear-gradient(to right, #ff00ff, #00ffff);
        }
        .text-gradient {
            background-image: linear-gradient(to right, #ff00ff, #00ffff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        /* Custom neon-like pulsating glow */
        .pulsate-glow {
            box-shadow: 0 0 10px #00ffff, 0 0 20px #00ffff, 0 0 30px #ff00ff;
            animation: pulse-effect 2.5s infinite ease-in-out;
        }
        @keyframes pulse-effect {
            0%, 100% {
                transform: scale(1);
                box-shadow: 0 0 10px #00ffff, 0 0 20px #00ffff, 0 0 30px #ff00ff;
            }
            50% {
                transform: scale(1.02);
                box-shadow: 0 0 15px #00ffff, 0 0 25px #00ffff, 0 0 40px #ff00ff;
            }
        }
        /* Active nav link style */
        .nav-link.active {
            font-weight: 700;
            color: #ff00ff;
            text-shadow: 0 0 5px #ff00ff;
        }

        /* Splash Screen */
        #splash-screen {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: #1a1a1a;
            z-index: 1000;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            transition: opacity 0.5s ease-out;
        }
        .loader {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            border: 5px solid rgba(255, 0, 255, 0.2);
            border-top-color: #ff00ff;
            animation: spin 1s infinite linear;
        }
        @keyframes spin {
            to { transform: rotate(360deg); }
        }
        .hidden-content {
            display: none;
        }
        
    </style>
</head>
<body class="bg-[#1a1a1a] text-gray-200">

    <!-- Splash Screen -->
    <div id="splash-screen">
        <div class="loader"></div>
        <div class="text-2xl mt-8 font-vt323 text-white animate-pulse">LOADING...</div>
    </div>

    <!-- Main Content Container -->
    <div id="main-content" class="hidden-content">
        <!-- Header / Navbar -->
        <header id="navbar" class="bg-gray-950/80 backdrop-blur-lg sticky top-0 z-50 transition-all duration-300">
            <div class="container mx-auto px-6 py-4 flex justify-between items-center">
                <a href="#home" class="text-2xl font-vt323 font-bold text-white transition-colors duration-300 hover:text-[#ff00ff]">
                    GAJANAN
                </a>
                <nav class="hidden md:flex space-x-8">
                    <a href="#home" class="nav-link transition duration-300 hover:text-[#ff00ff]">HOME</a>
                    <a href="#services" class="nav-link transition duration-300 hover:text-[#ff00ff]">SERVICES</a>
                    <a href="#gallery" class="nav-link transition duration-300 hover:text-[#ff00ff]">GALLERY</a>
                    <a href="#testimonials" class="nav-link transition duration-300 hover:text-[#ff00ff]">TESTIMONIALS</a>
                    <a href="#contact" class="nav-link transition duration-300 hover:text-[#ff00ff]">CONTACT</a>
                </nav>
                <button id="mobile-menu-button" class="md:hidden text-gray-400 text-2xl">
                    <i class="fas fa-bars"></i>
                </button>
            </div>
            <!-- Mobile Menu -->
            <div id="mobile-menu" class="hidden md:hidden bg-gray-900 border-t border-gray-800">
                <a href="#home" class="nav-link block py-4 px-6 text-sm hover:bg-gray-800">HOME</a>
                <a href="#services" class="nav-link block py-4 px-6 text-sm hover:bg-gray-800">SERVICES</a>
                <a href="#gallery" class="nav-link block py-4 px-6 text-sm hover:bg-gray-800">GALLERY</a>
                <a href="#testimonials" class="nav-link block py-4 px-6 text-sm hover:bg-gray-800">TESTIMONIALS</a>
                <a href="#contact" class="nav-link block py-4 px-6 text-sm hover:bg-gray-800">CONTACT</a>
            </div>
        </header>

        <main>
            <!-- Hero Section -->
            <section id="home" class="relative h-[80vh] flex items-center justify-center text-center overflow-hidden">
                <div class="absolute inset-0 z-0">
                    <img src="https://images.unsplash.com/photo-1514525253161-7a46d19cd819?q=80&w=1974&auto=format&fit=crop" onerror="this.onerror=null;this.src='https://placehold.co/1920x1080/1a1a1a/FFFFFF?text=Live+Concert';" alt="Live DJ Concert" class="w-full h-full object-cover opacity-50">
                </div>
                <div class="relative z-10 p-6" data-aos="fade-up">
                    <h1 class="text-4xl md:text-6xl font-extrabold font-vt323 mb-4 text-white drop-shadow-lg">
                        <span class="text-gradient">FEEL THE VIBE</span>
                    </h1>
                    <p class="text-lg md:text-xl text-gray-300 mb-8">HIGH-END LIGHT & SOUND FOR UNFORGETTABLE NIGHTS</p>
                    <a href="#contact" class="inline-block px-8 py-4 rounded-full font-bold uppercase tracking-wide transition-all duration-300 btn-gradient pulsate-glow">
                        BOOK NOW
                    </a>
                </div>
            </section>

            <!-- Services Section -->
            <section id="services" class="py-20 bg-gray-950">
                <div class="container mx-auto px-6">
                    <h2 class="text-4xl md:text-5xl font-bold text-center mb-12 text-white font-vt323" data-aos="fade-down">OUR EXPERTISE</h2>
                    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8">
                        <!-- Service Card 1 -->
                        <div class="flex flex-col items-center text-center p-8 bg-gray-900 rounded-xl shadow-lg border border-transparent hover:border-blue-400 transition-all duration-300" data-aos="fade-up" data-aos-delay="100">
                            <i class="fas fa-glass-cheers text-4xl text-cyan-400 mb-4"></i>
                            <h3 class="text-xl font-bold mb-2 text-white">PRIVATE PARTIES</h3>
                            <p class="text-gray-400 text-sm">Exclusive setups for birthdays, anniversaries, and private celebrations.</p>
                        </div>
                        <!-- Service Card 2 -->
                        <div class="flex flex-col items-center text-center p-8 bg-gray-900 rounded-xl shadow-lg border border-transparent hover:border-blue-400 transition-all duration-300" data-aos="fade-up" data-aos-delay="200">
                            <i class="fas fa-headphones-alt text-4xl text-cyan-400 mb-4"></i>
                            <h3 class="text-xl font-bold mb-2 text-white">DJ NIGHTS & PUBS</h3>
                            <p class="text-gray-400 text-sm">Pulsating sound and dynamic lights for the ultimate clubbing experience.</p>
                        </div>
                        <!-- Service Card 3 -->
                        <div class="flex flex-col items-center text-center p-8 bg-gray-900 rounded-xl shadow-lg border border-transparent hover:border-blue-400 transition-all duration-300" data-aos="fade-up" data-aos-delay="300">
                            <i class="fas fa-briefcase text-4xl text-cyan-400 mb-4"></i>
                            <h3 class="text-xl font-bold mb-2 text-white">CORPORATE EVENTS</h3>
                            <p class="text-gray-400 text-sm">Professional and sleek AV solutions for launches, conferences, and galas.</p>
                        </div>
                        <!-- Service Card 4 -->
                        <div class="flex flex-col items-center text-center p-8 bg-gray-900 rounded-xl shadow-lg border border-transparent hover:border-blue-400 transition-all duration-300" data-aos="fade-up" data-aos-delay="400">
                            <i class="fas fa-microphone-alt text-4xl text-cyan-400 mb-4"></i>
                            <h3 class="text-xl font-bold mb-2 text-white">LIVE CONCERTS</h3>
                            <p class="text-gray-400 text-sm">Massive stage setups with concert-grade sound and lighting trusses.</p>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Gallery Section -->
            <section id="gallery" class="py-20 bg-[#1a1a1a]">
                <div class="container mx-auto px-6">
                    <h2 class="text-4xl md:text-5xl font-bold text-center mb-12 text-white font-vt323" data-aos="fade-down">EVENT GALLERY</h2>
                    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
                        <!-- Image 1 -->
                        <div class="group relative overflow-hidden rounded-lg shadow-xl cursor-pointer gallery-item" data-aos="zoom-in-up" data-aos-delay="100"
                            data-image="https://placehold.co/1920x1080/00ffff/ff00ff?text=Galactic+Bass"
                            data-title="गैलेक्टिक बीट्स"
                            data-description="सबसे आधुनिक साउंड सिस्टम के साथ, हम आपकी पार्टी को एक कॉस्मिक सफर पर ले जाते हैं।">
                            <img src="https://placehold.co/1920x1080/00ffff/ff00ff?text=Galactic+Bass" alt="Galactic Bass" class="w-full h-full object-cover transform group-hover:scale-110 transition duration-500">
                            <div class="absolute inset-0 bg-black bg-opacity-0 group-hover:bg-opacity-70 transition duration-500 flex items-center justify-center">
                                <h3 class="text-lg font-bold text-white opacity-0 group-hover:opacity-100 transition duration-500 p-4 text-center">गैलेक्टिक बीट्स</h3>
                            </div>
                        </div>
                        <!-- Image 2 -->
                        <div class="group relative overflow-hidden rounded-lg shadow-xl cursor-pointer gallery-item" data-aos="zoom-in-up" data-aos-delay="200"
                            data-image="https://images.unsplash.com/photo-1493674686008-ac5627252876?q=80&w=1932&auto=format&fit=crop"
                            data-title="पार्टी का जुनून"
                            data-description="एनर्जी से भरपूर भीड़ के बीच, हमारी लाइट्स और म्यूजिक मिलकर एक शानदार माहौल बनाते हैं।">
                            <img src="https://images.unsplash.com/photo-1493674686008-ac5627252876?q=80&w=1932&auto=format&fit=crop" alt="Party Crowd" class="w-full h-full object-cover transform group-hover:scale-110 transition duration-500">
                            <div class="absolute inset-0 bg-black bg-opacity-0 group-hover:bg-opacity-70 transition duration-500 flex items-center justify-center">
                                <h3 class="text-lg font-bold text-white opacity-0 group-hover:opacity-100 transition duration-500 p-4 text-center">पार्टी का जुनून</h3>
                            </div>
                        </div>
                        <!-- Image 3 -->
                        <div class="group relative overflow-hidden rounded-lg shadow-xl cursor-pointer gallery-item" data-aos="zoom-in-up" data-aos-delay="300"
                            data-image="https://images.unsplash.com/photo-1524368535928-5b5e00ddc76b?q=80&w=1770&auto=format&fit=crop"
                            data-title="साइबर नाइट"
                            data-description="लेजर और एलईडी स्क्रीन के साथ, हम आपके इवेंट को भविष्य की तरह रोशनी से भर देते हैं।">
                            <img src="https://images.unsplash.com/photo-1524368535928-5b5e00ddc76b?q=80&w=1770&auto=format&fit=crop" alt="Cyber Night" class="w-full h-full object-cover transform group-hover:scale-110 transition duration-500">
                            <div class="absolute inset-0 bg-black bg-opacity-0 group-hover:bg-opacity-70 transition duration-500 flex items-center justify-center">
                                <h3 class="text-lg font-bold text-white opacity-0 group-hover:opacity-100 transition duration-500 p-4 text-center">साइबर नाइट</h3>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Testimonials Section -->
            <section id="testimonials" class="py-20 bg-gray-950">
                <div class="container mx-auto px-6">
                    <h2 class="text-4xl md:text-5xl font-bold text-center mb-12 text-white font-vt323" data-aos="fade-down">WHAT OUR CLIENTS SAY</h2>
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                        <!-- Testimonial 1 -->
                        <div class="bg-gray-900 rounded-xl p-8 shadow-lg border border-transparent hover:border-cyan-400 transition-all duration-300" data-aos="fade-right" data-aos-delay="100">
                            <p class="italic text-gray-400 mb-4">"The sound system was incredible! They truly made our corporate event a huge success. Professional and highly recommended."</p>
                            <p class="font-bold text-white">- Rajesh Kumar</p>
                            <p class="text-sm text-cyan-400">CEO, Tech Innovators</p>
                        </div>
                        <!-- Testimonial 2 -->
                        <div class="bg-gray-900 rounded-xl p-8 shadow-lg border border-transparent hover:border-cyan-400 transition-all duration-300" data-aos="fade-right" data-aos-delay="200">
                            <p class="italic text-gray-400 mb-4">"Gajanan DJ transformed our wedding reception. The lighting and music were perfect, creating the most amazing atmosphere."</p>
                            <p class="font-bold text-white">- Priya & Sameer</p>
                            <p class="text-sm text-cyan-400">Newlyweds</p>
                        </div>
                        <!-- Testimonial 3 -->
                        <div class="bg-gray-900 rounded-xl p-8 shadow-lg border border-transparent hover:border-cyan-400 transition-all duration-300" data-aos="fade-right" data-aos-delay="300">
                            <p class="italic text-gray-400 mb-4">"The energy was unmatched! Their DJ and sound setup made our party the talk of the town. Can't wait to book them again."</p>
                            <p class="font-bold text-white">- Arjun Singh</p>
                            <p class="text-sm text-cyan-400">Party Host</p>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Contact Section -->
            <section id="contact" class="py-20 bg-[#1a1a1a]">
                <div class="container mx-auto px-6">
                    <h2 class="text-4xl md:text-5xl font-bold text-center mb-12 text-white font-vt323" data-aos="fade-down">BOOK YOUR EVENT</h2>
                    <div class="flex flex-col lg:flex-row gap-12">
                        <!-- Contact Form -->
                        <div class="w-full lg:w-1/2" data-aos="fade-right">
                            <h3 class="text-2xl font-bold mb-6 text-[#ff00ff]">GET IN TOUCH</h3>
                            <form id="contactForm" class="bg-gray-900 rounded-xl p-8 shadow-lg">
                                <div class="mb-4">
                                    <label for="name" class="block text-gray-400 text-sm font-semibold mb-2">NAME</label>
                                    <input type="text" id="name" name="name" class="w-full p-3 bg-gray-800 rounded-lg focus:outline-none focus:ring-2 focus:ring-[#ff00ff] transition-colors duration-300" required>
                                </div>
                                <div class="mb-4">
                                    <label for="email" class="block text-gray-400 text-sm font-semibold mb-2">EMAIL</label>
                                    <input type="email" id="email" name="email" class="w-full p-3 bg-gray-800 rounded-lg focus:outline-none focus:ring-2 focus:ring-[#ff00ff] transition-colors duration-300" required>
                                </div>
                                <div class="mb-4">
                                    <label for="message" class="block text-gray-400 text-sm font-semibold mb-2">EVENT DETAILS</label>
                                    <textarea id="message" name="message" rows="5" class="w-full p-3 bg-gray-800 rounded-lg focus:outline-none focus:ring-2 focus:ring-[#ff00ff] transition-colors duration-300" required></textarea>
                                </div>
                                <button type="submit" class="w-full py-3 rounded-full font-bold uppercase transition-all duration-300 btn-gradient hover:scale-105">
                                    SEND INQUIRY
                                </button>
                            </form>
                        </div>

                        <!-- Contact Information -->
                        <div class="w-full lg:w-1/2" data-aos="fade-left">
                            <h3 class="text-2xl font-bold mb-6 text-[#ff00ff]">CONTACT DETAILS</h3>
                            <div class="space-y-6">
                                <div class="flex items-start">
                                    <i class="fas fa-phone-alt text-2xl text-[#00ffff] mr-4 mt-1"></i>
                                    <div>
                                        <p class="text-lg font-semibold text-white">PHONE</p>
                                        <a href="tel:+917489600750" class="text-gray-400 hover:text-[#00ffff] transition-colors duration-300">+91 74896 00750</a>
                                    </div>
                                </div>
                                <div class="flex items-start">
                                    <i class="fas fa-envelope text-2xl text-[#00ffff] mr-4 mt-1"></i>
                                    <div>
                                        <p class="text-lg font-semibold text-white">EMAIL</p>
                                        <a href="mailto:contact@gajanansounddj.com" class="text-gray-400 hover:text-[#00ffff] transition-colors duration-300">contact@gajanansounddj.com</a>
                                    </div>
                                </div>
                                <div class="flex items-start">
                                    <i class="fas fa-map-marker-alt text-2xl text-[#00ffff] mr-4 mt-1"></i>
                                    <div>
                                        <p class="text-lg font-semibold text-white">ADDRESS</p>
                                        <p class="text-gray-400">Rajgarh Naka, Jhabua, Madhya Pradesh, India</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
        </main>

        <!-- Footer -->
        <footer class="bg-gray-950 py-10">
            <div class="container mx-auto text-center px-6">
                <div class="flex justify-center space-x-6 mb-6">
                    <a href="#" class="text-2xl text-gray-400 hover:text-[#00ffff] transition-colors duration-300"><i class="fab fa-facebook"></i></a>
                    <a href="#" class="text-2xl text-gray-400 hover:text-[#ff00ff] transition-colors duration-300"><i class="fab fa-instagram"></i></a>
                    <a href="#" class="text-2xl text-gray-400 hover:text-red-500 transition-colors duration-300"><i class="fab fa-youtube"></i></a>
                </div>
                <p class="text-gray-500 text-sm">&copy; 2024 GAJANAN SOUND & DJ. All Rights Reserved.</p>
                <p class="text-gray-500 text-xs mt-2">Engineered for the night.</p>
            </div>
        </footer>
    </div>

    <!-- Portfolio Modal -->
    <div id="workModal" class="fixed inset-0 bg-black bg-opacity-75 z-[100] hidden items-center justify-center p-4 transition-opacity duration-300">
        <div class="bg-gray-900 border border-[#00ffff] rounded-lg shadow-xl max-w-2xl w-full relative transform transition-transform duration-300 scale-95" data-aos="zoom-in">
            <button id="closeModal" class="absolute -top-3 -right-3 bg-[#00ffff] text-white rounded-full h-9 w-9 flex items-center justify-center text-2xl leading-none shadow-lg hover:bg-cyan-600 transition-colors">&times;</button>
            <img id="modalImage" src="" alt="Project Image" class="w-full h-64 md:h-80 object-cover rounded-t-lg">
            <div class="p-6">
                <h3 id="modalTitle" class="text-2xl font-bold mb-2 text-white"></h3>
                <p id="modalDescription" class="text-gray-400"></p>
            </div>
        </div>
    </div>

    <!-- Thank You Modal -->
    <div id="thankYouModal" class="fixed inset-0 bg-black bg-opacity-75 z-[100] hidden items-center justify-center p-4 transition-opacity duration-300">
        <div class="bg-gray-900 border border-[#00ffff] rounded-lg shadow-xl max-w-sm w-full text-center p-8 relative transform transition-transform duration-300 scale-95">
            <button id="closeThankYouModal" class="absolute top-2 right-3 text-gray-500 hover:text-white text-3xl leading-none">&times;</button>
            <div class="text-[#00ffff] mb-4">
                <i class="fas fa-check-circle fa-4x"></i>
            </div>
            <h3 class="text-2xl font-bold mb-2 text-white">Thank You!</h3>
            <p class="text-gray-400">Your inquiry has been sent. We'll get back to you soon.</p>
        </div>
    </div>

    <!-- AOS Animation Library JS -->
    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            // Splash screen logic
            const splash = document.getElementById('splash-screen');
            const mainContent = document.getElementById('main-content');
            
            setTimeout(() => {
                splash.style.opacity = '0';
                splash.addEventListener('transitionend', () => {
                    splash.style.display = 'none';
                    mainContent.classList.remove('hidden-content');
                    AOS.init({ duration: 800, once: true });
                }, { once: true });

            }, 2000); // Shorter splash screen time for a snappier feel

            // Mobile menu toggle logic
            const mobileMenuButton = document.getElementById('mobile-menu-button');
            const mobileMenu = document.getElementById('mobile-menu');
            mobileMenuButton.addEventListener('click', () => mobileMenu.classList.toggle('hidden'));

            // Active nav link highlighting on scroll
            const sections = document.querySelectorAll('section');
            const navLinks = document.querySelectorAll('.nav-link');
            window.onscroll = () => {
                let current = 'home';
                sections.forEach(section => {
                    const sectionTop = section.offsetTop;
                    if (pageYOffset >= sectionTop - 150) {
                        current = section.getAttribute('id');
                    }
                });
                navLinks.forEach(link => {
                    link.classList.remove('active');
                    if (link.getAttribute('href') === '#' + current) {
                        link.classList.add('active');
                    }
                });
            };
            
            // Close mobile menu when a link is clicked
            navLinks.forEach(link => {
                link.addEventListener('click', () => {
                    if (!mobileMenu.classList.contains('hidden')) {
                        mobileMenu.classList.add('hidden');
                    }
                });
            });

            // Portfolio modal functionality
            const portfolioItems = document.querySelectorAll('.gallery-item[data-image]');
            const workModal = document.getElementById('workModal');
            const closeModalBtn = document.getElementById('closeModal');
            const modalImage = document.getElementById('modalImage');
            const modalTitle = document.getElementById('modalTitle');
            const modalDescription = document.getElementById('modalDescription');
            
            portfolioItems.forEach(item => {
                item.addEventListener('click', () => {
                    modalImage.src = item.dataset.image;
                    modalTitle.textContent = item.dataset.title;
                    modalDescription.textContent = item.dataset.description;
                    workModal.classList.remove('hidden');
                    workModal.classList.add('flex');
                });
            });

            function closeWorkModal() {
                workModal.classList.add('hidden');
                workModal.classList.remove('flex');
            }
            closeModalBtn.addEventListener('click', closeWorkModal);
            workModal.addEventListener('click', (e) => {
                if (e.target === workModal) closeWorkModal();
            });

            // Contact form and Thank You modal logic
            const contactForm = document.getElementById('contactForm');
            const thankYouModal = document.getElementById('thankYouModal');
            const closeThankYouBtn = document.getElementById('closeThankYouModal');

            contactForm.addEventListener('submit', function(e) {
                e.preventDefault();
                const name = document.getElementById('name').value;
                const email = document.getElementById('email').value;
                const message = document.getElementById('message').value;
                const phone = '7489600750';
                const whatsappMessage = `Hello GAJANAN SOUND & DJ,\n\nNew Inquiry:\n\n*Name:* ${name}\n*Email:* ${email}\n*Message:* ${message}`;
                const encodedMessage = encodeURIComponent(whatsappMessage);
                const whatsappUrl = `https://wa.me/91${phone}?text=${encodedMessage}`;
                window.open(whatsappUrl, '_blank');
                
                thankYouModal.classList.remove('hidden');
                thankYouModal.classList.add('flex');
                contactForm.reset();
            });

            function closeThankYouModal() {
                thankYouModal.classList.add('hidden');
                thankYouModal.classList.remove('flex');
            }
            closeThankYouBtn.addEventListener('click', closeThankYouModal);
            thankYouModal.addEventListener('click', (e) => {
                if(e.target === thankYouModal) closeThankYouModal();
            });
        });
    </script>

</body>
</html>
