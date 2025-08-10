<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Music Theory Hub | Chords, Notes & Scales</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        :root {
            --primary: #6366f1;
            --primary-dark: #4f46e5;
            --dark: #0f172a;
            --light: #f8fafc;
            --accent: #10b981;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
        }

        body {
            background-color: var(--dark);
            color: var(--light);
            overflow-x: hidden;
        }

        .gradient-text {
            background: linear-gradient(90deg, var(--primary), var(--accent));
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            display: inline-block;
        }

        .hero-gradient {
            background: radial-gradient(circle at center, rgba(99, 102, 241, 0.1) 0%, rgba(15, 23, 42, 0) 70%);
        }

        .feature-card {
            transition: all 0.3s ease;
            background: rgba(15, 23, 42, 0.6);
            backdrop-filter: blur(10px);
        }

        .feature-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1);
        }

        .nav-glass {
            background: rgba(15, 23, 42, 0.7);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid rgba(241, 245, 249, 0.1);
        }

        .animate-float {
            animation: float 6s ease-in-out infinite;
        }

        .animate-float-delay {
            animation: float 6s ease-in-out infinite;
            animation-delay: 1s;
        }

        .animate-pulse {
            animation: pulse 4s cubic-bezier(0.4, 0, 0.6, 1) infinite;
        }

        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-15px); }
            100% { transform: translateY(0px); }
        }

        @keyframes pulse {
            0%, 100% { opacity: 1; }
            50% { opacity: 0.6; }
        }

        .gradient-border {
            position: relative;
        }

        .gradient-border::before {
            content: '';
            position: absolute;
            top: -1px;
            left: -1px;
            right: -1px;
            bottom: -1px;
            background: linear-gradient(45deg, var(--primary), var(--accent));
            border-radius: 8px;
            z-index: -1;
            transition: all 0.3s ease;
        }

        .input-glass {
            background: rgba(241, 245, 249, 0.05);
            backdrop-filter: blur(5px);
            border: 1px solid rgba(241, 245, 249, 0.1);
        }

        .input-glass:focus {
            outline: none;
            border-color: var(--primary);
        }

        .scrollbar-hide::-webkit-scrollbar {
            display: none;
        }

        .scrollbar-hide {
            -ms-overflow-style: none;
            scrollbar-width: none;
        }

        .sparkle {
            position: absolute;
            background: white;
            border-radius: 50%;
            pointer-events: none;
            z-index: 100;
        }
    </style>
