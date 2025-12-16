<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wetine Enterprises | Quality Hardware & Electronics</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-green: #2e7d32;    /* Main brand green */
            --dark-green: #1b5e20;       /* Darker shade for hover states */
            --light-green: #e8f5e9;      /* Light tint for backgrounds */
            --accent-amber: #ff8f00;     /* Accent color for highlights */
            --neutral-dark: #2d3748;
            --neutral-gray: #718096;
            --neutral-light: #f7fafc;
            --white: #ffffff;
        }
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Inter', sans-serif;
            line-height: 1.6;
            color: var(--neutral-dark);
            background-color: var(--white);
        }
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        /* Header & Navigation */
        .main-header {
            background-color: var(--white);
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }
        .logo {
            font-size: 24px;
            font-weight: 700;
            color: var(--primary-green);
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        .logo span {
            color: var(--neutral-dark);
        }
        .main-nav {
            display: flex;
            align-items: center;
            gap: 30px;
        }
        .nav-links {
            display: flex;
            list-style: none;
            gap: 30px;
        }
        .nav-links a {
            text-decoration: none;
            color: var(--neutral-dark);
            font-weight: 500;
            transition: color 0.3s;
        }
        .nav-links a:hover {
            color: var(--primary-green);
        }
        .cart-icon {
            position: relative;
            cursor: pointer;
        }
        .cart-icon i {
            font-size: 22px;
            color: var(--neutral-dark);
        }
        .cart-count {
            position: absolute;
            top: -8px;
            right: -8px;
            background-color: var(--accent-amber);
            color: white;
            width: 20px;
            height: 20px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 12px;
            font-weight: bold;
        }
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 24px;
            color: var(--neutral-dark);
            cursor: pointer;
        }
        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(46, 125, 50, 0.9), rgba(27, 94, 32, 0.9)), url('https://images.unsplash.com/photo-1581094715295-bf7d63bd5c44?ixlib=rb-4.0.3&auto=format&fit=crop&w=1600&q=80');
            background-size: cover;
            background-position: center;
            color: var(--white);
            text-align: center;
            padding: 120px 0;
        }
        .hero h1 {
            font-size: 3.5rem;
            font-weight: 700;
            margin-bottom: 20px;
            line-height: 1.2;
        }
        .hero p {
            font-size: 1.25rem;
            max-width: 700px;
            margin: 0 auto 40px;
            opacity: 0.9;
        }
        .cta-button {
            display: inline-block;
            background-color: var(--white);
            color: var(--primary-green);
            padding: 15px 35px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            transition: all 0.3s ease;
        }
        .cta-button:hover {
            background-color: var(--light-green);
            transform: translateY(-3px);
        }
        /* Services/Products Section */
        .services {
            padding: 100px 0;
            background-color: var(--neutral-light);
        }
        .section-title {
            text-align: center;
            margin-bottom: 60px;
        }
        .section-title h2 {
            font-size: 2.5rem;
            font-weight: 700;
            color: var(--neutral-dark);
            margin-bottom: 15px;
        }
        .section-title p {
            font-size: 1.125rem;
            color: var(--neutral-gray);
            max-width: 700px;
            margin: 0 auto;
        }
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
        }
        .service-card {
            background-color: var(--white);
            border-radius: 10px;
            padding: 40px 30px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        .service-icon {
            width: 70px;
            height: 70px;
            background-color: var(--light-green);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 25px;
        }
        .service-icon i {
            font-size: 30px;
            color: var(--primary-green);
        }
        .service-card h3 {
            font-size: 1.5rem;
            font-weight: 600;
            margin-bottom: 15px;
            color: var(--neutral-dark);
        }
        .service-card p {
            color: var(--neutral-gray);
            margin-bottom: 20px;
        }
        /* Challenges Section */
        .challenges {
            padding: 100px 0;
            background-color: var(--white);
        }
        .challenges-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
        }
        .challenge-card {
            text-align: center;
        }
        .challenge-stat {
            font-size: 3rem;
            font-weight: 700;
            color: var(--primary-green);
            margin-bottom: 15px;
            line-height: 1;
        }
        .challenge-card h3 {
            font-size: 1.5rem;
            font-weight: 600;
            margin-bottom: 15px;
            color: var(--neutral-dark);
        }
        /* Testimonials */
        .testimonials {
            padding: 100px 0;
            background-color: var(--neutral-light);
        }
        .testimonial-slider {
            max-width: 800px;
            margin: 0 auto;
        }
        .testimonial-card {
            background-color: var(--white);
            border-radius: 10px;
            padding: 40px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        .testimonial-text {
            font-size: 1.25rem;
            font-style: italic;
            color: var(--neutral-dark);
            margin-bottom: 30px;
            line-height: 1.7;
        }
        .testimonial-author {
            display: flex;
            align-items: center;
            gap: 15px;
        }
        .author-avatar {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background-color: var(--light-green);
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--primary-green);
            font-size: 24px;
            font-weight: 700;
        }
        .author-info h4 {
            font-weight: 600;
            margin-bottom: 5px;
        }
        .author-info p {
            color: var(--neutral-gray);
            font-size: 0.9rem;
        }
        /* Product Grid & Cart */
        .product-section {
            padding: 100px 0;
            display: none;
        }
        .product-filters {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 10px;
            margin-bottom: 40px;
        }
        .filter-btn {
            background-color: var(--white);
            border: 2px solid var(--primary-green);
            color: var(--primary-green);
            padding: 10px 25px;
            border-radius: 30px;
            cursor: pointer;
            font-weight: 500;
            transition: all 0.3s ease;
        }
        .filter-btn.active, .filter-btn:hover {
            background-color: var(--primary-green);
            color: var(--white);
        }
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 30px;
            margin-bottom: 50px;
        }
        .product-card {
            background-color: var(--white);
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease;
        }
        .product-card:hover {
            transform: translateY(-5px);
        }
        .product-image {
            height: 200px;
            overflow: hidden;
        }
        .product-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        .product-card:hover .product-image img {
            transform: scale(1.05);
        }
        .product-info {
            padding: 20px;
        }
        .product-title {
            font-size: 1.1rem;
            font-weight: 600;
            margin-bottom: 10px;
            height: 50px;
            overflow: hidden;
        }
        .product-price {
            color: var(--primary-green);
            font-size: 1.5rem;
            font-weight: 700;
            margin-bottom: 15px;
        }
        .product-actions {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .add-to-cart {
            background-color: var(--primary-green);
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 8px;
            transition: background-color 0.3s ease;
        }
        .add-to-cart:hover {
            background-color: var(--dark-green);
        }
        /* Cart Modal */
        .cart-modal {
            position: fixed;
            top: 0;
            right: -400px;
            width: 380px;
            height: 100%;
            background-color: white;
            box-shadow: -5px 0 15px rgba(0, 0, 0, 0.1);
            z-index: 1100;
            transition: right 0.4s ease;
            overflow-y: auto;
        }
        .cart-modal.active {
            right: 0;
        }
        .cart-header {
            background-color: var(--primary-green);
            color: white;
            padding: 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .close-cart {
            background: none;
            border: none;
            color: white;
            font-size: 28px;
            cursor: pointer;
        }
        .cart-items {
            padding: 20px;
            max-height: calc(100vh - 250px);
            overflow-y: auto;
        }
        .cart-item {
            display: flex;
            gap: 15px;
            padding: 15px 0;
            border-bottom: 1px solid #eee;
        }
        .cart-footer {
            padding: 20px;
            border-top: 2px solid #eee;
            position: absolute;
            bottom: 0;
            width: 100%;
            background-color: white;
        }
        .cart-total {
            display: flex;
            justify-content: space-between;
            font-size: 1.5rem;
            font-weight: 700;
            margin-bottom: 20px;
        }
        .checkout-btn {
            background-color: var(--accent-amber);
            color: white;
            border: none;
            padding: 15px;
            border-radius: 5px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            width: 100%;
        }
        .checkout-btn:hover {
            background-color: #e67e00;
        }
        .overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
            z-index: 1050;
            display: none;
        }
        .overlay.active {
            display: block;
        }
        /* Footer */
        .main-footer {
            background-color: var(--neutral-dark);
            color: var(--white);
            padding: 70px 0 30px;
        }
        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 50px;
        }
        .footer-column h3 {
            font-size: 1.3rem;
            margin-bottom: 25px;
            position: relative;
            padding-bottom: 10px;
        }
        .footer-column h3::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 50px;
            height: 3px;
            background-color: var(--primary-green);
        }
        .contact-info {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }
        .contact-info div {
            display: flex;
            align-items: flex-start;
            gap: 10px;
        }
        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: rgba(255, 255, 255, 0.7);
            font-size: 0.9rem;
        }
        /* Responsive */
        @media (max-width: 992px) {
            .hero h1 {
                font-size: 2.8rem;
            }
            .services-grid {
                grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            }
        }
        @media (max-width: 768px) {
            .mobile-menu-btn {
                display: block;
            }
            .main-nav {
                position: fixed;
                top: 80px;
                left: 0;
                width: 100%;
                background-color: var(--white);
                flex-direction: column;
                padding: 20px;
                box-shadow: 0 10px 15px rgba(0,0,0,0.1);
                transform: translateY(-100%);
                opacity: 0;
                transition: all 0.3s ease;
                z-index: 999;
            }
            .main-nav.active {
                transform: translateY(0);
                opacity: 1;
            }
            .nav-links {
                flex-direction: column;
                width: 100%;
                text-align: center;
            }
            .hero {
                padding: 80px 0;
            }
            .hero h1 {
                font-size: 2.3rem;
            }
            .hero p {
                font-size: 1.1rem;
            }
            .cart-modal {
                width: 100%;
                right: -100%;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="main-header">
        <div class="container header-container">
            <a href="#" class="logo">
    <img src="prest.png" alt="Wetine Enterprises Logo">
</a>
            <button class="mobile-menu-btn" id="mobileMenuBtn">
                <i class="fas fa-bars"></i>
            </button>
            <nav class="main-nav" id="mainNav">
                <ul class="nav-links">
                    <li><a href="#home">Home</a></li>
                    <li><a href="#products" id="productsLink">Products</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#testimonials">Testimonials</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
                <div class="cart-icon" id="cartIcon">
                    <i class="fas fa-shopping-cart"></i>
                    <div class="cart-count" id="cartCount">0</div>
                </div>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <h1>Quality Hardware & Electronics.</h1>
            <p>From industrial tools and construction materials to cutting-edge computers and mobile devices, we provide durable, sustainable solutions designed to build, secure, and power your business forward.</p>
            <a href="#products" class="cta-button" id="shopNowBtn">Explore Our Products</a>
        </div>
    </section>

    <!-- Services/Products Overview -->
    <section class="services" id="services">
        <div class="container">
            <div class="section-title">
                <h2>Tailored Solutions for Every Need.</h2>
                <p>Secure, Reliable, and Built to Last. We supply the essential tools and technology that form the foundation of homes, businesses, and industries across Zimbabwe.</p>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-tools"></i>
                    </div>
                    <h3>Tools & Equipment</h3>
                    <p>High-quality tools for both home DIY and industrial applications, all meeting stringent quality standards and backed by guarantees.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-hammer"></i>
                    </div>
                    <h3>Hardware & Supplies</h3>
                    <p>Durable wheelbarrows, garden tools, construction equipment, electrical conduits, and sundries you can count on every day.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-hard-hat"></i>
                    </div>
                    <h3>Protective Clothing</h3>
                    <p>Trusted safety wear including industrial gear, fire-resistant clothing, heavy-duty wear, and full body protection for any worksite.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-tree"></i>
                    </div>
                    <h3>Timber & Wood Products</h3>
                    <p>Premium timber from the country's best mills, used for roofing, carpentry, and high-quality timber products like doors.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-home"></i>
                    </div>
                    <h3>Roofing Solutions</h3>
                    <p>High-quality asbestos roofing sheets, IBR sheets, and roofing tiles to provide secure and lasting shelter.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-laptop"></i>
                    </div>
                    <h3>Electronics & IT</h3>
                    <p>Computers, printers, CCTV systems, internet modems, mobile phones, and accessories from genuine suppliers with warranty.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Business Challenges -->
    <section class="challenges" id="challenges">
        <div class="container">
            <div class="section-title">
                <h2>Overcoming Common Business Hurdles</h2>
                <p>We understand the challenges faced by builders, contractors, and businesses in sourcing reliable materials and equipment.</p>
            </div>
            <div class="challenges-grid">
                <div class="challenge-card">
                    <div class="challenge-stat">90%</div>
                    <h3>Finding Durable Products</h3>
                    <p>of contractors report difficulty sourcing tools and materials that last, leading to frequent replacements and cost overruns.</p>
                </div>
                <div class="challenge-card">
                    <div class="challenge-stat">70%</div>
                    <h3>Supply Chain Delays</h3>
                    <p>of projects experience delays due to unreliable suppliers, impacting deadlines and increasing labour costs.</p>
                </div>
                <div class="challenge-card">
                    <div class="challenge-stat">$1K+</div>
                    <h3>Hidden Costs of Quality</h3>
                    <p>Average monthly loss per business from equipment failure, safety incidents, and substandard materials.</p>
                </div>
                <div class="challenge-card">
                    <div class="challenge-stat">24/7</div>
                    <h3>Need for Dependable Support</h3>
                    <p>Access to reliable product guarantees and supplier support is non-negotiable for keeping operations smooth.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Product Shopping Section (Initially Hidden) -->
    <section class="product-section" id="products">
        <div class="container">
            <div class="section-title">
                <h2>Our Product Catalog</h2>
                <p>Browse and purchase our high-quality range of hardware and electronics. Add items to your cart and order directly via WhatsApp.</p>
            </div>
            <div class="product-filters">
                <button class="filter-btn active" data-filter="all">All Products</button>
                <button class="filter-btn" data-filter="hardware">Hardware Tools</button>
                <button class="filter-btn" data-filter="electronics">Computer Accessories</button>
                <button class="filter-btn" data-filter="safety">Safety Equipment</button>
            </div>
            <div class="product-grid" id="productGrid">
                <!-- Products loaded by JavaScript -->
            </div>
        </div>
    </section>

    <!-- Testimonials -->
    <section class="testimonials" id="testimonials">
        <div class="container">
            <div class="section-title">
                <h2>Trusted by Industry Professionals</h2>
                <p>See what our customers say about the quality and reliability of Wetine Enterprises products and service.</p>
            </div>
            <div class="testimonial-slider">
                <div class="testimonial-card">
                    <p class="testimonial-text">"The roofing sheets and timber we sourced for our latest project were exceptional quality. They withstood heavy rains perfectly, and the delivery was on schedule. Wetine Enterprises is now our go-to supplier."</p>
                    <div class="testimonial-author">
                        <div class="author-avatar">C</div>
                        <div class="author-info">
                            <h4>Chengetai Mapfumo</h4>
                            <p>Project Manager, Harare Construction Ltd.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="main-footer" id="contact">
        <div class="container">
            <div class="footer-grid">
                <div class="footer-column">
                    <h3>Wetine Enterprises</h3>
                    <p>Providing high-quality tools, hardware, electronics, and sustainable products to individuals and corporates across Zimbabwe since establishment.</p>
                    <p><strong>Our Motto:</strong> Sustainable products everywhere.</p>
                </div>
                <div class="footer-column">
                    <h3>Quick Links</h3>
                    <ul style="list-style: none;">
                        <li style="margin-bottom: 10px;"><a href="#home" style="color: #ccc; text-decoration: none;">Home</a></li>
                        <li style="margin-bottom: 10px;"><a href="#products" style="color: #ccc; text-decoration: none;">Products</a></li>
                        <li style="margin-bottom: 10px;"><a href="#about" style="color: #ccc; text-decoration: none;">About Us</a></li>
                        <li style="margin-bottom: 10px;"><a href="#contact" style="color: #ccc; text-decoration: none;">Contact</a></li>
                    </ul>
                </div>
                <div class="footer-column">
                    <h3>Contact Details</h3>
                    <div class="contact-info">
                        <div>
                            <i class="fas fa-phone"></i>
                            <span>+263 788 375 175</span>
                        </div>
                        <div>
                            <i class="fas fa-envelope"></i>
                            <span>wetineenterprises2023@gmail.com</span>
                        </div>
                        <div>
                            <i class="fas fa-map-marker-alt"></i>
                            <span>Std No.56, Close 228, Budiriro 1, Harare</span>
                        </div>
                        <div>
                            <i class="fas fa-map-marker-alt"></i>
                            <span>56228 Close No.1, Budiriro, Harare</span>
                        </div>
                    </div>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2023 Wetine Enterprises. All Rights Reserved.</p>
            </div>
        </div>
    </footer>

    <!-- Cart Modal & Overlay -->
    <div class="overlay" id="overlay"></div>
    <div class="cart-modal" id="cartModal">
        <div class="cart-header">
            <h3 style="color: white; margin: 0;">Your Cart</h3>
            <button class="close-cart" id="closeCart">&times;</button>
        </div>
        <div class="cart-items" id="cartItems">
            <p style="text-align: center; padding: 40px 20px; color: #888;">Your cart is empty</p>
        </div>
        <div class="cart-footer">
            <div class="cart-total">
                <span>Total:</span>
                <span id="cartTotalPrice">$0.00</span>
            </div>
            <button class="checkout-btn" id="checkoutBtn">
                <i class="fab fa-whatsapp"></i> Order via WhatsApp
            </button>
        </div>
    </div>

    <script>
        // ===== PRODUCT DATA =====
        const products = [
            // HARDWARE TOOLS
            { id: 1, name: "Professional Claw Hammer", category: "hardware", price: 25.99, image: "https://images.unsplash.com/photo-1581235720524-7df154d0dbb8?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" },
            { id: 2, name: "Electric Power Drill Set", category: "hardware", price: 89.99, image: "https://images.unsplash.com/photo-1572981779307-38b8cabb2406?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" },
            { id: 3, name: "Industrial Wheelbarrow", category: "hardware", price: 149.99, image: "https://images.unsplash.com/photo-1565538810643-b5bdb714032a?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=60" },
            { id: 4, name: "Complete Tool Kit (32pc)", category: "hardware", price: 75.00, image: "https://images.unsplash.com/photo-1581094794329-c8112a89af12?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" },
            { id: 5, name: "Angle Grinder", category: "hardware", price: 69.99, image: "https://images.unsplash.com/photo-1581092580497-e0d4cb184827?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" },
            { id: 6, name: "Construction Screwdrivers Set", category: "hardware", price: 28.50, image: "https://images.unsplash.com/photo-1574944985073-8d7b79f9b5e9?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" },
            
            // COMPUTER ACCESSORIES
            { id: 7, name: "Wireless Keyboard & Mouse", category: "electronics", price: 45.99, image: "https://images.unsplash.com/photo-1541140532154-b024d705b90a?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" },
            { id: 8, name: "Computer Monitor 24-inch", category: "electronics", price: 189.99, image: "https://images.unsplash.com/photo-1593359677879-a4bb92f829d1?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" },
            { id: 9, name: "Laptop Cooling Pad", category: "electronics", price: 32.50, image: "https://images.unsplash.com/photo-1593640408182-31c70c8268f5?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" },
            { id: 10, name: "USB-C Hub Adapter", category: "electronics", price: 39.99, image: "https://images.unsplash.com/photo-1587829741301-dc798b83add3?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" },
            { id: 11, name: "Computer Speakers", category: "electronics", price: 59.99, image: "https://images.unsplash.com/photo-1589003077984-894e133dabab?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" },
            { id: 12, name: "Gaming Headset", category: "electronics", price: 79.99, image: "https://images.unsplash.com/photo-1505740420928-5e560c06d30e?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" },
            
            // SAFETY EQUIPMENT
            { id: 13, name: "Safety Helmet with Visor", category: "safety", price: 18.50, image: "https://images.unsplash.com/photo-1558618666-fcd25c85cd64?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" },
            { id: 14, name: "Industrial Safety Gloves", category: "safety", price: 12.75, image: "https://images.unsplash.com/photo-1611591437281-8a4d6c202c7a?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" },
            { id: 15, name: "Safety Goggles", category: "safety", price: 8.99, image: "https://images.unsplash.com/photo-1593536605975-3c36bdc7b4ec?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" },
            { id: 16, name: "Ear Protection", category: "safety", price: 15.50, image: "https://images.unsplash.com/photo-1621451537084-482c73073a0f?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" },
            
            // BUILDING MATERIALS
            { id: 17, name: "Roofing Sheets (10 pack)", category: "hardware", price: 125.00, image: "https://images.unsplash.com/photo-1621506289937-a8e4d8d2f4e1?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=60" },
            { id: 18, name: "Construction Nails (5kg)", category: "hardware", price: 15.75, image: "https://images.unsplash.com/photo-1598128558393-8ffc1f1bdc56?ixlib=rb-4.0.3&auto=format&fit=crop&w=600&q=80" }
        ];

        // ===== CART & STATE =====
        let cart = JSON.parse(localStorage.getItem('wetineCart')) || [];

        // ===== DOM ELEMENTS =====
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const mainNav = document.getElementById('mainNav');
        const cartIcon = document.getElementById('cartIcon');
        const cartModal = document.getElementById('cartModal');
        const overlay = document.getElementById('overlay');
        const closeCart = document.getElementById('closeCart');
        const cartCount = document.getElementById('cartCount');
        const cartItems = document.getElementById('cartItems');
        const cartTotalPrice = document.getElementById('cartTotalPrice');
        const checkoutBtn = document.getElementById('checkoutBtn');
        const productGrid = document.getElementById('productGrid');
        const filterBtns = document.querySelectorAll('.filter-btn');
        const productSection = document.querySelector('.product-section');
        const productsLink = document.getElementById('productsLink');
        const shopNowBtn = document.getElementById('shopNowBtn');

        // ===== INITIALIZATION =====
        document.addEventListener('DOMContentLoaded', function() {
            renderProducts('all');
            updateCartDisplay();
            setupEventListeners();
        });

        // ===== EVENT LISTENERS =====
        function setupEventListeners() {
            mobileMenuBtn.addEventListener('click', () => mainNav.classList.toggle('active'));
            cartIcon.addEventListener('click', toggleCart);
            closeCart.addEventListener('click', toggleCart);
            overlay.addEventListener('click', toggleCart);
            checkoutBtn.addEventListener('click', checkoutViaWhatsApp);
            productsLink.addEventListener('click', showProductSection);
            shopNowBtn.addEventListener('click', showProductSection);

            filterBtns.forEach(btn => {
                btn.addEventListener('click', function() {
                    filterBtns.forEach(b => b.classList.remove('active'));
                    this.classList.add('active');
                    renderProducts(this.dataset.filter);
                });
            });

            // Smooth scrolling for anchor links
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function(e) {
                    const href = this.getAttribute('href');
                    if (href === '#products') {
                        e.preventDefault();
                        showProductSection();
                        return;
                    }
                    if (href !== '#' && href !== '#home') {
                        e.preventDefault();
                        const targetEl = document.querySelector(href);
                        if (targetEl) {
                            window.scrollTo({
                                top: targetEl.offsetTop - 80,
                                behavior: 'smooth'
                            });
                            mainNav.classList.remove('active');
                        }
                    }
                });
            });
        }

        // ===== PRODUCT RENDERING =====
        function renderProducts(filter) {
            productGrid.innerHTML = '';
            const filtered = filter === 'all' ? products : products.filter(p => p.category === filter);

            filtered.forEach(product => {
                const isInCart = cart.find(item => item.id === product.id);
                const card = document.createElement('div');
                card.className = 'product-card';
                card.innerHTML = `
                    <div class="product-image">
                        <img src="${product.image}" alt="${product.name}">
                    </div>
                    <div class="product-info">
                        <h3 class="product-title">${product.name}</h3>
                        <div class="product-price">$${product.price.toFixed(2)}</div>
                        <div class="product-actions">
                            <button class="add-to-cart" data-id="${product.id}">
                                <i class="fas fa-cart-plus"></i> ${isInCart ? 'Update Cart' : 'Add to Cart'}
                            </button>
                        </div>
                    </div>
                `;
                productGrid.appendChild(card);
            });

            document.querySelectorAll('.add-to-cart').forEach(btn => {
                btn.addEventListener('click', function() {
                    const id = parseInt(this.dataset.id);
                    addToCart(id, 1);
                });
            });
        }

        // ===== CART FUNCTIONS =====
        function addToCart(productId, quantity) {
            const product = products.find(p => p.id === productId);
            const existingIndex = cart.findIndex(item => item.id === productId);

            if (existingIndex > -1) {
                cart[existingIndex].quantity += quantity;
            } else {
                cart.push({
                    id: product.id,
                    name: product.name,
                    price: product.price,
                    image: product.image,
                    quantity: quantity
                });
            }

            localStorage.setItem('wetineCart', JSON.stringify(cart));
            updateCartDisplay();
            showNotification(`Added ${product.name} to cart`);
        }

        function updateCartDisplay() {
            const totalItems = cart.reduce((sum, item) => sum + item.quantity, 0);
            cartCount.textContent = totalItems;

            const totalPrice = cart.reduce((sum, item) => sum + (item.price * item.quantity), 0);
            cartTotalPrice.textContent = `$${totalPrice.toFixed(2)}`;

            renderCartItems();
        }

        function renderCartItems() {
            if (cart.length === 0) {
                cartItems.innerHTML = `<p style="text-align: center; padding: 40px 20px; color: #888;">Your cart is empty</p>`;
                return;
            }

            cartItems.innerHTML = '';
            cart.forEach(item => {
                const cartItem = document.createElement('div');
                cartItem.className = 'cart-item';
                cartItem.innerHTML = `
                    <div style="width: 80px; height: 80px; border-radius: 8px; overflow: hidden;">
                        <img src="${item.image}" alt="${item.name}" style="width:100%; height:100%; object-fit:cover;">
                    </div>
                    <div style="flex:1;">
                        <div style="font-weight:600;">${item.name}</div>
                        <div style="color: #2e7d32; font-weight:700; margin:5px 0;">$${item.price.toFixed(2)} each</div>
                        <div style="display:flex; justify-content:space-between; align-items:center; margin-top:10px;">
                            <div>
                                Qty: ${item.quantity}
                            </div>
                            <button class="remove-item" data-id="${item.id}" style="background:none; border:none; color:#e53e3e; cursor:pointer;">
                                <i class="fas fa-trash"></i>
                            </button>
                        </div>
                    </div>
                `;
                cartItems.appendChild(cartItem);
            });

            document.querySelectorAll('.remove-item').forEach(btn => {
                btn.addEventListener('click', function() {
                    const id = parseInt(this.dataset.id);
                    cart = cart.filter(item => item.id !== id);
                    localStorage.setItem('wetineCart', JSON.stringify(cart));
                    updateCartDisplay();
                    renderProducts(document.querySelector('.filter-btn.active').dataset.filter);
                });
            });
        }

        function toggleCart() {
            cartModal.classList.toggle('active');
            overlay.classList.toggle('active');
            document.body.style.overflow = cartModal.classList.contains('active') ? 'hidden' : 'auto';
        }

        // ===== WHATSAPP CHECKOUT =====
        function checkoutViaWhatsApp() {
            if (cart.length === 0) {
                showNotification('Your cart is empty');
                return;
            }

            let message = `*ORDER FROM WETINE ENTERPRISES WEBSITE*\n\n`;
            message += `*Order Details:*\n`;
            cart.forEach((item, index) => {
                message += `${index + 1}. ${item.name} - $${item.price.toFixed(2)} x ${item.quantity} = $${(item.price * item.quantity).toFixed(2)}\n`;
            });
            const totalPrice = cart.reduce((sum, item) => sum + (item.price * item.quantity), 0);
            message += `\n*Total Amount: $${totalPrice.toFixed(2)}*\n\n`;
            message += `Please confirm this order and provide delivery details.`;

            const encodedMessage = encodeURIComponent(message);
            const whatsappUrl = `https://wa.me/263788375175?text=${encodedMessage}`;
            window.open(whatsappUrl, '_blank');
        }

        // ===== UI HELPERS =====
        function showProductSection(e) {
            if (e) e.preventDefault();
            productSection.style.display = 'block';
            window.scrollTo({
                top: productSection.offsetTop - 80,
                behavior: 'smooth'
            });
            mainNav.classList.remove('active');
        }

        function showNotification(message) {
            const notification = document.createElement('div');
            notification.textContent = message;
            notification.style.cssText = `
                position: fixed;
                top: 100px;
                right: 20px;
                background-color: #2e7d32;
                color: white;
                padding: 15px 25px;
                border-radius: 5px;
                box-shadow: 0 5px 15px rgba(0,0,0,0.2);
                z-index: 2000;
                font-weight: 500;
                transform: translateX(120%);
                transition: transform 0.3s ease;
            `;
            document.body.appendChild(notification);
            setTimeout(() => notification.style.transform = 'translateX(0)', 10);
            setTimeout(() => {
                notification.style.transform = 'translateX(120%)';
                setTimeout(() => document.body.removeChild(notification), 300);
            }, 3000);
        }
    </script>
</body>
</html>
