# Jm-Tours-Transfers.github.io
Jm Tours&amp; Transfers Website
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>JM Tours & Transfers</title>
  <style>
    body {
      box-sizing: border-box;
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      line-height: 1.6;
      color: #333;
      background: #fff;
    }
    nav {
      position: fixed;
      top: 0;
      width: 100%;
      background: #004aad;
      padding: 15px;
      text-align: center;
      z-index: 1000;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }
    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s ease;
    }
    nav a:hover {
      color: #ff9900;
    }
    header {
      background: linear-gradient(rgba(0,74,173,0.7), rgba(0,74,173,0.7)), url('https://images.unsplash.com/photo-1578662996442-48f60103fc96?ixlib=rb-4.0.3&auto=format&fit=crop&w=2070&q=80') center/cover no-repeat;
      color: white;
      height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
      text-align: center;
      padding: 20px;
    }
    header h1 { 
      font-size: 3.5rem; 
      margin: 0; 
      text-shadow: 2px 2px 4px rgba(0,0,0,0.5);
    }
    header p { 
      font-size: 1.3rem; 
      margin: 10px 0 30px; 
      text-shadow: 1px 1px 2px rgba(0,0,0,0.5);
    }
    .btn {
      background: #ff9900;
      color: white;
      padding: 15px 30px;
      text-decoration: none;
      border-radius: 8px;
      margin: 8px;
      display: inline-block;
      font-weight: bold;
      transition: all 0.3s ease;
      box-shadow: 0 4px 15px rgba(255,153,0,0.3);
    }
    .btn:hover {
      background: #e68a00;
      transform: translateY(-2px);
      box-shadow: 0 6px 20px rgba(255,153,0,0.4);
    }
    section {
      padding: 80px 20px;
      max-width: 1200px;
      margin: auto;
    }
    section h2 {
      text-align: center;
      margin-bottom: 40px;
      color: #004aad;
      font-size: 2.5rem;
    }
    .services, .testimonials, .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 30px;
      margin-top: 40px;
    }
    .card {
      background: #f8f9fa;
      padding: 30px;
      border-radius: 15px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.1);
      text-align: center;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 10px 25px rgba(0,0,0,0.15);
    }
    .card h3 {
      color: #004aad;
      margin-bottom: 15px;
      font-size: 1.4rem;
    }
    .gallery img {
      width: 100%;
      border-radius: 15px;
      height: 250px;
      object-fit: cover;
      transition: transform 0.3s ease;
      cursor: pointer;
    }
    .gallery img:hover {
      transform: scale(1.05);
    }
    .testimonial {
      background: #fff;
      border-left: 4px solid #ff9900;
    }
    .testimonial .rating {
      color: #ff9900;
      font-size: 1.2rem;
      margin-bottom: 10px;
    }
    form {
      display: grid;
      gap: 20px;
      max-width: 600px;
      margin: auto;
      background: #f8f9fa;
      padding: 40px;
      border-radius: 15px;
      box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    }
    input, textarea, select, button {
      padding: 15px;
      border: 2px solid #e0e0e0;
      border-radius: 8px;
      font-size: 1rem;
      transition: border-color 0.3s ease;
    }
    input:focus, textarea:focus, select:focus {
      outline: none;
      border-color: #004aad;
    }
    button {
      background: #004aad;
      color: white;
      border: none;
      cursor: pointer;
      font-weight: bold;
      transition: background 0.3s ease;
    }
    button:hover {
      background: #003a8c;
    }
    footer {
      background: #004aad;
      color: white;
      text-align: center;
      padding: 40px 20px;
    }
    .footer-content {
      max-width: 1200px;
      margin: auto;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 30px;
      text-align: left;
    }
    .footer-section h3 {
      margin-bottom: 15px;
      color: #ff9900;
    }
    .footer-section p, .footer-section a {
      color: #ccc;
      text-decoration: none;
      margin: 5px 0;
    }
    .footer-section a:hover {
      color: #ff9900;
    }
    .success-message {
      background: #d4edda;
      color: #155724;
      padding: 15px;
      border-radius: 8px;
      margin: 20px 0;
      display: none;
    }
    @media (max-width: 768px) {
      header h1 { font-size: 2.5rem; }
      nav a { margin: 0 8px; font-size: 0.9rem; }
      section { padding: 60px 15px; }
    }
  </style>