</head>
<body>
    <header class="nav-glass fixed w-full z-50">
        <div class="container mx-auto px-6 py-4">
            <div class="flex justify-between items-center">
                <div class="flex items-center space-x-2">
                    <span class="text-xl font-bold">Music Theory Hub</span>
                </div>
                
                <nav class="hidden md:flex space-x-8">
                    <a href="#" class="hover:text-indigo-400 transition">Home</a>
                    <a href="#" class="hover:text-indigo-400 transition">Chords</a>
                    <a href="#" class="hover:text-indigo-400 transition">Scales</a>
                    <a href="#" class="hover:text-indigo-400 transition">Rhythm</a>
                    <a href="#" class="hover:text-indigo-400 transition">Lessons</a>
                </nav>
                
                <div class="flex items-center space-x-4">
                    <button class="md:hidden">
                        <i class="fas fa-bars"></i>
                    </button>
                </div>
            </div>
        </div>
    </header>

    <main>
        <!-- Hero Section -->
        <section class="hero-gradient pt-20 pb-10 px-6">
            <div class="container mx-auto text-center">
                <h1 class="text-3xl md:text-4xl font-bold mb-4">Master Music Theory</h1>
                <p class="text-gray-400 mb-6 text-lg max-w-2xl mx-auto">
                    Learn chords, scales, notes and more to elevate your musical skills.
                </p>
                <div class="relative mx-auto max-w-3xl">
                    <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/37d2aadd-55b5-46c3-a999-8321297d935a.png" alt="Breaking news scene showing reporters and cameras" class="rounded-lg shadow-lg">
                </div>
            </div>
        </section>

        <!-- Clients Section -->
        <section class="py-16 px-6">
            <div class="container mx-auto">
                <p class="text-gray-400 text-center mb-6">Trusted by musicians worldwide</p>
                <div class="flex justify-center space-x-8">
                    <div class="text-center">
                        <i class="fas fa-guitar text-3xl text-indigo-400 mb-2"></i>
                        <p class="text-sm">Guitarists</p>
                    </div>
                    <div class="text-center">
                        <i class="fas fa-piano text-3xl text-emerald-400 mb-2"></i>
                        <p class="text-sm">Pianists</p>
                    </div>
                    <div class="text-center">
                        <i class="fas fa-music text-3xl text-purple-400 mb-2"></i>
                        <p class="text-sm">Producers</p>
                    </div>
                    <div class="text-center">
                        <i class="fas fa-user-graduate text-3xl text-yellow-400 mb-2"></i>
                        <p class="text-sm">Educators</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Features Section -->
        <section id="features" class="py-20 px-6">
            <div class="container mx-auto">
                <div class="text-center mb-16">
                    <span class="inline-block px-3 py-1 rounded-full bg-gray-800 text-emerald-400 mb-4">FEATURES</span>
                    <h2 class="text-3xl md:text-4xl font-bold mb-4">AI-Powered Efficiency <span class="gradient-text">Boosters</span></h2>
                    <p class="text-gray-400 max-w-2xl mx-auto">
                        Our suite of intelligent tools adapts to your workflow, automating mundane tasks and freeing you to focus on what matters.
                    </p>
                </div>
                
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                    <!-- Feature 1 -->
                    <div class="feature-card rounded-xl p-8 border border-gray-800">
                        <div class="w-12 h-12 rounded-lg bg-indigo-900 flex items-center justify-center mb-6">
                            <i class="fas fa-music text-indigo-400 text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-3">Chord Progressions</h3>
                        <p class="text-gray-400 mb-4">
                            Learn common chord progressions used in popular music across all genres.
                        </p>
                        <button class="text-indigo-400 hover:text-indigo-300 transition flex items-center">
                            Learn More <i class="fas fa-arrow-right ml-2"></i>
                        </button>
                    </div>
                    
                    <!-- Feature 2 -->
                    <div class="feature-card rounded-xl p-8 border border-gray-800">
                        <div class="w-12 h-12 rounded-lg bg-emerald-900 flex items-center justify-center mb-6">
                            <i class="fas fa-chart-line text-emerald-400 text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-3">Real-Time Analytics</h3>
                        <p class="text-gray-400 mb-4">
                            Get actionable insights with beautifully visualized data dashboards.
                        </p>
                        <button class="text-emerald-400 hover:text-emerald-300 transition flex items-center">
                            Learn More <i class="fas fa-arrow-right ml-2"></i>
                        </button>
                    </div>
                    
                    <!-- Feature 3 -->
                    <div class="feature-card rounded-xl p-8 border border-gray-800">
                        <div class="w-12 h-12 rounded-lg bg-purple-900 flex items-center justify-center mb-6">
                            <i class="fas fa-volume-up text-purple-400 text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-3">Ear Training</h3>
                        <p class="text-gray-400 mb-4">
                            Develop your musical ear to recognize intervals, chords, and melodies.
                        </p>
                        <button class="text-purple-400 hover:text-purple-300 transition flex items-center">
                            Learn More <i class="fas fa-arrow-right ml-2"></i>
                        </button>
                    </div>
                    
                    <!-- Feature 4 -->
                    <div class="feature-card rounded-xl p-8 border border-gray-800">
                        <div class="w-12 h-12 rounded-lg bg-blue-900 flex items-center justify-center mb-6">
                            <i class="fas fa-shield-alt text-blue-400 text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-3">Enterprise Security</h3>
                        <p class="text-gray-400 mb-4">
                            Military-grade encryption and privacy controls you can trust.
                        </p>
                        <button class="text-blue-400 hover:text-blue-300 transition flex items-center">
                            Learn More <i class="fas fa-arrow-right ml-2"></i>
                        </button>
                    </div>
                    
                    <!-- Feature 5 -->
                    <div class="feature-card rounded-xl p-8 border border-gray-800">
                        <div class="w-12 h-12 rounded-lg bg-pink-900 flex items-center justify-center mb-6">
                            <i class="fas fa-sync-alt text-pink-400 text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-3">Seamless Sync</h3>
                        <p class="text-gray-400 mb-4">
                            Real-time updates across all your devices and platforms.
                        </p>
                        <button class="text-pink-400 hover:text-pink-300 transition flex items-center">
                            Learn More <i class="fas fa-arrow-right ml-2"></i>
                        </button>
                    </div>
                    
                    <!-- Feature 6 -->
                    <div class="feature-card rounded-xl p-8 border border-gray-800">
                        <div class="w-12 h-12 rounded-lg bg-yellow-900 flex items-center justify-center mb-6">
                            <i class="fas fa-cogs text-yellow-400 text-xl"></i>
                        </div>
                        <h3 class="text-xl font-bold mb-3">Custom Workflows</h3>
                        <p class="text-gray-400 mb-4">
                            Design personalized automation flows with our drag-and-drop builder.
                        </p>
                        <button class="text-yellow-400 hover:text-yellow-300 transition flex items-center">
                            Learn More <i class="fas fa-arrow-right ml-2"></i>
                        </button>
                    </div>
                </div>
            </div>
        </section>

        <!-- Solutions Section -->
        <section id="solutions" class="py-20 px-6 bg-gray-900">
            <div class="container mx-auto">
                <div class="text-center mb-16">
                    <span class="inline-block px-3 py-1 rounded-full bg-gray-800 text-indigo-400 mb-4">INTEGRATIONS</span>
                    <h2 class="text-3xl md:text-4xl font-bold mb-4">Works With Your <span class="gradient-text">Favorite Tools</span></h2>
                    <p class="text-gray-400 max-w-2xl mx-auto">
                        Nexus integrates seamlessly with the platforms you already use, creating a unified productivity ecosystem.
                    </p>
                </div>
                
                <div class="flex flex-col lg:flex-row items-center gap-12">
                    <div class="lg:w-1/2">
                        <div class="grid grid-cols-3 gap-6">
                            <div class="bg-gray-800 rounded-xl p-6 flex flex-col items-center hover:bg-gray-700 transition">
                                <div class="w-16 h-16 bg-gray-700 rounded-lg flex items-center justify-center mb-4">
                                    <i class="fab fa-slack text-2xl text-purple-400"></i>
                                </div>
                                <span class="font-medium">Slack</span>
                            </div>
                            <div class="bg-gray-800 rounded-xl p-6 flex flex-col items-center hover:bg-gray-700 transition">
                                <div class="w-16 h-16 bg-gray-700 rounded-lg flex items-center justify-center mb-4">
                                    <i class="fab fa-google text-2xl text-red-400"></i>
                                </div>
                                <span class="font-medium">Google</span>
                            </div>
                            <div class="bg-gray-800 rounded-xl p-6 flex flex-col items-center hover:bg-gray-700 transition">
                                <div class="w-16 h-16 bg-gray-700 rounded-lg flex items-center justify-center mb-4">
                                    <i class="fab fa-microsoft text-2xl text-blue-400"></i>
                                </div>
                                <span class="font-medium">Microsoft</span>
                            </div>
                            <div class="bg-gray-800 rounded-xl p-6 flex flex-col items-center hover:bg-gray-700 transition">
                                <div class="w-16 h-16 bg-gray-700 rounded-lg flex items-center justify-center mb-4">
                                    <i class="fas fa-project-diagram text-2xl text-green-400"></i>
                                </div>
                                <span class="font-medium">Trello</span>
                            </div>
                            <div class="bg-gray-800 rounded-xl p-6 flex flex-col items-center hover:bg-gray-700 transition">
                                <div class="w-16 h-16 bg-gray-700 rounded-lg flex items-center justify-center mb-4">
                                    <i class="fas fa-envelope text-2xl text-yellow-400"></i>
                                </div>
                                <span class="font-medium">Mail</span>
                            </div>
                            <div class="bg-gray-800 rounded-xl p-6 flex flex-col items-center hover:bg-gray-700 transition">
                                <div class="w-16 h-16 bg-gray-700 rounded-lg flex items-center justify-center mb-4">
                                    <i class="fas fa-database text-2xl text-indigo-400"></i>
                                </div>
                                <span class="font-medium">Zapier</span>
                            </div>
                        </div>
                    </div>
                    
                    <div class="lg:w-1/2">
                        <div class="bg-gray-800 rounded-xl p-8">
                            <h3 class="text-xl font-bold mb-4">One-Click Magic</h3>
                            <p class="text-gray-400 mb-6">
                                Connect Nexus with over 500+ applications instantly. Our AI learns your integrations and suggests optimizations tailored to your workflow.
                            </p>
                            <div class="flex items-center space-x-4">
                                <div class="relative">
                                    <div class="w-12 h-12 rounded-full bg-indigo-500 flex items-center justify-center">
                                        <i class="fas fa-random text-white"></i>
                                    </div>
                                    <div class="w-12 h-12 rounded-full bg-emerald-500 flex items-center justify-center absolute -top-2 -right-2">
                                        <i class="fas fa-plus text-white text-sm"></i>
                                    </div>
                                </div>
                                <div>
                                    <h4 class="font-bold">Smart Connection Engine</h4>
                                    <p class="text-gray-400 text-sm">Auto-detects optimal pathways</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Pricing Section -->
        <section id="pricing" class="py-20 px-6">
            <div class="container mx-auto">
                <div class="text-center mb-16">
                    <span class="inline-block px-3 py-1 rounded-full bg-gray-800 text-emerald-400 mb-4">PRICING</span>
                    <h2 class="text-3xl md:text-4xl font-bold mb-4">Simple, Transparent <span class="gradient-text">Pricing</span></h2>
                    <p class="text-gray-400 max-w-2xl mx-auto">
                        Pay for what you need with plans that scale with your business.
                    </p>
                </div>
                
                <div class="grid grid-cols-1 md:grid-cols-3 gap-8 max-w-5xl mx-auto">
                    <!-- Starter Plan -->
                    <div class="rounded-xl overflow-hidden border border-gray-800 hover:border-indigo-500 transition">
                        <div class="bg-gray-900 p-6">
                            <h3 class="text-xl font-bold mb-2">Starter</h3>
                            <p class="text-gray-400 mb-4">Perfect for individuals and small teams</p>
                            <div class="flex items-end mb-6">
                                <span class="text-4xl font-bold">$19</span>
                                <span class="text-gray-400 ml-1">/user/month</span>
                            </div>
                            <button class="w-full py-3 rounded-lg border border-gray-700 hover:bg-gray-800 transition">
                                Get Started
                            </button>
                        </div>
                        <div class="border-t border-gray-800 bg-gray-900 p-6">
                            <ul class="space-y-3">
                                <li class="flex items-start">
                                    <i class="fas fa-check text-emerald-400 mt-1 mr-2"></i>
                                    <span>Up to 5 users</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check text-emerald-400 mt-1 mr-2"></i>
                                    <span>Basic automations</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check text-emerald-400 mt-1 mr-2"></i>
                                    <span>Standard integrations</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check text-emerald-400 mt-1 mr-2"></i>
                                    <span>Email support</span>
                                </li>
                            </ul>
                        </div>
                    </div>
                    
                    <!-- Pro Plan (Featured) -->
                    <div class="rounded-xl overflow-hidden border-2 border-indigo-500 transform scale-105 relative">
                        <div class="absolute -top-3 left-1/2 transform -translate-x-1/2 bg-indigo-500 text-white px-3 py-1 rounded-full text-xs font-bold">
                            POPULAR
                        </div>
                        <div class="bg-gray-900 p-6">
                            <h3 class="text-xl font-bold mb-2">Professional</h3>
                            <p class="text-gray-400 mb-4">For growing teams that need more power</p>
                            <div class="flex items-end mb-6">
                                <span class="text-4xl font-bold">$49</span>
                                <span class="text-gray-400 ml-1">/user/month</span>
                            </div>
                            <button class="w-full py-3 rounded-lg bg-gradient-to-r from-indigo-500 to-emerald-500 text-white font-medium hover:opacity-90 transition">
                                Get Started
                            </button>
                        </div>
                        <div class="border-t border-gray-800 bg-gray-900 p-6">
                            <ul class="space-y-3">
                                <li class="flex items-start">
                                    <i class="fas fa-check text-emerald-400 mt-1 mr-2"></i>
                                    <span>Up to 25 users</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check text-emerald-400 mt-1 mr-2"></i>
                                    <span>Advanced automations</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check text-emerald-400 mt-1 mr-2"></i>
                                    <span>Premium integrations</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check text-emerald-400 mt-1 mr-2"></i>
                                    <span>Priority support</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check text-emerald-400 mt-1 mr-2"></i>
                                    <span>Custom workflows</span>
                                </li>
                            </ul>
                        </div>
                    </div>
                    
                    <!-- Enterprise Plan -->
                    <div class="rounded-xl overflow-hidden border border-gray-800 hover:border-indigo-500 transition">
                        <div class="bg-gray-900 p-6">
                            <h3 class="text-xl font-bold mb-2">Enterprise</h3>
                            <p class="text-gray-400 mb-4">For organizations with complex needs</p>
                            <div class="flex items-end mb-6">
                                <span class="text-4xl font-bold">$99</span>
                                <span class="text-gray-400 ml-1">/user/month</span>
                            </div>
                            <button class="w-full py-3 rounded-lg border border-gray-700 hover:bg-gray-800 transition">
                                Contact Sales
                            </button>
                        </div>
                        <div class="border-t border-gray-800 bg-gray-900 p-6">
                            <ul class="space-y-3">
                                <li class="flex items-start">
                                    <i class="fas fa-check text-emerald-400 mt-1 mr-2"></i>
                                    <span>Unlimited users</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check text-emerald-400 mt-1 mr-2"></i>
                                    <span>Enterprise-grade automation</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check text-emerald-400 mt-1 mr-2"></i>
                                    <span>All integrations</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check text-emerald-400 mt-1 mr-2"></i>
                                    <span>24/7 dedicated support</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check text-emerald-400 mt-1 mr-2"></i>
                                    <span>Single sign-on (SSO)</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check text-emerald-400 mt-1 mr-2"></i>
                                    <span>Custom AI models</span>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
                
                <div class="mt-16 bg-gray-800 rounded-xl p-8 max-w-4xl mx-auto">
                    <h3 class="text-xl font-bold mb-2 text-center">Still unsure? Try our free plan</h3>
                    <p class="text-gray-400 text-center mb-6">No credit card required. Get started instantly with basic features.</p>
                    <div class="flex justify-center">
                        <button class="px-8 py-3 rounded-lg bg-gradient-to-r from-gray-700 to-gray-600 text-white font-medium hover:opacity-90 transition">
                            Try Free for 14 Days
                        </button>
                    </div>
                </div>
            </div>
        </section>

        <!-- Testimonials Section -->
        <section id="testimonials" class="py-20 px-6 bg-gray-900">
            <div class="container mx-auto">
                <div class="text-center mb-16">
                    <span class="inline-block px-3 py-1 rounded-full bg-gray-800 text-indigo-400 mb-4">TESTIMONIALS</span>
                    <h2 class="text-3xl md:text-4xl font-bold mb-4">What Our <span class="gradient-text">Customers Say</span></h2>
                </div>
                
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 max-w-6xl mx-auto">
                    <!-- Testimonial 1 -->
                    <div class="bg-gray-800 rounded-xl p-8">
                        <div class="mb-6">
                            <h4 class="font-bold">Jamie Wilson</h4>
                            <p class="text-gray-400 text-sm">Music Educator</p>
                        </div>
                        <p class="text-gray-300 mb-6">
                            "Nexus Labs has transformed how our team works. We've automated 75% of our repetitive tasks and gained back hundreds of hours each month."
                        </p>
                        <div class="flex items-center">
                            <i class="fas fa-star text-yellow-400 mr-1"></i>
                            <i class="fas fa-star text-yellow-400 mr-1"></i>
                            <i class="fas fa-star text-yellow-400 mr-1"></i>
                            <i class="fas fa-star text-yellow-400 mr-1"></i>
                            <i class="fas fa-star text-yellow-400"></i>
                        </div>
                    </div>
                    
                    <!-- Testimonial 2 -->
                    <div class="bg-gray-800 rounded-xl p-8">
                        <div class="mb-6">
                            <h4 class="font-bold">Alex Chen</h4>
                            <p class="text-gray-400 text-sm">Session Musician</p>
                        </div>
                        <p class="text-gray-300 mb-6">
                            "The AI-powered analytics alone are worth the price. We're making faster, data-driven decisions across the entire organization."
                        </p>
                        <div class="flex items-center">
                            <i class="fas fa-star text-yellow-400 mr-1"></i>
                            <i class="fas fa-star text-yellow-400 mr-1"></i>
                            <i class="fas fa-star text-yellow-400 mr-1"></i>
                            <i class="fas fa-star text-yellow-400 mr-1"></i>
                            <i class="fas fa-star text-yellow-400"></i>
                        </div>
                    </div>
                    
                    <!-- Testimonial 3 -->
                    <div class="bg-gray-800 rounded-xl p-8">
                        <div class="mb-6">
                            <h4 class="font-bold">Taylor Davis</h4>
                            <p class="text-gray-400 text-sm">Songwriter</p>
                        </div>
                        <p class="text-gray-300 mb-6">
                            "Our productivity skyrocketed after implementing Nexus. The custom workflows let us automate exactly what we need without any coding."
                        </p>
                        <div class="flex items-center">
                            <i class="fas fa-star text-yellow-400 mr-1"></i>
                            <i class="fas fa-star text-yellow-400 mr-1"></i>
                            <i class="fas fa-star text-yellow-400 mr-1"></i>
                            <i class="fas fa-star text-yellow-400 mr-1"></i>
                            <i class="fas fa-star-half-alt text-yellow-400"></i>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- CTA Section -->
        <section class="py-20 px-6 bg-gradient-to-r from-indigo-900 to-emerald-900">
            <div class="container mx-auto text-center">
                <h2 class="text-3xl md:text-4xl font-bold mb-6">Ready to Transform Your <span class="gradient-text">Workflow?</span></h2>
                <p class="text-gray-300 max-w-2xl mx-auto mb-10">
                    Join thousands of businesses that are saving time and boosting productivity with Nexus Labs.
                </p>
                <div class="flex flex-col sm:flex-row justify-center space-y-4 sm:space-y-0 sm:space-x-4">
                    <button class="px-8 py-4 rounded-lg bg-white text-indigo-600 font-bold hover:bg-opacity-90 transition">
                        Get Started Now
                    </button>
                    <button class="px-8 py-4 rounded-lg border-2 border-white text-white font-bold hover:bg-white hover:bg-opacity-10 transition">
                        Schedule Demo
                    </button>
                </div>
            </div>
        </section>
    </main>

    <footer class="bg-gray-900 py-16 px-6">
        <div class="container mx-auto">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-12 mb-16">
                <div>
                    <div class="flex items-center space-x-2 mb-6">
                        <div class="w-8 h-8 rounded-lg bg-gradient-to-r from-indigo-500 to-emerald-500 flex items-center justify-center">
                            <i class="fas fa-bolt text-white"></i>
                        </div>
                        <span class="text-xl font-bold">Nexus <span class="gradient-text">Labs</span></span>
                    </div>
                    <p class="text-gray-400 mb-6">
                        Harnessing AI to empower businesses and unlock human potential.
                    </p>
                    <div class="flex space-x-4">
                        <a href="#" class="w-10 h-10 rounded-full bg-gray-800 flex items-center justify-center hover:bg-indigo-500 transition">
                            <i class="fab fa-twitter"></i>
                        </a>
                        <a href="#" class="w-10 h-10 rounded-full bg-gray-800 flex items-center justify-center hover:bg-indigo-500 transition">
                            <i class="fab fa-linkedin-in"></i>
                        </a>
                        <a href="#" class="w-10 h-10 rounded-full bg-gray-800 flex items-center justify-center hover:bg-indigo-500 transition">
                            <i class="fab fa-github"></i>
                        </a>
                        <a href="#" class="w-10 h-10 rounded-full bg-gray-800 flex items-center justify-center hover:bg-indigo-500 transition">
                            <i class="fab fa-youtube"></i>
                        </a>
                    </div>
                </div>
                
                <div>
                    <h4 class="text-lg font-bold mb-6">Product</h4>
                    <ul class="space-y-3">
                        <li><a href="#" class="text-gray-400 hover:text-indigo-400 transition">Features</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-indigo-400 transition">Pricing</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-indigo-400 transition">Integrations</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-indigo-400 transition">Roadmap</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-indigo-400 transition">Changelog</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="text-lg font-bold mb-6">Resources</h4>
                    <ul class="space-y-3">
                        <li><a href="#" class="text-gray-400 hover:text-indigo-400 transition">Documentation</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-indigo-400 transition">Tutorials</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-indigo-400 transition">Blog</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-indigo-400 transition">Community</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-indigo-400 transition">Webinars</a></li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="text-lg font-bold mb-6">Company</h4>
                    <ul class="space-y-3">
                        <li><a href="#" class="text-gray-400 hover:text-indigo-400 transition">About Us</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-indigo-400 transition">Careers</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-indigo-400 transition">Press</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-indigo-400 transition">Contact</a></li>
                        <li><a href="#" class="text-gray-400 hover:text-indigo-400 transition">Partners</a></li>
                    </ul>
                </div>
            </div>
            
            <div class="pt-8 border-t border-gray-800 flex flex-col md:flex-row justify-between items-center">
                <p class="text-gray-500 text-sm mb-4 md:mb-0">
                    &copy; 2023 Nexus Labs. All rights reserved.
                </p>
                <div class="flex space-x-6">
                    <a href="#" class="text-gray-500 hover:text-indigo-400 text-sm transition">Privacy Policy</a>
                    <a href="#" class="text-gray-500 hover:text-indigo-400 text-sm transition">Terms of Service</a>
                    <a href="#" class="text-gray-500 hover:text-indigo-400 text-sm transition">Cookie Policy</a>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Floating sparkle effect
        document.addEventListener('DOMContentLoaded', function() {
            document.body.addEventListener('mousemove', function(e) {
                const sparkle = document.createElement('div');
                sparkle.className = 'sparkle';
                sparkle.style.left = e.clientX + 'px';
                sparkle.style.top = e.clientY + 'px';
                
                const size = Math.random() * 10 + 5;
                sparkle.style.width = size + 'px';
                sparkle.style.height = size + 'px';
                
                document.body.appendChild(sparkle);
                
                setTimeout(() => {
                    sparkle.style.opacity = '0';
                    sparkle.style.transform = 'translate(-50%, -50%) scale(2)';
                }, 50);
                
                setTimeout(() => {
                    sparkle.remove();
                }, 500);
            });
            
            // Smooth scroll for anchor links
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function(e) {
                    e.preventDefault();
                    document.querySelector(this.getAttribute('href')).scrollIntoView({
                        behavior: 'smooth'
                    });
                });
            });
            
            // Mobile menu toggle functionality
            const mobileMenuButton = document.querySelector('.md\\:hidden button');
            const mobileMenu = document.createElement('div');
            mobileMenu.className = 'fixed inset-0 bg-gray-900 bg-opacity-95 z-50 flex flex-col items-center justify-center hidden';
            mobileMenu.innerHTML = `
                <button class="absolute top-6 right-6 text-3xl">
                    <i class="fas fa-times"></i>
                </button>
                <nav class="flex flex-col items-center space-y-8 text-2xl">
                    <a href="#features" class="hover:text-indigo-400 transition">Features</a>
                    <a href="#solutions" class="hover:text-indigo-400 transition">Solutions</a>
                    <a href="#pricing" class="hover:text-indigo-400 transition">Pricing</a>
                    <a href="#testimonials" class="hover:text-indigo-400 transition">Testimonials</a>
                    <button class="mt-8 px-8 py-3 rounded-lg bg-gradient-to-r from-indigo-500 to-emerald-500 text-white font-medium hover:opacity-90 transition">
                        Get Started
                    </button>
                </nav>
            `;
            document.body.appendChild(mobileMenu);
            
            mobileMenuButton.addEventListener('click', function() {
                mobileMenu.classList.remove('hidden');
                document.body.style.overflow = 'hidden';
            });
            
            mobileMenu.querySelector('button').addEventListener('click', function() {
                mobileMenu.classList.add('hidden');
                document.body.style.overflow = '';
            });
            
            // Animation intersection observer
            const animateOnScroll = function() {
                const elements = document.querySelectorAll('.feature-card, .gradient-border');
                
                const observer = new IntersectionObserver((entries) => {
                    entries.forEach(entry => {
                        if (entry.isIntersecting) {
                            entry.target.classList.add('animate__animated', 'animate__fadeInUp');
                            observer.unobserve(entry.target);
                        }
                    });
                }, { threshold: 0.1 });
                
                elements.forEach(element => {
                    observer.observe(element);
                });
            };
            
            animateOnScroll();
        });
    </script>
</body>
</html>

