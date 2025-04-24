# PlayFin-website
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>PlayFin - Empower Your Finances</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <nav class="navbar">
      <a href="#" class="logo">
        <img src="assets/logo-placeholder.png" alt="PlayFin Logo">
      </a>
      <ul class="nav-links">
        <li><a href="#about">About</a></li>
        <li><a href="#features">Features</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <!-- Hero Section -->
    <section id="hero">
      <div class="hero-content">
        <h1>Welcome to PlayFin</h1>
        <p>Empowering your financial journey with innovation and simplicity.</p>
        <button class="cta-button">Get Started</button>
      </div>
    </section>

    <!-- About Section -->
    <section id="about">
      <h2>About PlayFin</h2>
      <p>PlayFin is your companion for smarter financial decisions. We simplify, organize, and empower you to achieve your goals.</p>
      <img src="assets/about-placeholder.jpg" alt="About PlayFin">
    </section>

    <!-- Features Section -->
    <section id="features">
      <h2>Key Features</h2>
      <div class="feature-list">
        <div class="feature-item">
          <h3>Track Expenses</h3>
          <p>Monitor your spending habits with ease.</p>
        </div>
        <div class="feature-item">
          <h3>Smart Insights</h3>
          <p>Get personalized tips to save more.</p>
        </div>
        <div class="feature-item">
          <h3>Secure Payments</h3>
          <p>Experience seamless and safe transactions.</p>
        </div>
      </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
      <h2>Contact Us</h2>
      <p>Have questions? We’d love to hear from you!</p>
      <form>
        <input type="text" placeholder="Your Name" required>
        <input type="email" placeholder="Your Email" required>
        <textarea placeholder="Your Message" required></textarea>
        <button type="submit">Send Message</button>
      </form>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 PlayFin. All rights reserved.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
/* General Styles */
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* Navigation Bar */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
  background-color: #2c3e50;
  color: white;
}

.nav-links {
  list-style: none;
  display: flex;
}

.nav-links li {
  margin: 0 15px;
}

.nav-links a {
  color: white;
  text-decoration: none;
  transition: color 0.3s;
}

.nav-links a:hover {
  color: #3498db;
}

.logo img {
  max-height: 50px;
}

/* Hero Section */
#hero {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 100vh;
  background: linear-gradient(to right, #3498db, #2c3e50);
  color: white;
  text-align: center;
}

.cta-button {
  margin-top: 20px;
  padding: 10px 20px;
  background-color: #e74c3c;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  transition: transform 0.3s ease;
}

.cta-button:hover {
  transform: scale(1.1);
}

/* Sections */
section {
  padding: 50px;
  text-align: center;
}

#about img {
  max-width: 100%;
  height: auto;
  margin-top: 20px;
}

.feature-list {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 20px;
  margin-top: 20px;
}

.feature-item {
  background-color: #ecf0f1;
  padding: 20px;
  border-radius: 10px;
  width: 300px;
}

.feature-item h3 {
  color: #2c3e50;
}

/* Footer */
footer {
  text-align: center;
  padding: 20px;
  background-color: #2c3e50;
  color: white;
}
// JavaScript for Interactivity

// Smooth scrolling for navigation links
document.querySelectorAll('.nav-links a').forEach(link => {
  link.addEventListener('click', function(event) {
    event.preventDefault();
    const targetId = this.getAttribute('href').substring(1);
    document.getElementById(targetId).scrollIntoView({ behavior: 'smooth' });
  });
});

// Add interactivity to the "Get Started" button
document.querySelector('.cta-button').addEventListener('click', () => {
  alert('Welcome to PlayFin! Let’s get started.');
});