</head>
<body>
  <!-- Navigation -->
  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#services">Services</a>
    <a href="#gallery">Gallery</a>
    <a href="#booking">Booking</a>
    <a href="#contact">Contact</a>
  </nav>

  <!-- Hero -->
  <header id="home">
    <h1>JM Tours & Transfers</h1>
    <p>Your trusted travel partner in Cape Town</p>
    <a href="#booking" class="btn">Book a Ride</a>
    <a href="#services" class="btn">Explore Tours</a>
  </header>

  <!-- About -->
  <section id="about">
    <h2>About Us</h2>
    <p style="text-align: center; font-size: 1.1rem; max-width: 800px; margin: auto;">
      JM Tours & Transfers offers safe, reliable, and comfortable transport services across Cape Town. 
      From airport transfers to scenic tours and custom itineraries, we're here to make your journey unforgettable.
      With over 10 years of experience, we pride ourselves on exceptional service and local expertise.
    </p>
  </section>

  <!-- Services -->
  <section id="services">
    <h2>Our Services</h2>
    <div class="services">
      <div class="card">
        <h3>🚗 Airport Transfers</h3>
        <p>On-time, stress-free pickups and drop-offs from Cape Town International Airport. Professional drivers and comfortable vehicles.</p>
      </div>
      <div class="card">
        <h3>🏛️ City Tours</h3>
        <p>Discover the beauty of Cape Town with guided tours of iconic attractions including Table Mountain and V&A Waterfront.</p>
      </div>
      <div class="card">
        <h3>🍷 Wine Route Tours</h3>
        <p>Experience the Cape Winelands with curated tours and luxury transport through Stellenbosch and Franschhoek.</p>
      </div>
      <div class="card">
        <h3>📋 Custom Itineraries</h3>
        <p>Personalized travel experiences tailored to your schedule and interests. Let us create your perfect Cape Town adventure.</p>
      </div>
    </div>
  </section>

  <!-- Gallery -->
  <section id="gallery">
    <h2>Gallery</h2>
    <div class="gallery">
      <img src="https://images.unsplash.com/photo-1580500550469-4e3d29e541c4?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Table Mountain Cape Town" onerror="this.src=''; this.alt='Image failed to load'; this.style.display='none';">
      <img src="https://images.unsplash.com/photo-1563656353898-febc9270a0f4?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Cape Town Waterfront" onerror="this.src=''; this.alt='Image failed to load'; this.style.display='none';">
      <img src="https://images.unsplash.com/photo-1539650116574-75c0c6d73f6e?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Cape Winelands" onerror="this.src=''; this.alt='Image failed to load'; this.style.display='none';">
      <img src="https://images.unsplash.com/photo-1578662996442-48f60103fc96?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Cape Town Coastline" onerror="this.src=''; this.alt='Image failed to load'; this.style.display='none';">
      <img src="https://images.unsplash.com/photo-1577717903315-1691ae25ab3f?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Luxury Transport Vehicle" onerror="this.src=''; this.alt='Image failed to load'; this.style.display='none';">
      <img src="https://images.unsplash.com/photo-1506905925346-21bda4d32df4?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Cape Point" onerror="this.src=''; this.alt='Image failed to load'; this.style.display='none';">
    </div>
  </section>

  <!-- Testimonials -->
  <section>
    <h2>What Our Clients Say</h2>
    <div class="testimonials">
      <div class="card testimonial">
        <div class="rating">⭐⭐⭐⭐⭐</div>
        <p>"Exceptional service! JM Tours made our Cape Town visit unforgettable. Professional, punctual, and very knowledgeable about local attractions."</p>
        <strong>- Sarah Johnson, UK</strong>
      </div>
      <div class="card testimonial">
        <div class="rating">⭐⭐⭐⭐⭐</div>
        <p>"Best airport transfer service in Cape Town. Clean vehicles, friendly drivers, and always on time. Highly recommended!"</p>
        <strong>- Michael Chen, Australia</strong>
      </div>
      <div class="card testimonial">
        <div class="rating">⭐⭐⭐⭐⭐</div>
        <p>"The wine tour was absolutely amazing. Our guide was fantastic and the whole experience exceeded our expectations."</p>
        <strong>- Emma Rodriguez, Spain</strong>
      </div>
    </div>
  </section>

  <!-- Booking -->
  <section id="booking">
    <h2>Book Your Journey</h2>
    <div class="success-message" id="successMessage">
      Thank you for your booking request! We'll contact you within 24 hours to confirm your reservation.
    </div>
    <form id="bookingForm">
      <input type="text" placeholder="Full Name" required>
      <input type="email" placeholder="Email Address" required>
      <input type="tel" placeholder="Phone Number" required>
      <select required>
        <option value="">Select Service</option>
        <option value="airport">Airport Transfer</option>
        <option value="city">City Tour</option>
        <option value="wine">Wine Route Tour</option>
        <option value="custom">Custom Itinerary</option>
      </select>
      <input type="date" required>
      <input type="time" required>
      <input type="number" placeholder="Number of Passengers" min="1" max="8" required>
      <textarea placeholder="Special Requirements or Additional Information" rows="4"></textarea>
      <button type="submit">Submit Booking Request</button>
    </form>
  </section>

  <!-- Contact -->
  <section id="contact">
    <h2>Contact Us</h2>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 40px; text-align: center;">
      <div class="card">
        <h3>📞 Phone</h3>
        <p>+27 21 123 4567</p>
        <p>Available 24/7</p>
      </div>
      <div class="card">
        <h3>📧 Email</h3>
        <p>info@jmtours.co.za</p>
        <p>bookings@jmtours.co.za</p>
      </div>
      <div class="card">
        <h3>📍 Location</h3>
        <p>Cape Town, South Africa</p>
        <p>Serving the Western Cape</p>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    <div class="footer-content">
      <div class="footer-section">
        <h3>JM Tours & Transfers</h3>
        <p>Your trusted travel partner in Cape Town, providing safe and reliable transport services since 2013.</p>
      </div>
      <div class="footer-section">
        <h3>Quick Links</h3>
        <a href="#services">Our Services</a><br>
        <a href="#booking">Book Now</a><br>
        <a href="#gallery">Gallery</a><br>
        <a href="#contact">Contact Us</a>
      </div>
      <div class="footer-section">
        <h3>Contact Info</h3>
        <p>📞 +27 21 123 4567</p>
        <p>📧 info@jmtours.co.za</p>
        <p>📍 Cape Town, South Africa</p>
      </div>
    </div>
    <div style="text-align: center; margin-top: 30px; padding-top: 20px; border-top: 1px solid #555;">
      <p>&copy; 2024 JM Tours & Transfers. All rights reserved.</p>
    </div>
  </footer>

  <script>
    // Smooth scrolling for navigation links
    document.querySelectorAll('nav a[href^="#"]').forEach(anchor => {
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

    // Header button smooth scrolling
    document.querySelectorAll('header a[href^="#"]').forEach(anchor => {
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

    // Booking form submission
    document.getElementById('bookingForm').addEventListener('submit', function(e) {
      e.preventDefault();
      
      // Show success message
      const successMessage = document.getElementById('successMessage');
      successMessage.style.display = 'block';
      
      // Reset form
      this.reset();
      
      // Scroll to success message
      successMessage.scrollIntoView({
        behavior: 'smooth',
        block: 'center'
      });
      
      // Hide success message after 5 seconds
      setTimeout(() => {
        successMessage.style.display = 'none';
      }, 5000);
    });

    // Gallery image click to enlarge (simple version)
    document.querySelectorAll('.gallery img').forEach(img => {
      img.addEventListener('click', function() {
        window.open(this.src, '_blank', 'noopener,noreferrer');
      });
    });

    // Add active navigation highlighting
    window.addEventListener('scroll', function() {
      const sections = document.querySelectorAll('section, header');
      const navLinks = document.querySelectorAll('nav a');
      
      let current = '';
      sections.forEach(section => {
        const sectionTop = section.offsetTop - 100;
        if (pageYOffset >= sectionTop) {
          current = section.getAttribute('id');
        }
      });

      navLinks.forEach(link => {
        link.style.color = '';
        if (link.getAttribute('href') === '#' + current) {
          link.style.color = '#ff9900';
        }
      });
    });
  </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'986c15d915644fb0',t:'MTc1OTE1NTI1MC4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
