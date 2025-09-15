# errands---buddy---ke
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Errands Buddy KE</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Errands Buddy KE</h1>
    <nav>
      <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section id="hero">
    <h2>Your Reliable Partner for Everyday Tasks</h2>
    <p>We help you save time and focus on what matters most.</p>
    <a href="#contact" class="btn">Get Started</a>
  </section>

  <section id="about">
    <h2>About Us</h2>
    <p>Errands Buddy KE is your trusted assistant for all your personal and business errands. Whether it’s shopping, deliveries, or administrative support, we’ve got you covered!</p>
  </section>

  <section id="services">
    <h2>Our Services</h2>
    <div class="service">
      <h3>🛒 Shopping & Delivery</h3>
      <p>We handle your shopping and deliver items right to your doorstep.</p>
    </div>
    <div class="service">
      <h3>📑 Administrative Support</h3>
      <p>From paperwork to organizing schedules, we keep you stress-free.</p>
    </div>
    <div class="service">
      <h3>🚗 Errand Running</h3>
      <p>Need something picked or dropped? We run errands so you don’t have to.</p>
    </div>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <form id="contactForm">
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea placeholder="Your Message" required></textarea>
      <button type="submit">Send</button>
    </form>
    <p id="formMessage"></p>
  </section>

  <footer>
    <p>© 2025 Errands Buddy KE | Designed with ❤️</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>

/* General Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  color: #333;
}

/* Header */
header {
  background: #2c3e50;
  color: white;
  padding: 1rem;
  text-align: center;
}

nav ul {
  list-style: none;
  display: flex;
  justify-content: center;
  margin-top: 10px;
}

nav ul li {
  margin: 0 15px;
}

nav ul li a {
  color: white;
  text-decoration: none;
  font-weight: bold;
}

nav ul li a:hover {
  text-decoration: underline;
}

/* Hero Section */
#hero {
  background: #27ae60;
  color: white;
  text-align: center;
  padding: 3rem 1rem;
}

#hero h2 {
  margin-bottom: 1rem;
}

.btn {
  display: inline-block;
  background: white;
  color: #27ae60;
  padding: 10px 20px;
  margin-top: 1rem;
  border-radius: 5px;
  text-decoration: none;
  font-weight: bold;
}

.btn:hover {
  background: #f1f1f1;
}

/* Sections */
section {
  padding: 2rem 1rem;
  text-align: center;
}

.service {
  margin: 1rem 0;
  padding: 1rem;
  border: 1px solid #ddd;
  border-radius: 8px;
}

/* Contact Form */
form {
  display: flex;
  flex-direction: column;
  width: 80%;
  max-width: 500px;
  margin: auto;
}

form input, form textarea, form button {
  margin: 10px 0;
  padding: 10px;
  border-radius: 5px;
  border: 1px solid #ccc;
}

form button {
  background: #27ae60;
  color: white;
  border: none;
  cursor: pointer;
}

form button:hover {
  background: #219150;
}

/* Footer */
footer {
  background: #2c3e50;
  color: white;
  text-align: center;
  padding: 1rem;
  margin-top: 20px;
}


document.getElementById("contactForm").addEventListener("submit", function(e) {
  e.preventDefault();
  document.getElementById("formMessage").innerText = "✅ Thank you for reaching out! We'll get back to you shortly.";
  this.reset();
});

