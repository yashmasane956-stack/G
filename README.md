<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>The Iberian Pig | Modern Spanish Tapas</title>
    <style>
        /* --- CSS STYLES --- */
        :root {
            --primary: #8B0000; /* Deep Spanish Red */
            --secondary: #1a1a1a; /* Dark Gray */
            --gold: #D4AF37; /* Gold Accent */
            --light: #f4f4f4;
            --white: #ffffff;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Georgia', serif;
        }

        body {
            line-height: 1.6;
            color: #333;
            background-color: var(--light);
        }

        /* Navigation */
        nav {
            background: var(--secondary);
            padding: 1rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav .logo {
            color: var(--gold);
            font-size: 1.5rem;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        nav ul {
            list-style: none;
            display: flex;
        }

        nav ul li {
            margin-left: 2rem;
        }

        nav ul li a {
            color: var(--white);
            text-decoration: none;
            font-size: 0.9rem;
            text-transform: uppercase;
            transition: color 0.3s;
        }

        nav ul li a:hover {
            color: var(--gold);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.6)), url('https://images.unsplash.com/photo-1555396273-367ea4eb4db5?ixlib=rb-1.2.1&auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
            height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: var(--white);
            padding: 0 20px;
        }

        .hero h1 {
            font-size: 4rem;
            margin-bottom: 1rem;
            color: var(--gold);
        }

        .hero p {
            font-size: 1.5rem;
            margin-bottom: 2rem;
            font-style: italic;
        }

        .btn {
            background: var(--primary);
            color: var(--white);
            padding: 12px 30px;
            text-decoration: none;
            text-transform: uppercase;
            font-weight: bold;
            border: none;
            cursor: pointer;
            transition: background 0.3s;
        }

        .btn:hover {
            background: #a00000;
        }

        /* Sections */
        section {
            padding: 4rem 10%;
        }

        h2 {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
            color: var(--secondary);
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        /* Locations */
        .locations-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .location-card {
            background: var(--white);
            padding: 2rem;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            border-top: 4px solid var(--gold);
        }

        .location-card h3 {
            color: var(--primary);
            margin-bottom: 1rem;
        }

        .location-card .address {
            font-weight: bold;
            margin-bottom: 0.5rem;
        }

        .location-card .hours {
            font-size: 0.9rem;
            color: #666;
            margin: 1rem 0;
        }

        .coming-soon {
            background: var(--secondary);
            color: var(--white);
            text-align: center;
            padding: 2rem;
        }

        /* Menu */
        .menu-section {
            background: var(--white);
        }

        .menu-category {
            margin-bottom: 3rem;
        }

        .menu-category h3 {
            color: var(--primary);
            border-bottom: 2px solid var(--gold);
            display: inline-block;
            margin-bottom: 1.5rem;
        }

        .menu-items {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
        }

        .menu-item {
            border: 1px solid #eee;
            padding: 1rem;
            border-radius: 5px;
        }

        .menu-item h4 {
            font-size: 1.1rem;
            margin-bottom: 0.5rem;
        }

        .menu-item .price {
            color: var(--primary);
            font-weight: bold;
        }

        /* Events */
        .events-section {
            background: var(--secondary);
            color: var(--white);
        }

        .events-section h2 {
            color: var(--gold);
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .contact-card {
            text-align: center;
            padding: 2rem;
            border: 1px solid #444;
        }

        .contact-card h4 {
            color: var(--gold);
            margin-bottom: 1rem;
        }

        .contact-card a {
            color: var(--white);
            text-decoration: underline;
        }

        /* Footer */
        footer {
            background: #111;
            color: #888;
            text-align: center;
            padding: 2rem;
            font-size: 0.8rem;
        }

        /* Mobile */
        @media (max-width: 768px) {
            .hero h1 { font-size: 2.5rem; }
            .hero p { font-size: 1rem; }
            nav { flex-direction: column; gap: 1rem; }
            nav ul { flex-wrap: wrap; justify-content: center; }
            nav ul li { margin: 0 10px; }
        }
    </style>
</head>
<body>

    <!-- NAVIGATION -->
    <nav>
        <div class="logo">The Iberian Pig</div>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#locations">Locations</a></li>
            <li><a href="#menu">Menu</a></li>
            <li><a href="#events">Events</a></li>
        </ul>
    </nav>

    <!-- HERO SECTION -->
    <section id="home" class="hero">
        <h1>The Iberian Pig</h1>
        <p>Modern Spanish Tapas • Jamón Ibérico • Wine</p>
        <a href="#locations" class="btn">Find a Location</a>
    </section>

    <!-- LOCATIONS SECTION -->
    <section id="locations">
        <h2>Our Locations</h2>
        <div class="locations-grid">
            
            <!-- Decatur -->
            <div class="location-card">
                <h3>Decatur</h3>
                <p class="address">121 Sycamore Street<br>Decatur, GA 30030</p>
                <p class="phone">📞 (404) 371-8800</p>
                <div class="hours">
                    <p><strong>Sun:</strong> 4 PM – 10 PM</p>
                    <p><strong>Mon – Thu:</strong> 5 PM – 10 PM</p>
                    <p><strong>Fri:</strong> 5 PM – 11 PM</p>
                    <p><strong>Sat:</strong> 4 PM – 11 PM</p>
                </div>
                <p>✨ Dine-in • Takeout • Delivery • Private Dining</p>
            </div>

            <!-- Buckhead -->
            <div class="location-card">
                <h3>Buckhead</h3>
                <p class="address">3150 Roswell Rd NW<br>Atlanta, GA 30305</p>
                <p class="phone">📞 (404) 994-4990</p>
                <div class="hours">
                    <p><strong>Sun – Thu:</strong> 5 PM – 10 PM</p>
                    <p><strong>Fri – Sat:</strong> 4 PM – 11 PM</p>
                </div>
                <p>✨ Dine-in • Takeout • Valet Parking</p>
            </div>

            <!-- Nashville -->
            <div class="location-card">
                <h3>Nashville</h3>
                <p class="address">607 Overton Street<br>Nashville, TN 37203</p>
                <p class="phone">📞 (615) 844-4242</p>
                <div class="hours">
                    <p><strong>Mon – Thu:</strong> 4 PM – 10 PM</p>
                    <p><strong>Fri & Sat:</strong> 4 PM – 11 PM</p>
                    <p><strong>Sun:</strong> 4 PM – 9 PM</p>
                </div>
                <p>✨ Dine-in • Takeout</p>
            </div>

        </div>
        
        <!-- Charlotte Coming Soon -->
        <div class="coming-soon" style="margin-top: 2rem;">
            <h3>🍖 Charlotte, NC — Coming 2026</h3>
        </div>
    </section>

    <!-- MENU SECTION -->
    <section id="menu" class="menu-section">
        <h2>Menus</h2>
        
        <div class="menu-category">
            <h3>Starters & Tapas</h3>
            <div class="menu-items">
                <div class="menu-item">
                    <h4>Patatas Bravas</h4>
                    <span class="price">$50 (Catering)</span>
                </div>
                <div class="menu-item">
                    <h4>Marinated Spanish Olives</h4>
                    <span class="price">$30 (Catering)</span>
                </div>
                <div class="menu-item">
                    <h4>Bacon Wrapped Dates</h4>
                    <span class="price">From $30</span>
                </div>
                <div class="menu-item">
                    <h4>Empanadas de Carne</h4>
                    <span class="price">From $90</span>
                </div>
            </div>
        </div>

        <div class="menu-category">
            <h3>Charcuterie & Cheese</h3>
            <div class="menu-items">
                <div class="menu-item">
                    <h4>Cheese & Charcuterie Board</h4>
                    <p>Serves 10</p>
                    <span class="price">$150</span>
                </div>
                <div class="menu-item">
                    <h4>Jamón Ibérico Selection</h4>
                    <p>Authentic cured ham</p>
                </div>
            </div>
        </div>

        <div class="menu-category">
            <h3>Mains & Large Format</h3>
            <div class="menu-items">
                <div class="menu-item">
                    <h4>Paella</h4>
                    <span class="price">$100</span>
                </div>
                <div class="menu-item">
                    <h4>Ibérico Mac N' Cheese</h4>
                    <span class="price">$50</span>
                </div>
                <div class="menu-item">
                    <h4>Bistec</h4>
                    <span class="price">$100</span>
                </div>
                <div class="menu-item">
                    <h4>Costillas (Ribs)</h4>
                    <span class="price">$60</span>
                </div>
            </div>
        </div>
    </section>

    <!-- EVENTS SECTION -->
    <section id="events" class="events-section">
        <h2>Private Events & Catering</h2>
        <p style="text-align: center; margin-bottom: 2rem; max-width: 600px; margin-left: auto; margin-right: auto;">
            Host your next celebration at The Iberian Pig. From semi-private dinners to full restaurant buyouts, we create unforgettable experiences.
        </p>
        
        <div class="contact-grid">
            <div class="contact-card">
                <h4>Buckhead Private Events</h4>
                <p>Contact Christa White</p>
                <a href="mailto:cwhite@chgrestaurants.com">cwhite@chgrestaurants.com</a>
            </div>
            
            <div class="contact-card">
                <h4>Decatur Private Events</h4>
                <p>Contact Ash James</p>
                <a href="mailto:ajames@chgrestaurants.com">ajames@chgrestaurants.com</a>
            </div>
            
            <div class="contact-card">
                <h4>Nashville Private Events</h4>
                <p>Contact Amanda Styczek</p>
                <a href="mailto:astyczek@chgrestaurants.com">astyczek@chgrestaurants.com</a>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer>
        <p>&copy; 2024 The Iberian Pig. All Rights Reserved.</p>
        <p>Follow us on Social Media</p>
    </footer>

</body>
</html>
