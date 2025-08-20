<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jane Doe - PhD Candidate</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        /* Style for the particle background container */
        #tsparticles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1; /* Places it behind all other content */
        }
        /* Active state for navigation links */
        .nav-link.active {
            color: #2563eb; /* text-blue-600 */
            font-weight: 700;
            transform: translateX(5px);
        }
        /* Smooth transition for nav links */
        .nav-link {
            transition: all 0.2s ease-in-out;
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800">

    <!-- Particle background container -->
    <div id="tsparticles"></div>

    <!-- Main container for two-column layout -->
    <div class="max-w-screen-xl mx-auto md:flex">

        <!-- Left-side Fixed Panel -->
        <header class="md:w-1/3 lg:w-1/4 md:h-screen md:sticky top-0 p-8 lg:p-12 flex flex-col justify-between">
            <div>
                <!-- Profile Info -->
                <div class="text-center md:text-left">
                    <div class="w-32 h-32 rounded-full overflow-hidden shadow-lg mx-auto md:mx-0 mb-4">
                        <img src="https://placehold.co/400x400/E2E8F0/4A5568?text=Your+Photo" alt="A professional headshot of Jane Doe" class="w-full h-full object-cover">
                    </div>
                    <h1 class="text-3xl font-bold text-gray-900">Jane Doe</h1>
                    <p class="text-lg text-blue-700 mt-1">PhD Candidate in Computational Linguistics</p>
                    <p class="text-gray-600 mt-4 max-w-xs mx-auto md:mx-0">
                        Exploring the intersection of NLP and cognitive science at the University of Science.
                    </p>
                </div>

                <!-- Navigation -->
                <nav class="hidden md:block mt-12">
                    <ul class="space-y-4" id="desktop-nav">
                        <li><a href="#about" class="nav-link text-gray-600 hover:text-blue-600 flex items-center"><span class="w-8 h-px bg-gray-400 mr-4"></span> About</a></li>
                        <li><a href="#research" class="nav-link text-gray-600 hover:text-blue-600 flex items-center"><span class="w-8 h-px bg-gray-400 mr-4"></span> Research</a></li>
                        <li><a href="#publications" class="nav-link text-gray-600 hover:text-blue-600 flex items-center"><span class="w-8 h-px bg-gray-400 mr-4"></span> Publications</a></li>
                        <li><a href="#contact" class="nav-link text-gray-600 hover:text-blue-600 flex items-center"><span class="w-8 h-px bg-gray-400 mr-4"></span> Contact</a></li>
                    </ul>
                </nav>
            </div>
            
            <!-- Socials & CV -->
            <div class="text-center md:text-left mt-8 md:mt-0">
                 <div class="flex justify-center md:justify-start space-x-4 mb-4">
                    <a href="#" class="text-gray-500 hover:text-blue-600 transition-colors" aria-label="Google Scholar">
                        <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true"><path d="M5.242 13.769L0 9.5L12 0l12 9.5l-5.242 4.269C17.548 11.249 14.978 9 12 9s-5.548 2.249-6.758 4.769zM12 10c-1.381 0-2.5 1.119-2.5 2.5s1.119 2.5 2.5 2.5c1.022 0 1.888-.622 2.296-1.5H12v-1.5h4.496c.004.167.004.334.004.5c0 2.485-2.015 4.5-4.5 4.5s-4.5-2.015-4.5-4.5S9.515 10 12 10z"/></svg>
                    </a>
                     <a href="#" class="text-gray-500 hover:text-blue-600 transition-colors" aria-label="LinkedIn">
                        <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true"><path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/></svg>
                    </a>
                    <a href="#" class="text-gray-500 hover:text-blue-600 transition-colors" aria-label="Twitter">
                        <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true"><path d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616v.064c0 2.299 1.634 4.211 3.803 4.652-.667.18-1.372.247-2.083.196.616 1.924 2.403 3.32 4.523 3.36-1.791 1.401-4.033 2.185-6.466 2.185-.42 0-.835-.025-1.243-.073 2.298 1.473 5.031 2.34 8.016 2.34 9.621 0 14.885-7.978 14.885-14.885 0-.227-.005-.453-.014-.678.98-.711 1.829-1.599 2.5-2.59z"/></svg>
                    </a>
                </div>
                <a href="cv.pdf" download class="bg-blue-600 text-white font-medium py-2 px-4 rounded-lg hover:bg-blue-700 transition-all shadow-sm text-sm inline-block">Download CV</a>
            </div>
        </header>

        <!-- Right-side Scrollable Content -->
        <main class="md:w-2/3 lg:w-3/4 p-8 lg:p-12">
            <div class="max-w-3xl">
                <!-- About Me Section -->
                <section id="about" class="mb-24 scroll-mt-24">
                    <h2 class="text-2xl font-bold text-gray-900 mb-6 md:hidden">About Me</h2>
                    <p class="text-lg text-gray-700 leading-relaxed mb-4">
                        I am a final-year PhD candidate at the University of Science, advised by the esteemed Dr. Alan Turing. My research focuses on developing robust models for understanding nuanced human language, including sarcasm and metaphor, which traditional NLP models often struggle with. 
                    </p>
                    <p class="text-lg text-gray-700 leading-relaxed">
                        Before my doctoral studies, I completed my M.S. in Computer Science and a B.A. in Linguistics. This interdisciplinary background fuels my passion for creating technology that not only processes language but truly comprehends its depth and context. When I'm not in the lab, I enjoy hiking, photography, and contributing to open-source NLP libraries.
                    </p>
                </section>

                <!-- Research Section -->
                <section id="research" class="mb-24 scroll-mt-24">
                    <h2 class="text-2xl font-bold text-gray-900 mb-6">Research Interests</h2>
                    <div class="grid md:grid-cols-2 gap-6">
                        <div class="bg-white/80 backdrop-blur-sm p-6 rounded-xl shadow-md">
                            <h3 class="text-xl font-bold mb-2">Metaphor & Sarcasm Detection</h3>
                            <p class="text-gray-600">Developing multi-modal models that leverage textual and acoustic cues to improve the detection of non-literal language.</p>
                        </div>
                        <div class="bg-white/80 backdrop-blur-sm p-6 rounded-xl shadow-md">
                            <h3 class="text-xl font-bold mb-2">Low-Resource Language Understanding</h3>
                            <p class="text-gray-600">Utilizing transfer learning and few-shot techniques to build effective NLP models for languages with limited data.</p>
                        </div>
                        <div class="bg-white/80 backdrop-blur-sm p-6 rounded-xl shadow-md">
                            <h3 class="text-xl font-bold mb-2">Explainable AI (XAI) for NLP</h3>
                            <p class="text-gray-600">Investigating methods to make large language models more transparent and interpretable.</p>
                        </div>
                    </div>
                </section>

                <!-- Publications Section -->
                <section id="publications" class="mb-24 scroll-mt-24">
                    <h2 class="text-2xl font-bold text-gray-900 mb-6">Selected Publications</h2>
                    <div class="space-y-8">
                        <div class="p-6 rounded-xl bg-white/80 backdrop-blur-sm shadow-md">
                            <p class="font-semibold text-gray-800 mb-1">ACL 2024</p>
                            <h3 class="font-bold text-lg text-gray-900">"Hearing the Irony: An Acoustic-Textual Approach to Sarcasm"</h3>
                            <p class="text-gray-600 text-sm"><strong>Jane Doe</strong>, John Smith, and Alan Turing</p>
                            <div class="mt-2"><a href="#" class="text-blue-600 hover:underline text-sm">[PDF]</a> <a href="#" class="text-blue-600 hover:underline text-sm">[Code]</a> <a href="#" class="text-blue-600 hover:underline text-sm">[DOI]</a></div>
                        </div>
                        <div class="p-6 rounded-xl bg-white/80 backdrop-blur-sm shadow-md">
                            <p class="font-semibold text-gray-800 mb-1">EMNLP 2023</p>
                            <h3 class="font-bold text-lg text-gray-900">"Few-Shot Learning for Underrepresented Languages"</h3>
                            <p class="text-gray-600 text-sm">John Smith, <strong>Jane Doe</strong>, and Alan Turing</p>
                            <div class="mt-2"><a href="#" class="text-blue-600 hover:underline text-sm">[PDF]</a> <a href="#" class="text-blue-600 hover:underline text-sm">[DOI]</a></div>
                        </div>
                        <div class="p-6 rounded-xl bg-white/80 backdrop-blur-sm shadow-md">
                            <p class="font-semibold text-gray-800 mb-1">NeurIPS 2022</p>
                            <h3 class="font-bold text-lg text-gray-900">"Probing the Black Box: Interpretability in Transformer Models"</h3>
                            <p class="text-gray-600 text-sm"><strong>Jane Doe</strong>, and Alan Turing</p>
                            <div class="mt-2"><a href="#" class="text-blue-600 hover:underline text-sm">[PDF]</a> <a href="#" class="text-blue-600 hover:underline text-sm">[DOI]</a></div>
                        </div>
                    </div>
                </section>

                <!-- Contact Section -->
                <section id="contact" class="mb-16 scroll-mt-24">
                    <h2 class="text-2xl font-bold text-gray-900 mb-6">Get In Touch</h2>
                    <p class="text-lg text-gray-700 mb-6">
                        I'm always open to discussing new research, collaborations, or interesting opportunities. Feel free to reach out.
                    </p>
                    <a href="mailto:jane.doe@university.edu" class="inline-block bg-blue-600 text-white font-medium py-3 px-6 rounded-lg hover:bg-blue-700 transition-all shadow-md">jane.doe@university.edu</a>
                </section>

                <footer class="text-center text-gray-500 text-sm py-8">
                    &copy; 2024 Jane Doe. All Rights Reserved.
                </footer>
            </div>
        </main>
    </div>

    <!-- tsParticles library -->
    <script src="https://cdn.jsdelivr.net/npm/tsparticles@2/tsparticles.bundle.min.js"></script>
    
    <script>
        // Scroll-spy for navigation
        const sections = document.querySelectorAll('section[id]');
        const navLinks = document.querySelectorAll('#desktop-nav a');

        window.addEventListener('scroll', () => {
            let current = '';
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                if (pageYOffset >= sectionTop - 150) { // Adjust offset as needed
                    current = section.getAttribute('id');
                }
            });

            navLinks.forEach(link => {
                link.classList.remove('active');
                if (link.getAttribute('href').includes(current)) {
                    link.classList.add('active');
                }
            });
        });

        // tsParticles initialization
        window.addEventListener('load', () => {
            tsParticles.load("tsparticles", {
                fpsLimit: 60,
                interactivity: {
                    events: {
                        onHover: { enable: true, mode: "grab" },
                        resize: true
                    },
                    modes: {
                        grab: { distance: 140, links: { opacity: 1 } }
                    }
                },
                particles: {
                    color: { value: "#a0aec0" },
                    links: { color: "#cbd5e0", distance: 150, enable: true, opacity: 0.5, width: 1 },
                    collisions: { enable: true },
                    move: { direction: "none", enable: true, outModes: { default: "bounce" }, random: false, speed: 1, straight: false },
                    number: { density: { enable: true, area: 800 }, value: 60 },
                    opacity: { value: 0.5 },
                    shape: { type: "circle" },
                    size: { value: { min: 1, max: 4 } }
                },
                detectRetina: true
            });
        });
    </script>
</body>
</html>
