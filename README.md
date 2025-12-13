<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mateor Labs (Pvt) Ltd | Technology Solutions for the Digital Age</title>
    <meta name="description" content="Leading technology solutions provider offering innovative software deployment, network configuration, and ICT equipment solutions. Digital transformation specialists since 2021.">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* CSS Variables - Professional Tech Theme */
        :root {
            --primary: #000000;
            --secondary: #1a1a1a;
            --accent: #0077ff;
            --accent-light: #3399ff;
            --text: #333333;
            --text-light: #666666;
            --background: #ffffff;
            --background-alt: #f8f9fa;
            --card-bg: #ffffff;
            --border: #e0e0e0;
            --shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
            --shadow-hover: 0 8px 24px rgba(0, 0, 0, 0.12);
            --transition: all 0.3s cubic-bezier(0.25, 0.46, 0.45, 0.94);
            --border-radius: 8px;
            --container-width: 1200px;
        }

        /* Reset & Base */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, sans-serif;
            line-height: 1.6;
            color: var(--text);
            background-color: var(--background);
            overflow-x: hidden;
        }

        h1, h2, h3, h4, h5 {
            font-weight: 700;
            line-height: 1.2;
            margin-bottom: 1rem;
            color: var(--primary);
        }

        p {
            margin-bottom: 1.2rem;
            color: var(--text-light);
        }

        a {
            text-decoration: none;
            color: inherit;
            transition: var(--transition);
        }

        ul {
            list-style: none;
        }

        img {
            max-width: 100%;
            height: auto;
        }

        .container {
            width: 100%;
            max-width: var(--container-width);
            margin: 0 auto;
            padding: 0 20px;
        }

        .section {
            padding: 100px 0;
        }

        .section-header {
            text-align: center;
            margin-bottom: 60px;
        }

        .section-title {
            font-size: 2.5rem;
            position: relative;
            display: inline-block;
            margin-bottom: 15px;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 60px;
            height: 3px;
            background-color: var(--accent);
        }

        .section-subtitle {
            font-size: 1.1rem;
            color: var(--text-light);
            max-width: 700px;
            margin: 0 auto;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            padding: 14px 32px;
            border-radius: var(--border-radius);
            font-weight: 600;
            font-size: 0.95rem;
            text-transform: uppercase;
            letter-spacing: 0.5px;
            transition: var(--transition);
            border: none;
            cursor: pointer;
            gap: 8px;
        }

        .btn-primary {
            background-color: var(--accent);
            color: white;
        }

        .btn-primary:hover {
            background-color: var(--accent-light);
            transform: translateY(-2px);
            box-shadow: var(--shadow-hover);
        }

        .btn-outline {
            background-color: transparent;
            color: var(--accent);
            border: 2px solid var(--accent);
        }

        .btn-outline:hover {
            background-color: var(--accent);
            color: white;
            transform: translateY(-2px);
        }

        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        .fade-in-up {
            animation: fadeInUp 0.8s ease forwards;
        }

        .fade-in {
            animation: fadeIn 0.8s ease forwards;
        }

        /* Header */
        .header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background-color: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            z-index: 1000;
            box-shadow: 0 2px 20px rgba(0, 0, 0, 0.05);
            padding: 15px 0;
            transition: var(--transition);
        }

        .header.scrolled {
            padding: 10px 0;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.1);
        }

        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            align-items: center;
            font-weight: 700;
            font-size: 1.8rem;
            color: var(--primary);
            height: 60px;
        }

        .logo img {
            height: 100%;
            width: auto;
        }

        .nav {
            display: flex;
            align-items: center;
        }

        .nav-list {
            display: flex;
        }

        .nav-item {
            margin-left: 35px;
        }

        .nav-link {
            font-weight: 600;
            font-size: 0.95rem;
            position: relative;
            padding: 5px 0;
        }

        .nav-link::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 2px;
            background-color: var(--accent);
            transition: var(--transition);
        }

        .nav-link:hover {
            color: var(--accent);
        }

        .nav-link:hover::after {
            width: 100%;
        }

        .mobile-menu-toggle {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            color: var(--primary);
            cursor: pointer;
        }

        /* Hero */
        .hero {
            padding-top: 160px;
            padding-bottom: 100px;
            background: linear-gradient(135deg, var(--secondary) 0%, var(--primary) 100%);
            color: white;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: url('https://images.unsplash.com/photo-1518709268805-4e9042af2176?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80') center/cover no-repeat;
            opacity: 0.2;
            filter: grayscale(100%);
        }

        .hero-container {
            position: relative;
            z-index: 1;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            align-items: center;
        }

        .hero-content h1 {
            font-size: 3.2rem;
            color: white;
            margin-bottom: 1.5rem;
            line-height: 1.1;
        }

        .hero-content p {
            font-size: 1.2rem;
            color: rgba(255, 255, 255, 0.85);
            margin-bottom: 2.5rem;
            max-width: 500px;
        }

        .hero-stats {
            display: flex;
            gap: 40px;
            margin-top: 3rem;
        }

        .stat-item {
            text-align: center;
        }

        .stat-number {
            font-size: 2.5rem;
            font-weight: 700;
            color: white;
            margin-bottom: 5px;
        }

        .stat-label {
            font-size: 0.9rem;
            color: rgba(255, 255, 255, 0.7);
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .hero-visual {
            position: relative;
        }

        .hero-image {
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--shadow-hover);
            transform: perspective(1000px) rotateY(-10deg);
            transition: var(--transition);
        }

        .hero-image:hover {
            transform: perspective(1000px) rotateY(0deg);
        }

        .hero-image img {
            width: 100%;
            height: 400px;
            object-fit: cover;
            filter: grayscale(30%);
            transition: var(--transition);
        }

        .hero-image:hover img {
            filter: grayscale(0%);
        }

        /* Services */
        .services {
            background-color: var(--background-alt);
        }

        .services-tabs {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 15px;
            margin-bottom: 50px;
        }

        .tab-btn {
            background-color: white;
            border: 2px solid var(--border);
            padding: 14px 28px;
            border-radius: 50px;
            font-weight: 600;
            font-size: 0.95rem;
            cursor: pointer;
            transition: var(--transition);
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .tab-btn.active {
            background-color: var(--accent);
            color: white;
            border-color: var(--accent);
        }

        .tab-btn:hover:not(.active) {
            border-color: var(--accent);
            color: var(--accent);
        }

        .services-content {
            display: none;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            align-items: center;
        }

        .services-content.active {
            display: grid;
            animation: fadeInUp 0.6s ease forwards;
        }

        .service-image {
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--shadow);
        }

        .service-image img {
            width: 100%;
            height: 350px;
            object-fit: cover;
            transition: var(--transition);
            filter: grayscale(100%);
        }

        .service-image:hover img {
            filter: grayscale(0%);
            transform: scale(1.03);
        }

        .service-details h3 {
            font-size: 2rem;
            margin-bottom: 1.5rem;
        }

        .service-features {
            margin-top: 1.5rem;
        }

        .service-feature {
            display: flex;
            align-items: flex-start;
            margin-bottom: 15px;
        }

        .service-feature i {
            color: var(--accent);
            margin-right: 12px;
            margin-top: 3px;
            font-size: 1.1rem;
        }

        /* Partners */
        .partners-container {
            max-width: 1000px;
            margin: 0 auto;
        }

        .partners-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }

        .partner-card {
            background-color: var(--card-bg);
            border-radius: var(--border-radius);
            padding: 40px 30px;
            text-align: center;
            box-shadow: var(--shadow);
            transition: var(--transition);
            border: 1px solid var(--border);
        }

        .partner-card:hover {
            transform: translateY(-10px);
            box-shadow: var(--shadow-hover);
            border-color: var(--accent);
        }

        .partner-logo {
            height: 80px;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 25px;
            filter: grayscale(100%);
            opacity: 0.8;
            transition: var(--transition);
        }

        .partner-card:hover .partner-logo {
            filter: grayscale(0%);
            opacity: 1;
        }

        .partner-name {
            font-size: 1.3rem;
            font-weight: 700;
            margin-bottom: 10px;
        }

        .partner-description {
            font-size: 0.95rem;
            color: var(--text-light);
        }

        /* Portfolio */
        .portfolio {
            background-color: var(--background-alt);
        }

        .portfolio-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
            gap: 30px;
        }

        .portfolio-item {
            background-color: var(--card-bg);
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition);
            position: relative;
        }

        .portfolio-item:hover {
            transform: translateY(-10px);
            box-shadow: var(--shadow-hover);
        }

        .portfolio-image {
            height: 250px;
            overflow: hidden;
        }

        .portfolio-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: var(--transition);
            filter: grayscale(100%);
        }

        .portfolio-item:hover .portfolio-image img {
            filter: grayscale(0%);
            transform: scale(1.05);
        }

        .portfolio-content {
            padding: 25px;
        }

        .portfolio-content h3 {
            font-size: 1.4rem;
            margin-bottom: 10px;
        }

        .portfolio-content p {
            font-size: 0.95rem;
            margin-bottom: 20px;
        }

        .portfolio-tech {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-top: 15px;
        }

        .tech-tag {
            background-color: rgba(0, 119, 255, 0.1);
            color: var(--accent);
            padding: 5px 12px;
            border-radius: 50px;
            font-size: 0.8rem;
            font-weight: 600;
        }

        /* About */
        .about-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            align-items: center;
        }

        .about-content h2 {
            font-size: 2.2rem;
            margin-bottom: 1.5rem;
        }

        .about-highlights {
            margin-top: 30px;
        }

        .highlight {
            display: flex;
            align-items: flex-start;
            margin-bottom: 25px;
        }

        .highlight-icon {
            background-color: rgba(0, 119, 255, 0.1);
            color: var(--accent);
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 15px;
            flex-shrink: 0;
            font-size: 1.2rem;
        }

        .about-visual {
            position: relative;
        }

        .about-image {
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--shadow);
        }

        .about-image img {
            width: 100%;
            height: 400px;
            object-fit: cover;
        }

        /* Contact */
        .contact {
            background-color: var(--secondary);
            color: white;
        }

        .contact .section-title,
        .contact .section-subtitle {
            color: white;
        }

        .contact .section-subtitle {
            opacity: 0.8;
        }

        .contact-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
        }

        .contact-info h3 {
            color: white;
            font-size: 1.8rem;
            margin-bottom: 1.5rem;
        }

        .contact-details {
            margin-top: 30px;
        }

        .contact-item {
            display: flex;
            align-items: flex-start;
            margin-bottom: 25px;
        }

        .contact-icon {
            background-color: rgba(255, 255, 255, 0.1);
            color: white;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 15px;
            flex-shrink: 0;
            font-size: 1.2rem;
        }

        .contact-text h4 {
            color: white;
            font-size: 1.1rem;
            margin-bottom: 5px;
        }

        .contact-text p {
            color: rgba(255, 255, 255, 0.7);
        }

        .contact-form {
            background-color: rgba(255, 255, 255, 0.05);
            border-radius: var(--border-radius);
            padding: 40px;
            backdrop-filter: blur(10px);
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-control {
            width: 100%;
            padding: 15px;
            border-radius: var(--border-radius);
            border: 1px solid rgba(255, 255, 255, 0.2);
            background-color: rgba(255, 255, 255, 0.05);
            color: white;
            font-family: inherit;
            font-size: 1rem;
            transition: var(--transition);
        }

        .form-control:focus {
            outline: none;
            border-color: var(--accent);
        }

        .form-control::placeholder {
            color: rgba(255, 255, 255, 0.5);
        }

        textarea.form-control {
            min-height: 150px;
            resize: vertical;
        }

        /* Footer */
        .footer {
            background-color: var(--primary);
            color: white;
            padding: 70px 0 30px;
        }

        .footer-container {
            display: grid;
            grid-template-columns: 2fr 1fr 1fr;
            gap: 50px;
            margin-bottom: 50px;
        }

        .footer-about .logo {
            color: white;
            margin-bottom: 20px;
        }

        .footer-about p {
            color: rgba(255, 255, 255, 0.7);
            max-width: 400px;
        }

        .footer-links h3,
        .footer-contact h3 {
            color: white;
            font-size: 1.2rem;
            margin-bottom: 25px;
            position: relative;
            padding-bottom: 10px;
        }

        .footer-links h3::after,
        .footer-contact h3::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 40px;
            height: 2px;
            background-color: var(--accent);
        }

        .footer-links ul li {
            margin-bottom: 12px;
        }

        .footer-links a {
            color: rgba(255, 255, 255, 0.7);
        }

        .footer-links a:hover {
            color: var(--accent);
            padding-left: 5px;
        }

        .footer-contact p {
            color: rgba(255, 255, 255, 0.7);
            margin-bottom: 15px;
            display: flex;
            align-items: flex-start;
        }

        .footer-contact i {
            margin-right: 10px;
            color: var(--accent);
            margin-top: 3px;
        }

        .footer-bottom {
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            padding-top: 30px;
            text-align: center;
        }

        .footer-bottom p {
            color: rgba(255, 255, 255, 0.6);
            font-size: 0.9rem;
        }

        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }

        .social-link {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background-color: rgba(255, 255, 255, 0.1);
            color: white;
            transition: var(--transition);
        }

        .social-link:hover {
            background-color: var(--accent);
            transform: translateY(-3px);
        }

        /* Logo Styling */
        .logo-placeholder {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            text-align: center;
            font-weight: bold;
            color: var(--primary);
        }

        .logo-main {
            font-size: 2.2rem;
            line-height: 1;
            letter-spacing: 1px;
        }

        .logo-subtitle {
            font-size: 0.9rem;
            color: var(--accent);
            letter-spacing: 2px;
            margin-top: 5px;
            font-weight: 600;
        }

        .logo-tagline {
            font-size: 0.7rem;
            color: var(--text-light);
            letter-spacing: 1px;
            margin-top: 2px;
            font-weight: 500;
        }

        .logo-year {
            font-size: 0.6rem;
            color: var(--text-light);
            letter-spacing: 1px;
            margin-top: 3px;
            font-weight: 400;
        }

        /* Responsive */
        @media (max-width: 992px) {
            .hero-container,
            .about-container,
            .contact-container,
            .services-content {
                grid-template-columns: 1fr;
            }
            
            .hero {
                padding-top: 140px;
            }
            
            .hero-content h1 {
                font-size: 2.8rem;
            }
            
            .section-title {
                font-size: 2.2rem;
            }
            
            .footer-container {
                grid-template-columns: 1fr 1fr;
            }
        }

        @media (max-width: 768px) {
            .mobile-menu-toggle {
                display: block;
            }
            
            .nav {
                position: fixed;
                top: 70px;
                left: 0;
                width: 100%;
                background-color: white;
                flex-direction: column;
                padding: 20px;
                box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
                transform: translateY(-100%);
                opacity: 0;
                visibility: hidden;
                transition: var(--transition);
            }
            
            .nav.active {
                transform: translateY(0);
                opacity: 1;
                visibility: visible;
            }
            
            .nav-list {
                flex-direction: column;
                width: 100%;
            }
            
            .nav-item {
                margin: 0 0 15px 0;
                width: 100%;
            }
            
            .nav-link {
                display: block;
                padding: 12px 0;
            }
            
            .hero-content h1 {
                font-size: 2.4rem;
            }
            
            .hero-stats {
                flex-direction: column;
                gap: 20px;
            }
            
            .services-tabs {
                flex-direction: column;
                align-items: center;
            }
            
            .tab-btn {
                width: 100%;
                max-width: 300px;
                justify-content: center;
            }
            
            .portfolio-grid {
                grid-template-columns: 1fr;
            }
            
            .footer-container {
                grid-template-columns: 1fr;
                gap: 40px;
            }
            
            .logo {
                height: 50px;
            }
            
            .logo-placeholder .logo-main {
                font-size: 1.8rem;
            }
        }

        @media (max-width: 576px) {
            .hero-content h1 {
                font-size: 2rem;
            }
            
            .section {
                padding: 70px 0;
            }
            
            .section-title {
                font-size: 1.8rem;
            }
            
            .btn {
                padding: 12px 24px;
                font-size: 0.9rem;
            }
            
            .contact-form {
                padding: 30px 20px;
            }
            
            .logo-placeholder .logo-main {
                font-size: 1.5rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header">
        <div class="container header-container">
            <a href="#home" class="logo">
                <!-- Logo Placeholder - Replace with actual logo image -->
                <div class="logo-placeholder">
                    <img src="mateor-labs-high-resolution-logo1.png" alt="Mateor Labs Logo" style="height: 60px; width: auto;">
                </div>
            </a>
            
            <button class="mobile-menu-toggle" id="mobileMenuToggle">
                <i class="fas fa-bars"></i>
            </button>
            
            <nav class="nav" id="nav">
                <ul class="nav-list">
                    <li class="nav-item"><a href="#home" class="nav-link">Home</a></li>
                    <li class="nav-item"><a href="#services" class="nav-link">Services</a></li>
                    <li class="nav-item"><a href="#portfolio" class="nav-link">Portfolio</a></li>
                    <li class="nav-item"><a href="#about" class="nav-link">About</a></li>
                    <li class="nav-item"><a href="#partners" class="nav-link">Partners</a></li>
                    <li class="nav-item"><a href="#contact" class="nav-link">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container hero-container">
            <div class="hero-content fade-in-up">
                <h1>Technology Solutions for the Digital Space</h1>
                <p>Providing innovative technological services, software deployment, network configuration, and ICT equipment solutions since 2021.</p>
                <div class="hero-buttons">
                    <a href="#contact" class="btn btn-primary">Get Started <i class="fas fa-arrow-right"></i></a>
                    <a href="#portfolio" class="btn btn-outline">View Our Work</a>
                </div>
                <div class="hero-stats">
                    <div class="stat-item">
                        <div class="stat-number">50+</div>
                        <div class="stat-label">Projects Completed</div>
                    </div>
                    <div class="stat-item">
                        <div class="stat-number">24/7</div>
                        <div class="stat-label">Support</div>
                    </div>
                    <div class="stat-item">
                        <div class="stat-number">100%</div>
                        <div class="stat-label">Client Satisfaction</div>
                    </div>
                </div>
            </div>
            <div class="hero-visual fade-in">
                <div class="hero-image">
                    <img src="https://images.unsplash.com/photo-1558494949-ef010cbdcc31?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Technology Solutions">
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="section services" id="services">
        <div class="container">
            <div class="section-header">
                <h2 class="section-title">Our Services</h2>
                <p class="section-subtitle">Comprehensive technology solutions tailored to drive your digital transformation and business growth.</p>
            </div>
            
            <div class="services-tabs">
                <button class="tab-btn active" data-tab="tech">
                    <i class="fas fa-laptop-code"></i> Technology Services
                </button>
                <button class="tab-btn" data-tab="network">
                    <i class="fas fa-network-wired"></i> Network Solutions
                </button>
                <button class="tab-btn" data-tab="ict">
                    <i class="fas fa-server"></i> ICT Equipment
                </button>
                <button class="tab-btn" data-tab="consulting">
                    <i class="fas fa-chart-line"></i> IT Consulting
                </button>
            </div>
            
            <!-- Technology Services -->
            <div class="services-content active" id="tech-content">
                <div class="service-image">
                    <img src="https://images.unsplash.com/photo-1517077304055-6e89abbf09b0?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Technology Services">
                </div>
                <div class="service-details">
                    <h3>Technology Services</h3>
                    <p>We deliver cutting-edge technology solutions that transform businesses and drive digital innovation. Our services are designed to optimize operations, enhance productivity, and future-proof your organization.</p>
                    <div class="service-features">
                        <div class="service-feature">
                            <i class="fas fa-check-circle"></i>
                            <div>
                                <h4>Custom Software Development</h4>
                                <p>Tailored applications built to address your specific business challenges and opportunities.</p>
                            </div>
                        </div>
                        <div class="service-feature">
                            <i class="fas fa-check-circle"></i>
                            <div>
                                <h4>Cloud Solutions & Migration</h4>
                                <p>Seamless transition to cloud infrastructure with ongoing management and optimization.</p>
                            </div>
                        </div>
                        <div class="service-feature">
                            <i class="fas fa-check-circle"></i>
                            <div>
                                <h4>System Integration</h4>
                                <p>Connecting disparate systems to create cohesive, efficient technology ecosystems.</p>
                            </div>
                        </div>
                    </div>
                    <a href="#contact" class="btn btn-primary">Discuss Your Project</a>
                </div>
            </div>
            
            <!-- Network Solutions -->
            <div class="services-content" id="network-content">
                <div class="service-image">
                    <img src="https://images.unsplash.com/photo-1558494949-ef010cbdcc31?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Network Solutions">
                </div>
                <div class="service-details">
                    <h3>Network Solutions</h3>
                    <p>Secure, reliable, and scalable network infrastructure designed to support your business operations now and in the future. We implement robust networking solutions that ensure connectivity, security, and performance.</p>
                    <div class="service-features">
                        <div class="service-feature">
                            <i class="fas fa-check-circle"></i>
                            <div>
                                <h4>Network Design & Implementation</h4>
                                <p>Comprehensive network architecture planning and deployment for optimal performance.</p>
                            </div>
                        </div>
                        <div class="service-feature">
                            <i class="fas fa-check-circle"></i>
                            <div>
                                <h4>Cybersecurity Infrastructure</h4>
                                <p>Multi-layered security solutions to protect your data, systems, and networks.</p>
                            </div>
                        </div>
                        <div class="service-feature">
                            <i class="fas fa-check-circle"></i>
                            <div>
                                <h4>Network Monitoring & Management</h4>
                                <p>Proactive monitoring and maintenance to ensure network reliability and uptime.</p>
                            </div>
                        </div>
                    </div>
                    <a href="#contact" class="btn btn-primary">Secure Your Network</a>
                </div>
            </div>
            
            <!-- ICT Equipment -->
            <div class="services-content" id="ict-content">
                <div class="service-image">
                    <img src="https://images.unsplash.com/photo-1581094794329-c8112a89af12?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="ICT Equipment">
                </div>
                <div class="service-details">
                    <h3>ICT Equipment Solutions</h3>
                    <p>High-quality ICT hardware and equipment from trusted manufacturers to build and enhance your technology infrastructure. We provide end-to-end solutions from procurement to configuration and support.</p>
                    <div class="service-features">
                        <div class="service-feature">
                            <i class="fas fa-check-circle"></i>
                            <div>
                                <h4>Enterprise Hardware Procurement</h4>
                                <p>Strategic sourcing of reliable, enterprise-grade ICT equipment from leading vendors.</p>
                            </div>
                        </div>
                        <div class="service-feature">
                            <i class="fas fa-check-circle"></i>
                            <div>
                                <h4>Installation & Configuration</h4>
                                <p>Professional setup and optimization of hardware to ensure peak performance.</p>
                            </div>
                        </div>
                        <div class="service-feature">
                            <i class="fas fa-check-circle"></i>
                            <div>
                                <h4>Maintenance & Support</h4>
                                <p>Ongoing technical support and maintenance services to maximize equipment lifespan.</p>
                            </div>
                        </div>
                    </div>
                    <a href="#contact" class="btn btn-primary">Request Equipment Quote</a>
                </div>
            </div>
            
            <!-- IT Consulting -->
            <div class="services-content" id="consulting-content">
                <div class="service-image">
                    <img src="https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="IT Consulting">
                </div>
                <div class="service-details">
                    <h3>IT Consulting & Strategy</h3>
                    <p>Strategic technology guidance to align your IT investments with business objectives. We help organizations navigate digital transformation and leverage technology for competitive advantage.</p>
                    <div class="service-features">
                        <div class="service-feature">
                            <i class="fas fa-check-circle"></i>
                            <div>
                                <h4>Digital Transformation Strategy</h4>
                                <p>Comprehensive roadmaps for leveraging technology to transform business operations.</p>
                            </div>
                        </div>
                        <div class="service-feature">
                            <i class="fas fa-check-circle"></i>
                            <div>
                                <h4>Technology Assessment & Planning</h4>
                                <p>Evaluation of current technology landscape and strategic planning for future needs.</p>
                            </div>
                        </div>
                        <div class="service-feature">
                            <i class="fas fa-check-circle"></i>
                            <div>
                                <h4>IT Governance & Compliance</h4>
                                <p>Framework development for effective IT management, risk mitigation, and compliance.</p>
                            </div>
                        </div>
                    </div>
                    <a href="#contact" class="btn btn-primary">Schedule Consultation</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Portfolio Section -->
    <section class="section portfolio" id="portfolio">
        <div class="container">
            <div class="section-header">
                <h2 class="section-title">Our Portfolio</h2>
                <p class="section-subtitle">Showcasing innovative technology solutions that have transformed businesses and delivered measurable results.</p>
            </div>
            
            <div class="portfolio-grid">
                <div class="portfolio-item fade-in-up">
                    <div class="portfolio-image">
                        <img src="https://images.unsplash.com/photo-1542744095-fcf48d80b0fd?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Enterprise Network Solutions">
                    </div>
                    <div class="portfolio-content">
                        <h3>Enterprise Network Solutions</h3>
                        <p>Comprehensive network infrastructure design and implementation for a financial institution with 50+ branches nationwide, improving connectivity and security.</p>
                        <div class="portfolio-tech">
                            <span class="tech-tag">Cisco</span>
                            <span class="tech-tag">Fortinet</span>
                            <span class="tech-tag">SD-WAN</span>
                        </div>
                    </div>
                </div>
                
                <div class="portfolio-item fade-in-up">
                    <div class="portfolio-image">
                        <img src="https://images.unsplash.com/photo-1531297484001-80022131f5a1?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Digital Transformation">
                    </div>
                    <div class="portfolio-content">
                        <h3>Digital Transformation Initiative</h3>
                        <p>Cloud migration and process automation for a retail chain with over 200 stores, resulting in 40% operational efficiency improvement.</p>
                        <div class="portfolio-tech">
                            <span class="tech-tag">AWS</span>
                            <span class="tech-tag">Azure</span>
                            <span class="tech-tag">Automation</span>
                        </div>
                    </div>
                </div>
                
                <div class="portfolio-item fade-in-up">
                    <div class="portfolio-image">
                        <img src="https://images.unsplash.com/photo-1518186285589-2f7649de83e0?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="ICT Infrastructure">
                    </div>
                    <div class="portfolio-content">
                        <h3>ICT Infrastructure Modernization</h3>
                        <p>End-to-end technology infrastructure setup for a new corporate campus supporting 1000+ employees with cutting-edge collaboration tools.</p>
                        <div class="portfolio-tech">
                            <span class="tech-tag">VMware</span>
                            <span class="tech-tag">Microsoft 365</span>
                            <span class="tech-tag">Unified Comms</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section class="section about" id="about">
        <div class="container">
            <div class="section-header">
                <h2 class="section-title">About Mateor Labs</h2>
                <p class="section-subtitle">Driving technological excellence through innovation, expertise, and client-focused solutions since 2021.</p>
            </div>
            
            <div class="about-container">
                <div class="about-content">
                    <h2>Leading Technology Solutions Provider</h2>
                    <p>Mateor Labs (Private) Limited is a premier technology solutions company specializing in delivering innovative digital transformation services, network infrastructure, and ICT equipment solutions.</p>
                    <p>Founded in 2021, we have rapidly established ourselves as a trusted partner for businesses seeking to leverage technology for competitive advantage and operational excellence.</p>
                    
                    <div class="about-highlights">
                        <div class="highlight">
                            <div class="highlight-icon">
                                <i class="fas fa-bullseye"></i>
                            </div>
                            <div>
                                <h3>Our Mission</h3>
                                <p>To empower businesses with transformative technology solutions that drive growth, efficiency, and innovation in the digital era.</p>
                            </div>
                        </div>
                        
                        <div class="highlight">
                            <div class="highlight-icon">
                                <i class="fas fa-eye"></i>
                            </div>
                            <div>
                                <h3>Our Vision</h3>
                                <p>To be the leading technology partner for organizations across Africa, recognized for excellence, innovation, and client success.</p>
                            </div>
                        </div>
                        
                        <div class="highlight">
                            <div class="highlight-icon">
                                <i class="fas fa-handshake"></i>
                            </div>
                            <div>
                                <h3>Our Values</h3>
                                <p>Innovation, Integrity, Excellence, Client-Centricity, and Continuous Improvement guide everything we do.</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="about-visual">
                    <div class="about-image">
                        <img src="https://images.unsplash.com/photo-1522071820081-009f0129c71c?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="About Mateor Labs">
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Partners Section -->
    <section class="section partners" id="partners">
        <div class="container">
            <div class="section-header">
                <h2 class="section-title">Technology Partners</h2>
                <p class="section-subtitle">We collaborate with industry-leading technology partners to deliver best-in-class solutions to our clients.</p>
            </div>
            
            <div class="partners-container">
                <div class="partners-grid">
                    <div class="partner-card fade-in-up">
                        <div class="partner-logo">
                            <i class="fas fa-shield-alt" style="font-size: 3.5rem; color: var(--accent);"></i>
                        </div>
                        <h3 class="partner-name">ESET Cybersecurity</h3>
                        <p class="partner-description">World-leading cybersecurity solutions provider with advanced threat detection and prevention technologies.</p>
                    </div>
                    
                    <div class="partner-card fade-in-up">
                        <div class="partner-logo">
                            <i class="fas fa-lock" style="font-size: 3.5rem; color: var(--accent);"></i>
                        </div>
                        <h3 class="partner-name">SOPHOS Security</h3>
                        <p class="partner-description">Advanced network security and threat intelligence solutions for businesses of all sizes.</p>
                    </div>
                    
                    <div class="partner-card fade-in-up">
                        <div class="partner-logo">
                            <i class="fas fa-cloud" style="font-size: 3.5rem; color: var(--accent);"></i>
                        </div>
                        <h3 class="partner-name">Microsoft Azure</h3>
                        <p class="partner-description">Leading cloud platform for building, deploying, and managing applications and services.</p>
                    </div>
                    
                    <div class="partner-card fade-in-up">
                        <div class="partner-logo">
                            <i class="fas fa-network-wired" style="font-size: 3.5rem; color: var(--accent);"></i>
                        </div>
                        <h3 class="partner-name">Cisco Systems</h3>
                        <p class="partner-description">Global leader in networking, cybersecurity, and collaboration solutions for enterprises.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="section contact" id="contact">
        <div class="container">
            <div class="section-header">
                <h2 class="section-title">Get In Touch</h2>
                <p class="section-subtitle">Ready to transform your business with technology? Contact us today to discuss your requirements.</p>
            </div>
            
            <div class="contact-container">
                <div class="contact-info">
                    <h3>Connect With Our Team</h3>
                    <p>We're here to help you navigate your technology journey. Reach out to us for consultations, project discussions, or any inquiries.</p>
                    
                    <div class="contact-details">
                        <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fas fa-envelope"></i>
                            </div>
                            <div class="contact-text">
                                <h4>Email Us</h4>
                                <p>info@mateorlabs.co.zw</p>
                            </div>
                        </div>
                        
                        <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fas fa-globe"></i>
                            </div>
                            <div class="contact-text">
                                <h4>Online Presence</h4>
                                <p>Fully digital operations with remote support capabilities across regions</p>
                            </div>
                        </div>
                        
                        <div class="contact-item">
                            <div class="contact-icon">
                                <i class="fas fa-clock"></i>
                            </div>
                            <div class="contact-text">
                                <h4>Response Time</h4>
                                <p>We typically respond to inquiries within 24 hours during business days</p>
                            </div>
                        </div>
                    </div>
                    
                    <div class="social-links">
                        <a href="https://www.instagram.com/mateorlabs" class="social-link" target="_blank"><i class="fab fa-instagram"></i></a>
                        <a href="https://www.facebook.com/MateorLabs" class="social-link" target="_blank"><i class="fab fa-facebook-f"></i></a>
                        <a href="https://www.linkedin.com/company/mateorlabs" class="social-link" target="_blank"><i class="fab fa-linkedin-in"></i></a>
                        <a href="https://www.x.com/mateorlabs" class="social-link" target="_blank"><i class="fab fa-twitter"></i></a>
                    </div>
                </div>
                
                <div class="contact-form">
                    <form id="contactForm">
                        <div class="form-group">
                            <input type="text" class="form-control" placeholder="Your Name" required>
                        </div>
                        <div class="form-group">
                            <input type="email" class="form-control" placeholder="Email Address" required>
                        </div>
                        <div class="form-group">
                            <input type="text" class="form-control" placeholder="Company Name">
                        </div>
                        <div class="form-group">
                            <select class="form-control" required>
                                <option value="" disabled selected>Service Interest</option>
                                <option value="technology">Technology Services</option>
                                <option value="network">Network Solutions</option>
                                <option value="ict">ICT Equipment</option>
                                <option value="consulting">IT Consulting</option>
                                <option value="other">Other</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <textarea class="form-control" placeholder="Project Details or Inquiry" required></textarea>
                        </div>
                        <button type="submit" class="btn btn-primary" style="width: 100%;">Send Message <i class="fas fa-paper-plane"></i></button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="container">
            <div class="footer-container">
                <div class="footer-about">
                    <a href="#home" class="logo">
                        <!-- Logo Placeholder - Replace with actual logo image -->
                        <div class="logo-placeholder">
                           <img src="mateor-labs-high-resolution-logo1.png" alt="Mateor Labs Logo" style="height: 60px; width: auto;">
                        </div>
                    </a>
                    <p>Leading provider of innovative technology solutions, software deployment, network configuration, and ICT equipment since 2021.</p>
                    <p>Mateor Labs (Private) Limited</p>
                </div>
                
                <div class="footer-links">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#home">Home</a></li>
                        <li><a href="#services">Services</a></li>
                        <li><a href="#portfolio">Portfolio</a></li>
                        <li><a href="#about">About Us</a></li>
                        <li><a href="#partners">Partners</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </div>
                
                <div class="footer-contact">
                    <h3>Contact Info</h3>
                    <p><i class="fas fa-envelope"></i> info@mateorlabs.co.zw</p>
                    <p><i class="fas fa-globe"></i> www.mateorlabs.co.zw</p>
                    <p><i class="fas fa-map-marker-alt"></i> Digital Operations | Serving Clients Nationwide</p>
                    <p><i class="fas fa-building"></i> Mateor Labs (Private) Limited</p>
                </div>
            </div>
            
            <div class="footer-bottom">
                <p>&copy; 2021-2023 Mateor Labs (Private) Limited. All rights reserved. | Data privacy and protection compliant.</p>
                <p>Technology Solutions for the Digital Space</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile Menu Toggle
        const mobileMenuToggle = document.getElementById('mobileMenuToggle');
        const nav = document.getElementById('nav');
        
        mobileMenuToggle.addEventListener('click', () => {
            nav.classList.toggle('active');
            mobileMenuToggle.innerHTML = nav.classList.contains('active') 
                ? '<i class="fas fa-times"></i>' 
                : '<i class="fas fa-bars"></i>';
        });
        
        // Close mobile menu when clicking a link
        document.querySelectorAll('.nav-link').forEach(link => {
            link.addEventListener('click', () => {
                nav.classList.remove('active');
                mobileMenuToggle.innerHTML = '<i class="fas fa-bars"></i>';
            });
        });
        
        // Header scroll effect
        const header = document.querySelector('.header');
        
        window.addEventListener('scroll', () => {
            if (window.scrollY > 50) {
                header.classList.add('scrolled');
            } else {
                header.classList.remove('scrolled');
            }
        });
        
        // Services Tabs
        const tabButtons = document.querySelectorAll('.tab-btn');
        const serviceContents = document.querySelectorAll('.services-content');
        
        tabButtons.forEach(button => {
            button.addEventListener('click', () => {
                // Remove active class from all buttons and contents
                tabButtons.forEach(btn => btn.classList.remove('active'));
                serviceContents.forEach(content => content.classList.remove('active'));
                
                // Add active class to clicked button
                button.classList.add('active');
                
                // Show corresponding content
                const tabId = button.getAttribute('data-tab');
                document.getElementById(`${tabId}-content`).classList.add('active');
            });
        });
        
        // Fade-in animation on scroll
        const fadeElements = document.querySelectorAll('.fade-in-up');
        
        const fadeInOnScroll = () => {
            fadeElements.forEach(element => {
                const elementTop = element.getBoundingClientRect().top;
                const elementVisible = 150;
                
                if (elementTop < window.innerHeight - elementVisible) {
                    element.classList.add('active');
                }
            });
        };
        
        // Set initial state
        fadeElements.forEach(element => {
            element.classList.remove('active');
        });
        
        // Check on scroll and load
        window.addEventListener('scroll', fadeInOnScroll);
        window.addEventListener('load', fadeInOnScroll);
        
        // Form submission
        const contactForm = document.getElementById('contactForm');
        
        contactForm.addEventListener('submit', (e) => {
            e.preventDefault();
            
            // Get form data
            const formData = new FormData(contactForm);
            const formValues = Object.fromEntries(formData);
            
            // In a real implementation, you would send this to a server
            console.log('Form submitted:', formValues);
            
            // Show success message
            alert('Thank you for your message! We will contact you within 24 hours.');
            contactForm.reset();
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
    </script>
</body>
</html>
