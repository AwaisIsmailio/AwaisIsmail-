<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Join My Team – Back-End Assistant Needed</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&family=Montserrat:wght@700;800&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #4361ee;
            --secondary: #3f37c9;
            --accent: #4cc9f0;
            --light: #f8f9fa;
            --dark: #212529;
            --success: #4ade80;
            --gray: #6c757d;
            --light-gray: #e9ecef;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(135deg, #f5f7fa 0%, #e4edf5 100%);
            color: var(--dark);
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        section {
            padding: 80px 0;
        }
        
        h1, h2, h3 {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            line-height: 1.2;
        }
        
        h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            letter-spacing: -0.5px;
        }
        
        h2 {
            font-size: 2.5rem;
            margin-bottom: 40px;
            position: relative;
            display: inline-block;
        }
        
        h2::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 70px;
            height: 4px;
            background: var(--accent);
            border-radius: 2px;
        }
        
        .subheading {
            font-size: 1.5rem;
            color: var(--gray);
            margin-bottom: 30px;
            max-width: 700px;
        }
        
        .btn {
            display: inline-block;
            background: var(--primary);
            color: white;
            padding: 15px 35px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(67, 97, 238, 0.3);
            border: none;
            cursor: pointer;
        }
        
        .btn:hover {
            background: var(--secondary);
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(67, 97, 238, 0.4);
        }
        
        .btn-whatsapp {
            background: #25D366;
            box-shadow: 0 4px 15px rgba(37, 211, 102, 0.3);
        }
        
        .btn-whatsapp:hover {
            background: #128C7E;
            box-shadow: 0 6px 20px rgba(37, 211, 102, 0.4);
        }
        
        .card {
            background: white;
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.1);
        }
        
        .icon-box {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 70px;
            height: 70px;
            background: rgba(67, 97, 238, 0.1);
            border-radius: 18px;
            margin-bottom: 25px;
        }
        
        .icon-box i {
            font-size: 30px;
            color: var(--primary);
        }
        
        ul {
            list-style: none;
            padding-left: 0;
        }
        
        ul li {
            margin-bottom: 15px;
            padding-left: 30px;
            position: relative;
        }
        
        ul li::before {
            content: '\f00c';
            font-family: 'Font Awesome 6 Free';
            font-weight: 900;
            position: absolute;
            left: 0;
            top: 2px;
            color: var(--success);
        }
        
        .feature-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .feature-item {
            display: flex;
            align-items: flex-start;
            gap: 20px;
        }
        
        .feature-icon {
            flex-shrink: 0;
            width: 60px;
            height: 60px;
            background: rgba(67, 97, 238, 0.1);
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .feature-icon i {
            font-size: 24px;
            color: var(--primary);
        }
        
        .contact-box {
            background: white;
            border-radius: 20px;
            padding: 50px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
            max-width: 700px;
            margin: 0 auto;
        }
        
        .contact-box h2 {
            margin-bottom: 20px;
        }
        
        .contact-box p {
            margin-bottom: 30px;
            font-size: 1.1rem;
            color: var(--gray);
        }
        
        footer {
            background: var(--dark);
            color: white;
            padding: 30px 0;
            text-align: center;
        }
        
        .social-icons {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }
        
        .social-icons a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 45px;
            height: 45px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            color: white;
            font-size: 18px;
            transition: all 0.3s ease;
        }
        
        .social-icons a:hover {
            background: var(--primary);
            transform: translateY(-3px);
        }
        
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            position: relative;
            overflow: hidden;
            padding-top: 80px;
        }
        
        .hero-content {
            position: relative;
            z-index: 2;
            max-width: 700px;
        }
        
        .hero-bg {
            position: absolute;
            top: 0;
            right: 0;
            height: 100%;
            width: 50%;
            background: linear-gradient(135deg, rgba(67, 97, 238, 0.1) 0%, rgba(63, 55, 201, 0.1) 100%);
            border-bottom-left-radius: 50%;
            z-index: 1;
        }
        
        .work-details {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .detail-card {
            background: white;
            border-radius: 15px;
            padding: 30px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .detail-card i {
            font-size: 40px;
            color: var(--primary);
            margin-bottom: 20px;
        }
        
        /* Animation Classes */
        .animate-on-scroll {
            opacity: 0;
            transform: translateY(30px);
            transition: opacity 0.6s ease, transform 0.6s ease;
        }
        
        .animate-on-scroll.visible {
            opacity: 1;
            transform: translateY(0);
        }
        
        /* Mobile Styles */
        @media (max-width: 768px) {
            h1 {
                font-size: 2.5rem;
            }
            
            h2 {
                font-size: 2rem;
            }
            
            .subheading {
                font-size: 1.2rem;
            }
            
            section {
                padding: 60px 0;
            }
            
            .hero {
                min-height: auto;
                padding: 100px 0 60px;
            }
            
            .hero-bg {
                width: 100%;
                border-radius: 0 0 50% 50%;
            }
            
            .contact-box {
                padding: 30px;
            }
            
            .card {
                padding: 30px;
            }
        }
        
        @media (max-width: 480px) {
            h1 {
                font-size: 2rem;
            }
            
            h2 {
                font-size: 1.8rem;
            }
            
            .btn {
                padding: 12px 25px;
                font-size: 1rem;
            }
            
            .feature-grid {
                grid-template-columns: 1fr;
            }
            
            .work-details {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <div class="hero-content animate-on-scroll">
                <h1>Work With Me on Real AI Projects</h1>
                <p class="subheading">Looking for a reliable back-end assistant to manage files, design, and digital tasks.</p>
                <a href="https://wa.me/923293209581?text=Hi%20👋%20I'm%20interested%20in%20the%20Back-End%20Assistant%20job!" class="btn btn-whatsapp">
                    <i class="fab fa-whatsapp"></i> Apply Now
                </a>
            </div>
        </div>
        <div class="hero-bg"></div>
    </section>

    <!-- About the Role -->
    <section>
        <div class="container">
            <div class="card animate-on-scroll">
                <div class="icon-box">
                    <i class="fas fa-briefcase"></i>
                </div>
                <h2>About the Role</h2>
                <p>I'm looking for a dedicated Back-End Assistant to join my team and help manage various digital operations. This role involves handling Google Drive organization, creating visual content, managing social media platforms, and assisting with website updates.</p>
                <p>You'll be working directly with me on exciting AI-related projects, helping to streamline operations and ensure everything runs smoothly behind the scenes. This is a great opportunity for someone who enjoys variety in their work and wants to grow their digital skills.</p>
            </div>
        </div>
    </section>

    <!-- Responsibilities -->
    <section>
        <div class="container">
            <h2 class="animate-on-scroll">Key Responsibilities</h2>
            <p class="subheading animate-on-scroll">Your day-to-day tasks will include:</p>
            
            <div class="feature-grid">
                <div class="feature-item animate-on-scroll">
                    <div class="feature-icon">
                        <i class="fab fa-google-drive"></i>
                    </div>
                    <div>
                        <h3>Manage Google Drive Files</h3>
                        <p>Organize and maintain files in Google Drive, ensuring everything is properly categorized and easily accessible.</p>
                    </div>
                </div>
                
                <div class="feature-item animate-on-scroll">
                    <div class="feature-icon">
                        <i class="fas fa-heading"></i>
                    </div>
                    <div>
                        <h3>Write Titles & Descriptions</h3>
                        <p>Create compelling titles and descriptions for various content pieces and projects.</p>
                    </div>
                </div>
                
                <div class="feature-item animate-on-scroll">
                    <div class="feature-icon">
                        <i class="fas fa-palette"></i>
                    </div>
                    <div>
                        <h3>Design Posters in Canva</h3>
                        <p>Create visually appealing posters and graphics using Canva for promotions and announcements.</p>
                    </div>
                </div>
                
                <div class="feature-item animate-on-scroll">
                    <div class="feature-icon">
                        <i class="fab fa-whatsapp"></i>
                    </div>
                    <div>
                        <h3>Post to WhatsApp & Instagram</h3>
                        <p>Manage and schedule posts across WhatsApp and Instagram platforms.</p>
                    </div>
                </div>
                
                <div class="feature-item animate-on-scroll">
                    <div class="feature-icon">
                        <i class="fas fa-code"></i>
                    </div>
                    <div>
                        <h3>Create Course Pages</h3>
                        <p>Set up and maintain course pages on the website with provided content.</p>
                    </div>
                </div>
                
                <div class="feature-item animate-on-scroll">
                    <div class="feature-icon">
                        <i class="fas fa-sync-alt"></i>
                    </div>
                    <div>
                        <h3>Process Management</h3>
                        <p>Follow and repeat established processes for each new project or content piece.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Requirements -->
    <section>
        <div class="container">
            <div class="card animate-on-scroll">
                <div class="icon-box">
                    <i class="fas fa-user-check"></i>
                </div>
                <h2>Requirements</h2>
                <p>We're looking for someone with the following qualifications:</p>
                
                <ul>
                    <li>Basic mobile and laptop operation skills</li>
                    <li>Familiarity with Google Drive, Canva, and Instagram</li>
                    <li>Reliable and responsive communication style</li>
                    <li>Willingness to learn new tools and processes</li>
                    <li>Good organizational skills and attention to detail</li>
                    <li>Ability to follow instructions precisely</li>
                    <li>Positive attitude and team spirit</li>
                </ul>
                
                <p style="margin-top: 20px; font-style: italic;">Don't worry if you're not an expert in all areas - training will be provided for the right candidate!</p>
            </div>
        </div>
    </section>

    <!-- Work Details -->
    <section>
        <div class="container">
            <h2 class="animate-on-scroll">Work Details</h2>
            <p class="subheading animate-on-scroll">Here's what you need to know about the position:</p>
            
            <div class="work-details">
                <div class="detail-card animate-on-scroll">
                    <i class="fas fa-map-marker-alt"></i>
                    <h3>Location</h3>
                    <p>Badin preferred (Remote work available)</p>
                </div>
                
                <div class="detail-card animate-on-scroll">
                    <i class="fas fa-calendar-alt"></i>
                    <h3>Schedule</h3>
                    <p>Flexible hours, part-time commitment</p>
                </div>
                
                <div class="detail-card animate-on-scroll">
                    <i class="fas fa-money-bill-wave"></i>
                    <h3>Payment</h3>
                    <p>Monthly payments</p>
                </div>
                
                <div class="detail-card animate-on-scroll">
                    <i class="fas fa-laptop-house"></i>
                    <h3>Work Environment</h3>
                    <p>Fully remote position</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section>
        <div class="container">
            <div class="contact-box animate-on-scroll">
                <h2>Ready to Join the Team?</h2>
                <p>If you're excited about this opportunity and believe you'd be a good fit, apply now via WhatsApp. Let's discuss how you can contribute to our exciting projects!</p>
                <a href="https://wa.me/923293209581?text=Hi%20👋%20I'm%20interested%20in%20the%20Back-End%20Assistant%20job!" class="btn btn-whatsapp">
                    <i class="fab fa-whatsapp"></i> Apply on WhatsApp
                </a>
                <p style="margin-top: 20px; font-size: 1rem;">
                    <i class="fas fa-phone-alt"></i> WhatsApp: +92 329 3209581
                </p>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>Powered by Awais Ismail</p>
            <div class="social-icons">
                <a href="#"><i class="fab fa-facebook-f"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-linkedin-in"></i></a>
            </div>
            <p style="margin-top: 20px; font-size: 0.9rem; opacity: 0.7;">&copy; 2023 All Rights Reserved</p>
        </div>
    </footer>

    <script>
        // Animation on scroll
        document.addEventListener('DOMContentLoaded', function() {
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('visible');
                    }
                });
            }, {
                threshold: 0.1
            });
            
            document.querySelectorAll('.animate-on-scroll').forEach(el => {
                observer.observe(el);
            });
        });
    </script>
</body>
</html>
