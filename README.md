<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Transform Your LinkedIn Presence | LinkedIn Strategy Expert</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            color: #333;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header Section */
        .hero {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            margin: 40px auto;
            padding: 60px 40px;
            text-align: center;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
            animation: fadeInUp 0.8s ease-out;
        }

        .hero h1 {
            font-size: 3.5rem;
            font-weight: 800;
            color: #1a1a1a;
            margin-bottom: 20px;
            line-height: 1.2;
        }

        .hero p {
            font-size: 1.3rem;
            color: #666;
            margin-bottom: 40px;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        .cta-button {
            background: linear-gradient(45deg, #4facfe, #00f2fe);
            color: white;
            padding: 18px 40px;
            border: none;
            border-radius: 50px;
            font-size: 1.2rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            display: inline-block;
            box-shadow: 0 10px 30px rgba(79, 172, 254, 0.3);
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 15px 40px rgba(79, 172, 254, 0.4);
        }

        /* Services Section */
        .services {
            background: white;
            border-radius: 20px;
            padding: 60px 40px;
            margin: 40px auto;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
            animation: fadeInUp 0.8s ease-out 0.2s both;
        }

        .services h2 {
            text-align: center;
            font-size: 2.5rem;
            color: #1a1a1a;
            margin-bottom: 50px;
            font-weight: 700;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 30px;
            margin-bottom: 40px;
        }

        .service-card {
            background: #f8f9ff;
            padding: 40px 30px;
            border-radius: 15px;
            text-align: left;
            transition: all 0.3s ease;
            border: 2px solid transparent;
            position: relative;
            overflow: hidden;
        }

        .service-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(45deg, #4facfe, #00f2fe);
            transform: scaleX(0);
            transition: transform 0.3s ease;
        }

        .service-card:hover::before {
            transform: scaleX(1);
        }

        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
        }

        .service-icon {
            width: 60px;
            height: 60px;
            background: linear-gradient(45deg, #4facfe, #00f2fe);
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 20px;
            font-size: 24px;
            color: white;
        }

        .service-card h3 {
            font-size: 1.5rem;
            color: #1a1a1a;
            margin-bottom: 15px;
            font-weight: 600;
        }

        .service-card p {
            color: #666;
            font-size: 1.1rem;
            line-height: 1.6;
        }

        /* About Section */
        .about {
            background: white;
            border-radius: 20px;
            padding: 60px 40px;
            margin: 40px auto;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
            animation: fadeInUp 0.8s ease-out 0.4s both;
        }

        .about-content {
            display: grid;
            grid-template-columns: 2fr 1fr;
            gap: 50px;
            align-items: center;
        }

        .about h2 {
            font-size: 2.5rem;
            color: #1a1a1a;
            margin-bottom: 20px;
            font-weight: 700;
        }

        .about p {
            font-size: 1.2rem;
            color: #666;
            line-height: 1.7;
        }

        .profile-image {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            object-fit: cover;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease;
        }

        .profile-image:hover {
            transform: scale(1.05);
        }

        /* Contact Section */
        .contact {
            background: white;
            border-radius: 20px;
            padding: 60px 40px;
            margin: 40px auto;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
            animation: fadeInUp 0.8s ease-out 0.6s both;
        }

        .contact h2 {
            text-align: center;
            font-size: 2.5rem;
            color: #1a1a1a;
            margin-bottom: 20px;
            font-weight: 700;
        }

        .contact-subtitle {
            text-align: center;
            font-size: 1.2rem;
            color: #666;
            margin-bottom: 50px;
        }

        .contact-form {
            max-width: 600px;
            margin: 0 auto;
        }

        .form-row {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            margin-bottom: 20px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 18px 20px;
            border: 2px solid #e0e0e0;
            border-radius: 12px;
            font-size: 1.1rem;
            transition: all 0.3s ease;
            background: #f8f9ff;
        }

        .form-group input:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: #4facfe;
            box-shadow: 0 0 0 3px rgba(79, 172, 254, 0.1);
            background: white;
        }

        .form-group textarea {
            height: 120px;
            resize: vertical;
        }

        .submit-btn {
            background: linear-gradient(45deg, #4facfe, #00f2fe);
            color: white;
            padding: 18px 40px;
            border: none;
            border-radius: 50px;
            font-size: 1.2rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            width: 100%;
            box-shadow: 0 10px 30px rgba(79, 172, 254, 0.3);
        }

        .submit-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 15px 40px rgba(79, 172, 254, 0.4);
        }

        /* Footer */
        .footer {
            text-align: center;
            padding: 40px 20px;
            color: white;
            font-size: 1.1rem;
        }

        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.5rem;
            }

            .hero p {
                font-size: 1.1rem;
            }

            .services-grid {
                grid-template-columns: 1fr;
            }

            .about-content {
                grid-template-columns: 1fr;
                text-align: center;
            }

            .form-row {
                grid-template-columns: 1fr;
            }

            .hero,
            .services,
            .about,
            .contact {
                padding: 40px 20px;
                margin: 20px auto;
            }
        }

        @media (max-width: 480px) {
            .hero h1 {
                font-size: 2rem;
            }

            .services h2,
            .about h2,
            .contact h2 {
                font-size: 2rem;
            }
        }

        /* Success Message Styles */
        .success-message {
            background: #d4edda;
            color: #155724;
            padding: 15px 20px;
            border-radius: 8px;
            margin-bottom: 20px;
            border: 1px solid #c3e6cb;
            display: none;
        }

        .success-message.show {
            display: block;
            animation: fadeInUp 0.5s ease-out;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Hero Section -->
        <section class="hero">
            <h1>Transform Your LinkedIn Presence</h1>
            <p>Grow your brand, boost engagement & unlock new opportunities through proven LinkedIn strategies.</p>
            <a href="#contact" class="cta-button">Book a Free Call</a>
        </section>

        <!-- Services Section -->
        <section class="services">
            <h2>My Services</h2>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">💎</div>
                    <h3>Personal Branding</h3>
                    <p>We craft your unique voice & identity on LinkedIn to make you stand out from the crowd and establish thought leadership.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🚀</div>
                    <h3>Boosting Engagement</h3>
                    <p>Increase likes, comments, and shares with proven strategies that spark meaningful conversations with your audience.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">✏️</div>
                    <h3>Content Creation</h3>
                    <p>Viral posts, carousel designs, and strategic content that resonates with your target audience and drives results.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">🤝</div>
                    <h3>Product/Brand Collaboration</h3>
                    <p>Connect with brands and create partnership opportunities that align with your personal brand and values.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">📊</div>
                    <h3>Marketing Strategy</h3>
                    <p>Comprehensive LinkedIn marketing plans that convert your network into business opportunities and leads.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">📈</div>
                    <h3>LinkedIn Growth & Management</h3>
                    <p>Complete handle management and organic growth strategies to build your professional network and influence.</p>
                </div>
            </div>
        </section>

        <!-- About Section -->
        <section class="about">
            <div class="about-content">
                <div>
                    <h2>Meet Your LinkedIn Strategist</h2>
                    <p>I'm a social media expert with 5+ years of experience managing personal brands and building authority on LinkedIn. I've helped hundreds of professionals transform their LinkedIn presence and unlock new opportunities. Let's grow your presence together and establish you as a thought leader in your industry.</p>
                </div>
                <div style="text-align: center;">
                    <img src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1000&q=80" alt="LinkedIn Strategist" class="profile-image">
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section class="contact" id="contact">
            <h2>Let's Get You Noticed on LinkedIn</h2>
            <p class="contact-subtitle">Fill out the form or message me directly on LinkedIn to get started</p>
            
            <form class="contact-form" id="contactForm">
                <div id="successMessage" class="success-message">
                    Thanks for your message! I'll get back to you within 24 hours.
                </div>
                
                <div class="form-row">
                    <div class="form-group">
                        <input type="text" id="name" name="name" placeholder="Your Name" required>
                    </div>
                    <div class="form-group">
                        <input type="email" id="email" name="email" placeholder="Email" required>
                    </div>
                </div>
                
                <div class="form-group">
                    <textarea id="message" name="message" placeholder="How can I help you grow your LinkedIn presence?" required></textarea>
                </div>
                
                <button type="submit" class="submit-btn">Send Message</button>
            </form>
        </section>
    </div>

    <!-- Footer -->
    <footer class="footer">
        <p>&copy; 2025 LinkedIn Strategy Expert. All rights reserved. | Transform your professional presence today.</p>
    </footer>

    <script>
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Form submission handling
        document.getElementById('contactForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Get form data
            const formData = new FormData(this);
            const name = formData.get('name');
            const email = formData.get('email');
            const message = formData.get('message');
            
            // Simulate form submission (in real implementation, this would send to a server)
            setTimeout(() => {
                // Show success message
                const successMessage = document.getElementById('successMessage');
                successMessage.classList.add('show');
                
                // Reset form
                this.reset();
                
                // Hide success message after 5 seconds
                setTimeout(() => {
                    successMessage.classList.remove('show');
                }, 5000);
            }, 500);
        });

        // Add scroll animation trigger
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.animationPlayState = 'running';
                }
            });
        }, observerOptions);

        // Observe all animated elements
        document.querySelectorAll('.hero, .services, .about, .contact').forEach(el => {
            observer.observe(el);
        });

        // Add hover effects to service cards
        document.querySelectorAll('.service-card').forEach(card => {
            card.addEventListener('mouseenter', function() {
                this.style.transform = 'translateY(-10px) scale(1.02)';
            });
            
            card.addEventListener('mouseleave', function() {
                this.style.transform = 'translateY(0) scale(1)';
            });
        });

        // Add dynamic gradient background
        let gradientAngle = 135;
        setInterval(() => {
            gradientAngle += 0.5;
            document.body.style.background = `linear-gradient(${gradientAngle}deg, #667eea 0%, #764ba2 100%)`;
        }, 100);
    </script>
</body>
</html>
