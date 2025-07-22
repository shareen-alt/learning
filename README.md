<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lavender Learning Hub</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        
        :root {
            --lavender-50: #f5f3ff;
            --lavender-100: #ede9fe;
            --lavender-200: #ddd6fe;
            --lavender-300: #c4b5fd;
            --lavender-400: #a78bfa;
            --lavender-500: #8b5cf6;
            --lavender-600: #7c3aed;
            --lavender-700: #6d28d9;
            --lavender-800: #5b21b6;
            --lavender-900: #4c1d95;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: var(--lavender-50);
        }
        
        .lavender-bg {
            background-color: var(--lavender-200);
        }
        
        .lavender-text {
            color: var(--lavender-700);
        }
        
        .lavender-border {
            border-color: var(--lavender-400);
        }
        
        .lavender-button {
            background-color: var(--lavender-600);
            color: white;
        }
        
        .lavender-button:hover {
            background-color: var(--lavender-700);
        }
        
        .testimonial-card {
            transition: transform 0.3s ease;
        }
        
        .testimonial-card:hover {
            transform: translateY(-5px);
        }
        
        .course-card {
            transition: all 0.3s ease;
            border: 2px solid var(--lavender-300);
        }
        
        .course-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
            border-color: var(--lavender-500);
        }
        
        .teacher-img {
            border: 3px solid var(--lavender-400);
        }
    </style>
