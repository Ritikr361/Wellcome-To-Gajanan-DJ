<html lang="hi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GAJANAN SOUND & DJ - Club & Event Experts</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Monoton&family=Poppins:wght@400;500;600;700;900&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <!-- AOS Animation Library CSS -->
    <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet">
    <style>
        html {
            scroll-behavior: smooth;
        }
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #111827; /* bg-gray-900 */
            overflow-x: hidden; /* Prevents horizontal scroll/shake */
        }
        .font-monoton {
            font-family: 'Monoton', cursive;
        }
        .neon-text {
            color: #fff;
            animation: pulsate-text 4s infinite linear;
        }
        .neon-box-blue {
            box-shadow: 0 0 5px #0ea5e9, 0 0 15px #0ea5e9;
            animation: pulsate-box-blue 3s infinite linear;
        }
        .neon-box-pink {
             box-shadow: 0 0 5px #ec4899, 0 0 15px #ec4899;
             animation: pulsate-box-pink 3s infinite linear;
        }
        .nav-link.active {
            color: #38bdf8; /* sky-400 */
            font-weight: 700;
            transform: scale(1.1);
            text-shadow: 0 0 8px #38bdf8;
        }
        .gallery-item {
            aspect-ratio: 1 / 1;
            overflow: hidden;
            background-color: #000;
        }

        /* Pulsating Animation Keyframes */
        @keyframes pulsate-text {
            0%, 100% { text-shadow: 0 0 5px #0ea5e9, 0 0 10px #0ea5e9, 0 0 20px #0ea5e9, 0 0 40px #0ea5e9; }
            50% { text-shadow: 0 0 7px #0ea5e9, 0 0 15px #0ea5e9, 0 0 30px #0ea5e9, 0 0 60px #0ea5e9; }
        }
        @keyframes pulsate-box-blue {
            0%, 100% { box-shadow: 0 0 5px #0ea5e9, 0 0 15px #0ea5e9; }
            50% { box-shadow: 0 0 8px #0ea5e9, 0 0 25px #0ea5e9; }
        }
        @keyframes pulsate-box-pink {
            0%, 100% { box-shadow: 0 0 5px #ec4899, 0 0 15px #ec4899; }
            50% { box-shadow: 0 0 8px #ec4899, 0 0 25px #ec4899; }
        }

        /* Splash Screen Styles */
        #splash-screen {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: #111827;
            z-index: 1000;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            transition: opacity 0.5s ease-out;
        }
        .equalizer {
            display: flex;
            align-items: flex-end;
            height: 100px;
        }
        .equalizer span {
            display: block;
            width: 15px;
            background: linear-gradient(to top, #ec4899, #0ea5e9);
            margin: 0 4px;
            animation: dance 1.5s infinite linear;
            border-radius: 4px 4px 0 0;
        }
        @keyframes dance {
            0% { height: 10%; }
            25% { height: 100%; }
            50% { height: 40%; }
            75% { height: 75%; }
            100% { height: 10%; }
        }
        .equalizer span:nth-child(2) { animation-delay: 0.2s; }
        .equalizer span:nth-child(3) { animation-delay: 0.4s; }
        .equalizer span:nth-child(4) { animation-delay: 0.6s; }
        .equalizer span:nth-child(5) { animation-delay: 0.8s; }
        
        .splash-text {
            margin-top: 2rem;
            text-align: center;
        }
        .splash-text h1 {
            font-family: 'Monoton', cursive;
            font-size: 3rem;
            color: #fff;
            text-shadow: 0 0 10px #0ea5e9, 0 0 20px #0ea5e9;
            padding-bottom: 0.5rem;
            border-bottom: 2px solid #0ea5e9;
            display: inline-block;
        }
        .splash-text p {
            font-family: 'Poppins', sans-serif;
            font-size: 1.5rem;
            color: #ec4899;
            letter-spacing: 2px;
            text-shadow: 0 0 10px #ec4899;
            margin-top: 0.5rem;
        }
        .hidden-content {
            display: none;
        }
    </style>
</head>
<body class="bg-gray-900 text-gray-300">

    <!-- Splash Screen -->
    <div id="splash-screen">
        <div class="equalizer">
            <span></span>
            <span></span>
            <span></span>
            <span></span>
            <span></span>
        </div>
        <div class="splash-text">
            <h1>GAJANAN</h1>
            <p>SOUND & DJ</p>
        </div>
    </div>

    <div id="main-content" class="hidden-content">
        <!-- Header / Navbar -->
        <header id="navbar" class="bg-gray-900/70 backdrop-blur-lg sticky top-0 z-50">
            <div class="container mx-auto px-4 sm:px-6 py-4 flex justify-between items-center">
                <a href="#home" class="text-xl sm:text-2xl font-monoton tracking-wider text-white">
                    <i class="fa-solid fa-waveform-lines text-sky-400"></i> GAJANAN SOUND & DJ
                </a>
                <nav class="hidden md:flex space-x-8">
                    <a href="#home" class="nav-link transition duration-300 text-gray-400 hover:text-sky-400">Home</a>
                    <a href="#services" class="nav-link transition duration-300 text-gray-400 hover:text-sky-400">Services</a>
                    <a href="#work" class="nav-link transition duration-300 text-gray-400 hover:text-sky-400">Our Work</a>
                    <a href="#team" class="nav-link transition duration-300 text-gray-400 hover:text-sky-400">Our Team</a>
                    <a href="#pricing" class="nav-link transition duration-300 text-gray-400 hover:text-sky-400">Pricing</a>
                    <a href="#contact" class="nav-link transition duration-300 text-gray-400 hover:text-sky-400">Contact</a>
                </nav>
                <a href="#contact" class="hidden lg:inline-block bg-sky-500 hover:bg-sky-600 text-white font-bold py-2 px-4 rounded-lg transition duration-300 neon-box-blue">Contact Us</a>
                <button id="mobile-menu-button" class="md:hidden text-white text-2xl p-2">
                    <i class="fas fa-bars"></i>
                </button>
            </div>
            <!-- Mobile Menu -->
            <div id="mobile-menu" class="hidden md:hidden bg-gray-800">
                <a href="#home" class="nav-link block py-3 px-4 text-base hover:bg-gray-700">Home</a>
                <a href="#services" class="nav-link block py-3 px-4 text-base hover:bg-gray-700">Services</a>
                <a href="#work" class="nav-link block py-3 px-4 text-base hover:bg-gray-700">Our Work</a>
                <a href="#team" class="nav-link block py-3 px-4 text-base hover:bg-gray-700">Our Team</a>
                <a href="#pricing" class="nav-link block py-3 px-4 text-base hover:bg-gray-700">Pricing</a>
                <a href="#contact" class="nav-link block py-3 px-4 text-base hover:bg-gray-700">Contact Us</a>
            </div>
        </header>

        <main>
            <!-- Home Section -->
            <section id="home">
                <div class="relative h-[70vh] md:h-[90vh] text-white overflow-hidden">
                    <!-- Static Background Image -->
                    <div class="absolute inset-0">
                         <img src="https://images.unsplash.com/photo-1514525253161-7a46d19cd819?q=80&w=1974&auto=format&fit=crop" onerror="this.onerror=null;this.src='https://placehold.co/1920x1080/000000/FFFFFF?text=Live+Concert';" class="w-full h-full object-cover" alt="Live Concert Stage">
                    </div>
                    <!-- Overlay -->
                    <div class="absolute inset-0 bg-black bg-opacity-60 flex items-center justify-center">
                        <div class="text-center px-4" data-aos="zoom-in">
                            <h1 class="font-monoton text-4xl sm:text-5xl md:text-7xl mb-4 drop-shadow-lg neon-text">Feel The Vibe</h1>
                            <p class="text-lg md:text-2xl mb-8 text-gray-300 drop-shadow-md font-semibold">High-End Light & Sound For Unforgettable Nights</p>
                            <a href="#work" class="bg-pink-500 hover:bg-pink-600 text-white font-bold py-3 px-8 rounded-full text-lg transition duration-300 transform hover:scale-105 neon-box-pink">See Our Events</a>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Services Section -->
            <section id="services" class="py-16 md:py-20 bg-gray-800">
                <div class="container mx-auto px-4 sm:px-6">
                    <div class="text-center mb-12" data-aos="fade-down">
                        <h2 class="text-3xl md:text-4xl font-bold text-white">Our Expertise</h2>
                        <p class="text-gray-400 mt-2">We power events that make a statement.</p>
                    </div>
                    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
                        <!-- Service Card 1 -->
                        <div class="bg-gray-900 rounded-lg p-6 text-center transform hover:-translate-y-2 transition duration-300 shadow-lg hover:shadow-sky-500/40" data-aos="fade-up" data-aos-delay="100">
                            <i class="fa-solid fa-champagne-glasses text-5xl text-sky-400 mb-4"></i>
                            <h3 class="text-xl font-bold mb-2 text-white">Private Parties</h3>
                            <p class="text-gray-400">Exclusive setups for birthdays, anniversaries, and private celebrations.</p>
                        </div>
                        <!-- Service Card 2 -->
                        <div class="bg-gray-900 rounded-lg p-6 text-center transform hover:-translate-y-2 transition duration-300 shadow-lg hover:shadow-sky-500/40" data-aos="fade-up" data-aos-delay="200">
                            <i class="fa-solid fa-record-vinyl text-5xl text-sky-400 mb-4"></i>
                            <h3 class="text-xl font-bold mb-2 text-white">DJ Nights & Pubs</h3>
                            <p class="text-gray-400">Pulsating sound and dynamic lights for the ultimate clubbing experience.</p>
                        </div>
                        <!-- Service Card 3 -->
                        <div class="bg-gray-900 rounded-lg p-6 text-center transform hover:-translate-y-2 transition duration-300 shadow-lg hover:shadow-sky-500/40" data-aos="fade-up" data-aos-delay="300">
                            <i class="fa-solid fa-building-columns text-5xl text-sky-400 mb-4"></i>
                            <h3 class="text-xl font-bold mb-2 text-white">Corporate Events</h3>
                            <p class="text-gray-400">Professional and sleek AV solutions for launches, conferences, and galas.</p>
                        </div>
                        <!-- Service Card 4 -->
                        <div class="bg-gray-900 rounded-lg p-6 text-center transform hover:-translate-y-2 transition duration-300 shadow-lg hover:shadow-sky-500/40" data-aos="fade-up" data-aos-delay="400">
                            <i class="fa-solid fa-masks-theater text-5xl text-sky-400 mb-4"></i>
                            <h3 class="text-xl font-bold mb-2 text-white">Live Concerts</h3>
                            <p class="text-gray-400">Massive stage setups with concert-grade sound and lighting trusses.</p>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Our Work / Portfolio Section -->
            <section id="work" class="py-16 md:py-20 bg-gray-900">
                <div class="container mx-auto px-4 sm:px-6">
                    <div class="text-center mb-12" data-aos="fade-down">
                        <h2 class="text-3xl md:text-4xl font-bold text-white">Event Gallery</h2>
                        <p class="text-gray-400 mt-2">A glimpse into the experiences we create.</p>
                    </div>
                    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
                        <!-- YouTube Short Embed -->
                        <div class="gallery-item rounded-lg shadow-lg overflow-hidden" data-aos="zoom-in-up" data-aos-delay="100">
                            <iframe class="w-full h-full" src="https://www.youtube.com/embed/XBeobtTWXfQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
                        </div>
                        <div class="gallery-item rounded-lg shadow-lg overflow-hidden" data-aos="zoom-in-up" data-aos-delay="200">
                            <iframe class="w-full h-full" src="https://www.youtube.com/embed/Oc03TUTAYgw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
                        </div>
                        <div class="group relative overflow-hidden rounded-lg shadow-lg cursor-pointer portfolio-item gallery-item" data-aos="zoom-in-up" data-aos-delay="300"
                             data-image="https://images.unsplash.com/photo-1524368535928-5b5e00ddc76b?q=80&w=1770&auto=format&fit=crop"
                             data-title="Rooftop Sangeet Party"
                             data-description="A chic and stylish Sangeet ceremony on a rooftop, featuring elegant ambient lighting, fairy lights, and a premium sound setup for live music and DJ.">
                            <img src="https://images.unsplash.com/photo-1524368535928-5b5e00ddc76b?q=80&w=1770&auto=format&fit=crop" class="w-full h-full object-cover transform group-hover:scale-110 transition duration-500">
                            <div class="absolute inset-0 bg-black bg-opacity-0 group-hover:bg-opacity-70 transition duration-500 flex items-center justify-center"><h3 class="text-lg font-bold text-white opacity-0 group-hover:opacity-100 transition duration-500 p-4 text-center">Rooftop Sangeet Party</h3></div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Pricing Section -->
            <section id="pricing" class="py-16 md:py-20 bg-gray-800">
                <div class="container mx-auto px-4 sm:px-6">
                    <div class="text-center mb-12" data-aos="fade-down">
                        <h2 class="text-3xl md:text-4xl font-bold text-white">Event Packages</h2>
                        <p class="text-gray-400 mt-2">Choose the perfect power-pack for your event.</p>
                    </div>
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-8 max-w-4xl mx-auto">
                        <!-- Basic Package -->
                        <div class="bg-gray-900 rounded-lg p-8 border-2 border-gray-700 text-center flex flex-col" data-aos="fade-up" data-aos-delay="100">
                            <h3 class="text-2xl font-bold text-sky-400 mb-4">Ignite</h3>
                            <p class="text-4xl font-extrabold text-white mb-4">₹20,000 <span class="text-lg font-normal text-gray-400">/event</span></p>
                            <ul class="text-gray-400 space-y-2 mb-8 text-left flex-grow">
                                <li><i class="fas fa-check-circle text-green-500 mr-2"></i>Dynamic Party Lights</li>
                                <li><i class="fas fa-check-circle text-green-500 mr-2"></i>High-Quality Sound System</li>
                                <li><i class="fas fa-check-circle text-green-500 mr-2"></i>Ideal for House Parties</li>
                            </ul>
                            <a href="#contact" class="mt-auto bg-gray-700 hover:bg-sky-500 text-white font-bold py-2 px-4 rounded-lg transition duration-300">Book Now</a>
                        </div>
                        <!-- Premium Package -->
                        <div class="bg-gray-900 rounded-lg p-8 border-2 border-pink-500 text-center flex flex-col transform md:scale-105 shadow-2xl shadow-pink-500/30" data-aos="fade-up" data-aos-delay="200">
                            <p class="absolute top-0 -translate-y-1/2 left-1/2 -translate-x-1/2 bg-pink-500 text-white text-xs font-bold px-3 py-1 rounded-full">PRO'S CHOICE</p>
                            <h3 class="text-2xl font-bold text-pink-400 mb-4">Overdrive</h3>
                            <p class="text-4xl font-extrabold text-white mb-4">₹50,000 <span class="text-lg font-normal text-gray-400">/event</span></p>
                            <ul class="text-gray-400 space-y-2 mb-8 text-left flex-grow">
                                <li><i class="fas fa-check-circle text-green-500 mr-2"></i>Laser & LED Video Wall</li>
                                <li><i class="fas fa-check-circle text-green-500 mr-2"></i>Club-Grade Sound System</li>
                                <li><i class="fas fa-check-circle text-green-500 mr-2"></i>Perfect for Pubs & Sangeet</li>
                                <li><i class="fas fa-check-circle text-green-500 mr-2"></i>Professional DJ Included</li>
                            </ul>
                            <a href="#contact" class="mt-auto bg-pink-500 hover:bg-pink-600 text-white font-bold py-2 px-4 rounded-lg transition duration-300">Book Now</a>
                        </div>
                        <!-- Custom Package -->
                        <div class="bg-gray-900 rounded-lg p-8 border-2 border-gray-700 text-center flex flex-col" data-aos="fade-up" data-aos-delay="300">
                            <h3 class="text-2xl font-bold text-sky-400 mb-4">Apocalypse</h3>
                            <p class="text-4xl font-extrabold text-white mb-4">Let's Talk</p>
                            <ul class="text-gray-400 space-y-2 mb-8 text-left flex-grow">
                                <li><i class="fas fa-check-circle text-green-500 mr-2"></i>Full Concert Production</li>
                                <li><i class="fas fa-check-circle text-green-500 mr-2"></i>Custom Stage & Trussing</li>
                                <li><i class="fas fa-check-circle text-green-500 mr-2"></i>International Standard AV</li>
                            </ul>
                            <a href="#contact" class="mt-auto bg-gray-700 hover:bg-sky-500 text-white font-bold py-2 px-4 rounded-lg transition duration-300">Book Now</a>
                        </div>
                    </div>
                </div>
            </section>
            
            <!-- Team Section -->
            <section id="team" class="py-16 md:py-20 bg-gray-900">
                <div class="container mx-auto px-4 sm:px-6">
                    <div class="text-center mb-12" data-aos="fade-down">
                        <h2 class="text-3xl md:text-4xl font-bold text-white">The Crew</h2>
                        <p class="text-gray-400 mt-2">The masterminds behind the console.</p>
                    </div>
                    <div class="flex flex-col sm:flex-row justify-center items-center gap-8 sm:gap-12">
                        <!-- Founder Card -->
                        <div class="text-center" data-aos="fade-up" data-aos-delay="100">
                            <img src="https://res.cloudinary.com/dtjjgiitl/image/upload/q_auto:good,f_auto,fl_progressive/v1752681317/g0bibqhoyardg0n2ggaq.jpg" onerror="this.onerror=null;this.src='https://placehold.co/150x150/f97316/FFFFFF?text=V';" alt="Founder Vinay" class="w-36 h-36 mx-auto rounded-full shadow-lg border-4 border-sky-500 mb-4 object-cover">
                            <h3 class="text-xl font-bold text-white">Vinnay Verma</h3>
                            <p class="text-sky-400">Founder</p>
                        </div>
                        <!-- Co-Founder Card -->
                        <div class="text-center" data-aos="fade-up" data-aos-delay="200">
                            <img src="https://res.cloudinary.com/dtjjgiitl/image/upload/q_auto:good,f_auto,fl_progressive/v1752681371/orrjv6zq0fcr2qwgqmi6.jpg" onerror="this.onerror=null;this.src='https://placehold.co/150x150/3b82f6/FFFFFF?text=HG';" alt="Co-Founder Harsh Gupta" class="w-36 h-36 mx-auto rounded-full shadow-lg border-4 border-pink-500 mb-4 object-cover">
                            <h3 class="text-xl font-bold text-white">Harsh Gupta</h3>
                            <p class="text-pink-400">Co-Founder</p>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Contact Section -->
            <section id="contact" class="py-16 md:py-20 bg-gray-800">
                <div class="container mx-auto px-4 sm:px-6">
                    <div class="text-center mb-12" data-aos="fade-down">
                        <h2 class="text-3xl md:text-4xl font-bold text-white">Book Your Date</h2>
                        <p class="text-gray-400 mt-2">Let's plan an event that they'll talk about for years.</p>
                    </div>
                    <div class="flex flex-col lg:flex-row gap-8">
                        <div class="w-full lg:w-1/2" data-aos="fade-right">
                            <div class="bg-gray-900 rounded-lg p-8 shadow-lg h-full">
                                <form id="contactForm">
                                    <div class="mb-4"><label for="name" class="block text-gray-400 mb-2">Name</label><input type="text" id="name" name="name" class="w-full bg-gray-800 text-white rounded-lg py-2 px-3 focus:outline-none focus:ring-2 focus:ring-sky-500" required></div>
                                    <div class="mb-4"><label for="email" class="block text-gray-400 mb-2">Email</label><input type="email" id="email" name="email" class="w-full bg-gray-800 text-white rounded-lg py-2 px-3 focus:outline-none focus:ring-2 focus:ring-sky-500" required></div>
                                    <div class="mb-4"><label for="message" class="block text-gray-400 mb-2">Event Details</label><textarea id="message" name="message" rows="4" class="w-full bg-gray-800 text-white rounded-lg py-2 px-3 focus:outline-none focus:ring-2 focus:ring-sky-500" required></textarea></div>
                                    <button type="submit" class="w-full bg-sky-500 hover:bg-sky-600 text-white font-bold py-3 px-4 rounded-lg transition duration-300 neon-box-blue">Send Inquiry</button>
                                </form>
                            </div>
                        </div>
                        <div class="w-full lg:w-1/2" data-aos="fade-left">
                            <div class="bg-gray-900 rounded-lg p-8 h-full flex flex-col justify-center shadow-lg">
                                <div class="mb-6"><h3 class="text-xl font-bold text-white mb-2 flex items-center"><i class="fas fa-phone-alt text-sky-400 mr-3"></i> Phone</h3><a href="tel:+917489600750" class="text-gray-300 hover:text-sky-400">+91 74896 00750</a></div>
                                <div class="mb-6"><h3 class="text-xl font-bold text-white mb-2 flex items-center"><i class="fas fa-envelope text-sky-400 mr-3"></i> Email</h3><a href="mailto:contact@gajanansounddj.com" class="text-gray-300 hover:text-sky-400">contact@gajanansounddj.com</a></div>
                                <div><h3 class="text-xl font-bold text-white mb-2 flex items-center"><i class="fas fa-map-marker-alt text-sky-400 mr-3"></i> Address</h3><p class="text-gray-300">Rajgarh Naka, Jhabua, Madhya Pradesh, India</p></div>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
        </main>

        <!-- Footer -->
        <footer class="bg-gray-900 border-t border-gray-800">
            <div class="container mx-auto px-6 py-8 text-center text-gray-400">
                <div class="flex justify-center space-x-6 mb-4"><a href="#" class="text-2xl hover:text-sky-400 transition duration-300"><i class="fab fa-facebook"></i></a><a href="#" class="text-2xl hover:text-pink-400 transition duration-300"><i class="fab fa-instagram"></i></a><a href="#" class="text-2xl hover:text-red-500 transition duration-300"><i class="fab fa-youtube"></i></a></div>
                <p>&copy; 2024 GAJANAN SOUND & DJ. All Rights Reserved.</p>
                <p class="text-sm mt-2">Engineered for the night.</p>
            </div>
        </footer>

        <!-- Portfolio Modal -->
        <div id="workModal" class="fixed inset-0 bg-black bg-opacity-75 z-[100] hidden items-center justify-center p-4 transition-opacity duration-300">
            <div class="bg-gray-800 border border-sky-500 rounded-lg shadow-xl max-w-2xl w-full relative transform transition-transform duration-300 scale-95" data-aos="zoom-in">
                <button id="closeModal" class="absolute -top-3 -right-3 bg-sky-500 text-white rounded-full h-9 w-9 flex items-center justify-center text-2xl leading-none shadow-lg hover:bg-sky-600 transition-colors">&times;</button>
                <img id="modalImage" src="" alt="Project Image" class="w-full h-64 md:h-80 object-cover rounded-t-lg">
                <div class="p-6">
                    <h3 id="modalTitle" class="text-2xl font-bold mb-2 text-white"></h3>
                    <p id="modalDescription" class="text-gray-300"></p>
                </div>
            </div>
        </div>

        <!-- Thank You Modal -->
        <div id="thankYouModal" class="fixed inset-0 bg-black bg-opacity-75 z-[100] hidden items-center justify-center p-4 transition-opacity duration-300">
            <div class="bg-gray-800 border border-green-500 rounded-lg shadow-xl max-w-sm w-full text-center p-8 relative transform transition-transform duration-300 scale-95">
                 <button id="closeThankYouModal" class="absolute top-2 right-3 text-gray-500 hover:text-white text-3xl leading-none">&times;</button>
                <div class="text-green-400 mb-4">
                    <i class="fas fa-check-circle fa-4x"></i>
                </div>
                <h3 class="text-2xl font-bold mb-2 text-white">Thank You!</h3>
                <p class="text-gray-300">Your inquiry has been sent. We'll get back to you soon.</p>
            </div>
        </div>
    </div>


    <!-- AOS Animation Library JS -->
    <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            const splash = document.getElementById('splash-screen');
            const mainContent = document.getElementById('main-content');
            
            setTimeout(() => {
                splash.style.opacity = '0';
                splash.addEventListener('transitionend', () => {
                    splash.style.display = 'none';
                    mainContent.classList.remove('hidden-content');
                     AOS.init({ duration: 800, once: true });
                }, { once: true });

            }, 3000);

            const mobileMenuButton = document.getElementById('mobile-menu-button');
            const mobileMenu = document.getElementById('mobile-menu');
            mobileMenuButton.addEventListener('click', () => mobileMenu.classList.toggle('hidden'));

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
            
            navLinks.forEach(link => {
                link.addEventListener('click', () => {
                    if (!mobileMenu.classList.contains('hidden')) {
                        mobileMenu.classList.add('hidden');
                    }
                });
            });

            const portfolioItems = document.querySelectorAll('.portfolio-item');
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
