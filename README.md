<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wetine Enterprises | Quality Hardware & Electronics</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-dark-blue: #1e3a8a;    /* Main brand dark blue */
            --dark-blue: #1d366b;           /* Darker shade for hover states */
            --light-blue: #e0f2fe;          /* Light tint for backgrounds */
            --accent-amber: #ff8f00;        /* Accent color for highlights */
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
            color: var(--primary-dark-blue);
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
            color: var(--primary-dark-blue);
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
            background: linear-gradient(rgba(30, 58, 138, 0.9), rgba(29, 54, 107, 0.9)), url('https://images.unsplash.com/photo-1581094715295-bf7d63bd5c44?ixlib=rb-4.0.3&auto=format&fit=crop&w=1600&q=80');
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
            color: var(--primary-dark-blue);
            padding: 15px 35px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 600;
            font-size: 1.1rem;
            transition: all 0.3s ease;
        }
        .cta-button:hover {
            background-color: var(--light-blue);
            transform: translateY(-3px);
        }
        /* Services/Products Section */
        .services {
            padding: 100px 