</head>
<body>
    <!-- Navigation -->
    <nav class="lavender-bg shadow-lg">
        <div class="max-w-6xl mx-auto px-4">
            <div class="flex justify-between">
                <div class="flex space-x-7">
                    <div>
                        <a href="#" class="flex items-center py-4 px-2">
                            <span class="font-semibold text-xl lavender-text">Lavender Learning Hub</span>
                        </a>
                    </div>
                </div>
                <div class="hidden md:flex items-center space-x-1">
                    <a href="#" class="py-4 px-2 text-gray-700 hover:text-purple-900 transition duration-300">Home</a>
                    <a href="#courses" class="py-4 px-2 text-gray-700 hover:text-purple-900 transition duration-300">Courses</a>
                    <a href="#about" class="py-4 px-2 text-gray-700 hover:text-purple-900 transition duration-300">About</a>
                    <a href="#testimonials" class="py-4 px-2 text-gray-700 hover:text-purple-900 transition duration-300">Testimonials</a>
                    <a href="#contact" class="py-4 px-2 text-gray-700 hover:text-purple-900 transition duration-300">Contact</a>
                </div>
                <div class="md:hidden flex items-center">
                    <button class="outline-none mobile-menu-button">
                        <svg class="w-6 h-6 text-gray-700 hover:text-purple-900"
                            x-show="!showMenu"
                            fill="none"
                            stroke-linecap="round"
                            stroke-linejoin="round"
                            stroke-width="2"
                            viewBox="0 0 24 24"
                            stroke="currentColor"
                        >
                            <path d="M4 6h16M4 12h16M4 18h16"></path>
                        </svg>
                    </button>
                </div>
            </div>
        </div>
        <div class="hidden mobile-menu">
            <ul>
                <li><a href="#" class="block px-2 py-4 hover:bg-purple-100 transition duration-300">Home</a></li>
                <li><a href="#courses" class="block px-2 py-4 hover:bg-purple-100 transition duration-300">Courses</a></li>
                <li><a href="#about" class="block px-2 py-4 hover:bg-purple-100 transition duration-300">About</a></li>
                <li><a href="#testimonials" class="block px-2 py-4 hover:bg-purple-100 transition duration-300">Testimonials</a></li>
                <li><a href="#contact" class="block px-2 py-4 hover:bg-purple-100 transition duration-300">Contact</a></li>
            </ul>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="lavender-bg">
        <div class="container mx-auto flex px-5 py-24 md:flex-row flex-col items-center">
            <div class="lg:flex-grow md:w-1/2 lg:pr-24 md:pr-16 flex flex-col md:items-start md:text-left mb-16 md:mb-0 items-center text-center">
                <h1 class="title-font sm:text-4xl text-3xl mb-4 font-bold lavender-text">
                    Unlock Your Potential 
                    <br class="hidden lg:inline-block">With Our Courses
                </h1>
                <p class="mb-8 leading-relaxed text-gray-700">
                    Join thousands of students who have transformed their careers with our expert-led courses. Learn at your own pace with our flexible online learning platform.
                </p>
                <div class="flex justify-center">
                    <a href="#courses" class="inline-flex text-white lavender-button border-0 py-2 px-6 focus:outline-none hover:bg-purple-700 rounded text-lg">
                        Explore Courses
                    </a>
                    <a href="#contact" class="ml-4 inline-flex text-gray-700 bg-gray-100 border-0 py-2 px-6 focus:outline-none hover:bg-gray-200 rounded text-lg">
                        Contact Us
                    </a>
                </div>
            </div>
            <div class="lg:max-w-lg lg:w-full md:w-1/2 w-5/6">
                <img class="object-cover object-center rounded" alt="hero" src="https://images.unsplash.com/photo-1522202176988-66273c2fd55f?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1471&q=80">
            </div>
        </div>
    </section>

    <!-- Courses Section -->
    <section id="courses" class="text-gray-700 body-font">
        <div class="container px-5 py-24 mx-auto">
            <div class="flex flex-col text-center w-full mb-20">
                <h1 class="sm:text-3xl text-2xl font-bold title-font mb-4 lavender-text">Our Popular Courses</h1>
                <p class="lg:w-2/3 mx-auto leading-relaxed text-base">Choose from our wide range of courses designed to help you succeed in today's competitive world.</p>
            </div>
            <div class="flex flex-wrap -m-4">
                <!-- Course 1 -->
                <div class="p-4 md:w-1/3">
                    <div class="h-full border-2 border-gray-200 rounded-lg overflow-hidden course-card">
                        <img class="lg:h-48 md:h-36 w-full object-cover object-center" src="https://images.unsplash.com/photo-1551434678-e076c223a692?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="blog">
                        <div class="p-6">
                            <h2 class="tracking-widest text-xs title-font font-medium text-gray-500 mb-1">WEB DEVELOPMENT</h2>
                            <h1 class="title-font text-lg font-medium text-gray-900 mb-3">Full Stack Web Development</h1>
                            <p class="leading-relaxed mb-3">Master both front-end and back-end development with our comprehensive course.</p>
                            <div class="flex items-center flex-wrap ">
                                <span class="text-purple-700 font-bold text-xl">₹150/HR</span>
                                <a href="#contact" class="lavender-button inline-flex items-center md:mb-2 lg:mb-0 ml-auto px-3 py-1 rounded">
                                    Enroll Now
                                    <svg class="w-4 h-4 ml-2" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round">
                                        <path d="M5 12h14"></path>
                                        <path d="M12 5l7 7-7 7"></path>
                                    </svg>
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- Course 2 -->
                <div class="p-4 md:w-1/3">
                    <div class="h-full border-2 border-gray-200 rounded-lg overflow-hidden course-card">
                        <img class="lg:h-48 md:h-36 w-full object-cover object-center" src="https://images.unsplash.com/photo-1635070041078-e363dbe005cb?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="blog">
                        <div class="p-6">
                            <h2 class="tracking-widest text-xs title-font font-medium text-gray-500 mb-1">AI & PROMPTS</h2>
                            <h1 class="title-font text-lg font-medium text-gray-900 mb-3">AI and Prompt Engineering</h1>
                            <p class="leading-relaxed mb-3">Master AI tools and effective prompt engineering techniques for optimal results.</p>
                            <div class="flex items-center flex-wrap">
                                <span class="text-purple-700 font-bold text-xl">₹150/HR</span>
                                <a href="#contact" class="lavender-button inline-flex items-center md:mb-2 lg:mb-0 ml-auto px-3 py-1 rounded">
                                    Enroll Now
                                    <svg class="w-4 h-4 ml-2" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round">
                                        <path d="M5 12h14"></path>
                                        <path d="M12 5l7 7-7 7"></path>
                                    </svg>
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- Course 4 -->
                <div class="p-4 md:w-1/3">
                    <div class="h-full border-2 border-gray-200 rounded-lg overflow-hidden course-card">
                        <img class="lg:h-48 md:h-36 w-full object-cover object-center" src="https://images.unsplash.com/photo-1551288049-bebda4e38f71?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80" alt="blog">
                        <div class="p-6">
                            <h2 class="tracking-widest text-xs title-font font-medium text-gray-500 mb-1">DATA ENTRY</h2>
                            <h1 class="title-font text-lg font-medium text-gray-900 mb-3">Data Entry Mastery</h1>
                            <p class="leading-relaxed mb-3">Learn efficient data entry techniques and tools to boost your productivity.</p>
                            <div class="flex items-center flex-wrap">
                                <span class="text-purple-700 font-bold text-xl">₹150/HR</span>
                                <a href="#contact" class="lavender-button inline-flex items-center md:mb-2 lg:mb-0 ml-auto px-3 py-1 rounded">
                                    Enroll Now
                                    <svg class="w-4 h-4 ml-2" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round">
                                        <path d="M5 12h14"></path>
                                        <path d="M12 5l7 7-7 7"></path>
                                    </svg>
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
                <!-- Course 3 (Graphic Design) -->
                <div class="p-4 md:w-1/3">
                    <div class="h-full border-2 border-gray-200 rounded-lg overflow-hidden course-card">
                        <img class="lg:h-48 md:h-36 w-full object-cover object-center" src="https://images.unsplash.com/photo-1626785774573-4b799315345d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1471&q=80" alt="blog">
                        <div class="p-6">
                            <h2 class="tracking-widest text-xs title-font font-medium text-gray-500 mb-1">GRAPHIC DESIGN</h2>
                            <h1 class="title-font text-lg font-medium text-gray-900 mb-3">Graphic Design Masterclass</h1>
                            <p class="leading-relaxed mb-3">Create stunning visuals with Adobe Photoshop, Illustrator and InDesign.</p>
                            <div class="flex items-center flex-wrap ">
                                <span class="text-purple-700 font-bold text-xl">₹150/HR</span>
                                <a href="#contact" class="lavender-button inline-flex items-center md:mb-2 lg:mb-0 ml-auto px-3 py-1 rounded">
                                    Enroll Now
                                    <svg class="w-4 h-4 ml-2" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round">
                                        <path d="M5 12h14"></path>
                                        <path d="M12 5l7 7-7 7"></path>
                                    </svg>
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="lavender-bg body-font">
        <div class="container mx-auto flex px-5 py-24 md:flex-row flex-col items-center">
            <div class="lg:max-w-lg lg:w-full md:w-1/2 w-5/6 mb-10 md:mb-0">
                <img class="object-cover object-center rounded" alt="hero" src="https://images.unsplash.com/photo-1523240795612-9a054b0db644?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80">
            </div>
            <div class="lg:flex-grow md:w-1/2 lg:pl-24 md:pl-16 flex flex-col md:items-start md:text-left items-center text-center">
                <h1 class="title-font sm:text-4xl text-3xl mb-4 font-bold lavender-text">About Lavender Learning Hub</h1>
                <p class="mb-8 leading-relaxed text-gray-700">
                    Founded in 2024, Lavender Learning Hub is dedicated to providing high-quality, affordable education to students worldwide. Our mission is to make learning accessible to everyone, regardless of their background or location.
                </p>
                <div class="flex flex-col w-full">
                    <div class="flex items-center mb-4">
                        <div class="w-8 h-8 mr-3 inline-flex items-center justify-center rounded-full bg-purple-100 text-purple-700 flex-shrink-0">
                            <i class="fas fa-chalkboard-teacher"></i>
                        </div>
                        <h2 class="text-gray-900 text-lg title-font font-medium">Expert Instructors</h2>
                    </div>
                    <p class="text-gray-700 mb-4">Learn from industry professionals with years of real-world experience.</p>
                    
                    <div class="flex items-center mb-4">
                        <div class="w-8 h-8 mr-3 inline-flex items-center justify-center rounded-full bg-purple-100 text-purple-700 flex-shrink-0">
                            <i class="fas fa-laptop-code"></i>
                        </div>
                        <h2 class="text-gray-900 text-lg title-font font-medium">Hands-on Projects</h2>
                    </div>
                    <p class="text-gray-700 mb-4">Apply what you learn through practical projects that build your portfolio.</p>
                    
                    <div class="flex items-center mb-4">
                        <div class="w-8 h-8 mr-3 inline-flex items-center justify-center rounded-full bg-purple-100 text-purple-700 flex-shrink-0">
                            <i class="fas fa-user-graduate"></i>
                        </div>
                        <h2 class="text-gray-900 text-lg title-font font-medium">Career Support</h2>
                    </div>
                    <p class="text-gray-700">Get help with resume building, interview preparation, and job placement.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section id="testimonials" class="text-gray-700 body-font">
        <div class="container px-5 py-24 mx-auto">
            <div class="flex flex-col text-center w-full mb-20">
                <h1 class="sm:text-3xl text-2xl font-bold title-font mb-4 lavender-text">Student Testimonials</h1>
                <p class="lg:w-2/3 mx-auto leading-relaxed text-base">Hear what our students have to say about their learning experience with us.</p>
            </div>
            <div class="flex flex-wrap -m-4">
                <div class="p-4 md:w-1/2 w-full">
                    <div class="h-full bg-gray-100 p-8 rounded testimonial-card">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="block w-5 h-5 text-purple-700 mb-4" viewBox="0 0 975.036 975.036">
                            <path d="M925.036 57.197h-304c-27.6 0-50 22.4-50 50v304c0 27.601 22.4 50 50 50h145.5c-1.9 79.601-20.4 143.3-55.4 191.2-27.6 37.8-69.399 69.1-125.3 93.8-25.7 11.3-36.8 41.7-27.3 67.2l18.8 85.5c8.6 40.9 44.1 72.7 85.6 72.7h166.9c27.6 0 50-22.4 50-50v-304c0-27.599-22.4-50-50-50h-145.5c12.8-36.1 19.9-79.2 19.9-128.8 0-101.7-22.3-180.9-62-242.3C847.8 72.6 888.9 50 925.036 50v7.197z"></path>
                        </svg>
                        <p class="leading-relaxed mb-6">The Full Stack Web Development course completely transformed my career. Within 3 months of completing the course, I landed a job as a junior developer. The instructors were incredibly supportive and the curriculum was perfectly structured.</p>
                        <div class="mt-4">
                            <span class="title-font font-medium text-gray-900">Alex Raj</span>
                            <span class="text-gray-500 text-sm block">Web Developer</span>
                        </div>
                    </div>
                </div>
                <div class="p-4 md:w-1/2 w-full">
                    <div class="h-full bg-gray-100 p-8 rounded testimonial-card">
                        <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="block w-5 h-5 text-purple-700 mb-4" viewBox="0 0 975.036 975.036">
                            <path d="M925.036 57.197h-304c-27.6 0-50 22.4-50 50v304c0 27.601 22.4 50 50 50h145.5c-1.9 79.601-20.4 143.3-55.4 191.2-27.6 37.8-69.399 69.1-125.3 93.8-25.7 11.3-36.8 41.7-27.3 67.2l18.8 85.5c8.6 40.9 44.1 72.7 85.6 72.7h166.9c27.6 0 50-22.4 50-50v-304c0-27.599-22.4-50-50-50h-145.5c12.8-36.1 19.9-79.2 19.9-128.8 0-101.7-22.3-180.9-62-242.3C847.8 72.6 888.9 50 925.036 50v7.197z"></path>
                        </svg>
                        <p class="leading-relaxed mb-6">As someone with no prior experience in data science, I was nervous about starting the course. But the way concepts were broken down made everything so easy to understand. The hands-on projects were especially valuable in helping me build confidence.</p>
                        <div class="mt-4">
                            <span class="title-font font-medium text-gray-900">Shreya Rai</span>
                            <span class="text-gray-500 text-sm block">Data Analyst</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Teachers Section -->
    <section class="lavender-bg body-font">
        <div class="container px-5 py-24 mx-auto">
            <div class="flex flex-col text-center w-full mb-20">
                <h1 class="sm:text-3xl text-2xl font-bold title-font mb-4 lavender-text">Meet Our Instructors</h1>
                <p class="lg:w-2/3 mx-auto leading-relaxed text-gray-700">Learn from industry experts with years of teaching and professional experience.</p>
            </div>
            <div class="flex flex-wrap -m-4">
                <div class="p-4 lg:w-1/3">
                    <div class="h-full bg-white bg-opacity-75 px-8 pt-16 pb-24 rounded-lg overflow-hidden text-center relative">
                        <h1 class="title-font sm:text-2xl text-xl font-medium text-gray-900 mb-3">Alex Raj</h1>
                        <p class="leading-relaxed mb-3">Full Stack Developer with 2+ years of experience building web applications for Fortune companies.</p>
                        <a class="text-purple-700 inline-flex items-center">View Profile
                            <svg class="w-4 h-4 ml-2" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M5 12h14"></path>
                                <path d="M12 5l7 7-7 7"></path>
                            </svg>
                        </a>
                    </div>
                </div>
                <div class="p-4 lg:w-1/3">
                    <div class="h-full bg-white bg-opacity-75 px-8 pt-16 pb-24 rounded-lg overflow-hidden text-center relative">
                        <h1 class="title-font sm:text-2xl text-xl font-medium text-gray-900 mb-3">Shreya Rai</h1>
                        <p class="leading-relaxed mb-3">Data Scientist specializing in machine learning and AI, previously worked at Google and Microsoft.</p>
                        <a class="text-purple-700 inline-flex items-center">View Profile
                            <svg class="w-4 h-4 ml-2" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M5 12h14"></path>
                                <path d="M12 5l7 7-7 7"></path>
                            </svg>
                        </a>
                    </div>
                </div>
                <div class="p-4 lg:w-1/3">
                    <div class="h-full bg-white bg-opacity-75 px-8 pt-16 pb-24 rounded-lg overflow-hidden text-center relative">
                        <h1 class="title-font sm:text-2xl text-xl font-medium text-gray-900 mb-3">Shareen Fatima</h1>
                        <p class="leading-relaxed mb-3">Creative Director and Graphic Designer with 10+ years of experience in branding and visual communication.</p>
                        <a class="text-purple-700 inline-flex items-center">View Profile
                            <svg class="w-4 h-4 ml-2" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2" fill="none" stroke-linecap="round" stroke-linejoin="round">
                                <path d="M5 12h14"></path>
                                <path d="M12 5l7 7-7 7"></path>
                            </svg>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="text-gray-700 body-font relative">
        <div class="container px-5 py-24 mx-auto">
            <div class="flex flex-col text-center w-full mb-12">
                <h1 class="sm:text-3xl text-2xl font-bold title-font mb-4 lavender-text">Contact Us</h1>
                <p class="lg:w-2/3 mx-auto leading-relaxed text-base">Have questions? Get in touch with our team for more information about our courses.</p>
            </div>
            <div class="lg:w-1/2 md:w-2/3 mx-auto">
                <div class="flex flex-wrap -m-2">
                    <div class="p-2 w-full">
                        <div class="relative">
                            <label for="name" class="leading-7 text-sm text-gray-600">Name</label>
                            <input type="text" id="name" name="name" class="w-full bg-gray-100 rounded border border-gray-300 focus:border-purple-500 focus:bg-white focus:ring-2 focus:ring-purple-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out">
                        </div>
                    </div>
                    <div class="p-2 w-full">
                        <div class="relative">
                            <label for="email" class="leading-7 text-sm text-gray-600">Email</label>
                            <input type="email" id="email" name="email" class="w-full bg-gray-100 rounded border border-gray-300 focus:border-purple-500 focus:bg-white focus:ring-2 focus:ring-purple-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out">
                        </div>
                    </div>
                    <div class="p-2 w-full">
                        <div class="relative">
                            <label for="phone" class="leading-7 text-sm text-gray-600">Phone Number</label>
                            <input type="tel" id="phone" name="phone" class="w-full bg-gray-100 rounded border border-gray-300 focus:border-purple-500 focus:bg-white focus:ring-2 focus:ring-purple-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out mb-4">
                            <label for="course" class="leading-7 text-sm text-gray-600">Name of Course</label>
                            <input type="text" id="course" name="course" class="w-full bg-gray-100 rounded border border-gray-300 focus:border-purple-500 focus:bg-white focus:ring-2 focus:ring-purple-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out mb-4">
                            <label for="message" class="leading-7 text-sm text-gray-600">Additional Message</label>
                            <textarea id="message" name="message" class="w-full bg-gray-100 rounded border border-gray-300 focus:border-purple-500 focus:bg-white focus:ring-2 focus:ring-purple-200 h-32 text-base outline-none text-gray-700 py-1 px-3 resize-none leading-6 transition-colors duration-200 ease-in-out"></textarea>
                        </div>
                    </div>
                    <div class="p-2 w-full">
                        <button onclick="sendWhatsAppMessage()" type="button" class="flex mx-auto text-white lavender-button border-0 py-2 px-8 focus:outline-none hover:bg-purple-700 rounded text-lg">
                            Send Message
                        </button>
                    </div>
                    <div class="p-2 w-full pt-8 mt-8 border-t border-gray-200 text-center">
                        <div class="flex flex-col items-center">
                            <div class="w-12 h-1 rounded mt-2 mb-4 lavender-bg"></div>
                            <h2 class="text-gray-900 font-medium title-font tracking-wider text-sm">CONTACT INFORMATION</h2>
                            <p class="text-gray-600">fatimashareen778@gmail.com</p>
                            <p class="text-gray-600">7678592378</p>
                            <div class="flex mt-4">
                                <a class="text-purple-700 hover:text-purple-900 mx-2">
                                    <i class="fab fa-facebook-f text-xl"></i>
                                </a>
                                <a class="text-purple-700 hover:text-purple-900 mx-2">
                                    <i class="fab fa-twitter text-xl"></i>
                                </a>
                                <a href="https://instagram.com/__shr3n" target="_blank" class="text-purple-700 hover:text-purple-900 mx-2">
                                    <i class="fab fa-instagram text-xl"></i>
                                </a>
                                <a class="text-purple-700 hover:text-purple-900 mx-2">
                                    <i class="fab fa-linkedin-in text-xl"></i>
                                </a>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="lavender-bg text-gray-700 body-font">
        <div class="container px-5 py-8 mx-auto flex items-center sm:flex-row flex-col">
            <a class="flex title-font font-medium items-center md:justify-start justify-center text-gray-900">
                <span class="ml-3 text-xl lavender-text">Lavender Learning Hub</span>
            </a>
            <p class="text-sm text-gray-500 sm:ml-4 sm:pl-4 sm:border-l-2 sm:border-gray-200 sm:py-2 sm:mt-0 mt-4">© 2023 Lavender Learning Hub —
                <a href="https://twitter.com/knyttneve" class="text-gray-600 ml-1" rel="noopener noreferrer" target="_blank">@lavenderlearning</a>
            </p>
            <span class="inline-flex sm:ml-auto sm:mt-0 mt-4 justify-center sm:justify-start">
                <a class="text-gray-500">
                    <svg fill="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="w-5 h-5" viewBox="0 0 24 24">
                        <path d="M18 2h-3a5 5 0 00-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 011-1h3z"></path>
                    </svg>
                </a>
                <a class="ml-3 text-gray-500">
                    <svg fill="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="w-5 h-5" viewBox="0 0 24 24">
                        <path d="M23 3a10.9 10.9 0 01-3.14 1.53 4.48 4.48 0 00-7.86 3v1A10.66 10.66 0 013 4s-4 9 5 13a11.64 11.64 0 01-7 2c9 5 20 0 20-11.5a4.5 4.5 0 00-.08-.83A7.72 7.72 0 0023 3z"></path>
                    </svg>
                </a>
                <a href="https://instagram.com/__shr3n" target="_blank" class="ml-3 text-gray-500">
                    <svg fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="w-5 h-5" viewBox="0 0 24 24">
                        <rect width="20" height="20" x="2" y="2" rx="5" ry="5"></rect>
                        <path d="M16 11.37A4 4 0 1112.63 8 4 4 0 0116 11.37zm1.5-4.87h.01"></path>
                    </svg>
                </a>
                <a class="ml-3 text-gray-500">
                    <svg fill="currentColor" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="0" class="w-5 h-5" viewBox="0 0 24 24">
                        <path stroke="none" d="M16 8a6 6 0 016 6v7h-4v-7a2 2 0 00-2-2 2 2 0 00-2 2v7h-4v-7a6 6 0 016-6zM2 9h4v12H2z"></path>
                        <circle cx="4" cy="4" r="2" stroke="none"></circle>
                    </svg>
                </a>
            </span>
        </div>
    </footer>

    <script>
        // Mobile menu toggle
        const btn = document.querySelector("button.mobile-menu-button");
        const menu = document.querySelector(".mobile-menu");

        btn.addEventListener("click", () => {
            menu.classList.toggle("hidden");
        });

        function sendWhatsAppMessage() {
            // Get form values
            const name = document.getElementById("name").value;
            const email = document.getElementById("email").value;
            const phone = document.getElementById("phone").value;
            const course = document.getElementById("course").value;
            const message = document.getElementById("message").value;
            
            // Format WhatsApp message
            const whatsappMessage = `New Enrollment Inquiry:%0A%0AName: ${name}%0AEmail: ${email}%0APhone: ${phone}%0ACourse: ${course}%0AMessage: ${message || 'No additional message'}`;
            
            // Open WhatsApp with pre-filled message
            window.open(`https://wa.me/917678592378?text=${whatsappMessage}`, '_blank');
        }

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    targetElement.scrollIntoView({
                        behavior: 'smooth'
                    });
                }
            });
        });
    </script>
</body>
</html>
