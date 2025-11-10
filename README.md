<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>DECA Store</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: 'Poppins', sans-serif;
      color: #222;
      background-color: #fff;
    }

    header {
      background-color: #c40000;
      color: white;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 1rem 2rem;
      position: sticky;
      top: 0;
      z-index: 10;
    }

    header h1 {
      font-size: 1.8rem;
      font-weight: 700;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin-left: 1.5rem;
      font-weight: 500;
      transition: 0.3s;
    }

    nav a:hover {
      color: #ffd6d6;
    }

    section {
      padding: 4rem 2rem;
      max-width: 900px;
      margin: auto;
      text-align: center;
    }

    #home {
      background-color: #fff5f5;
      border-bottom: 4px solid #c40000;
    }

    #home h2 {
      color: #c40000;
      font-size: 2.5rem;
      margin-bottom: 1rem;
    }

    #home p {
      font-size: 1.2rem;
      margin-bottom: 2rem;
    }

    .btn {
      background-color: #c40000;
      color: white;
      padding: 0.8rem 1.5rem;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      font-size: 1rem;
      transition: 0.3s;
    }

    .btn:hover {
      background-color: #a30000;
    }

    #about h2, #contact h2 {
      color: #c40000;
      font-size: 2rem;
      margin-bottom: 1rem;
    }

    #about p {
      font-size: 1.1rem;
      line-height: 1.6;
      margin-bottom: 1rem;
    }

    .products {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1.5rem;
      margin-top: 2rem;
    }

    .product {
      background: white;
      border: 2px solid #c40000;
      border-radius: 10px;
      padding: 1rem;
      width: 220px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      transition: transform 0.3s;
    }

    .product:hover {
      transform: scale(1.05);
    }

    .product img {
      width: 100%;
      border-radius: 8px;
      margin-bottom: 0.5rem;
    }

    footer {
      background-color: #c40000;
      color: white;
      text-align: center;
      padding: 1rem;
      margin-top: 3rem;
    }

    form {
      display: flex;
      flex-direction: column;
      gap: 1rem;
      max-width: 400px;
      margin: 2rem auto 0;
    }

    input, textarea {
      padding: 0.8rem;
      border: 2px solid #c40000;
      border-radius: 6px;
      font-size: 1rem;
      width: 100%;
    }

    textarea {
      resize: none;
      height: 100px;
    }

    @media (max-width: 600px) {
      nav a {
        margin-left: 1rem;
        font-size: 0.9rem;
      }
      .product {
        width: 90%;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>DECA Store</h1>
    <nav>
      <a href="#home">Home</a>
      <a href="#about">About Us</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section id="home">
    <h2>Welcome to the DECA Store!</h2>
    <p>Your one-stop shop for DECA merch, snacks, and school spirit!</p>
    <button class="btn" onclick="document.getElementById('about').scrollIntoView({behavior: 'smooth'})">Learn More</button>

    <div class="products">
      <div class="product">
        <img src="https://via.placeholder.com/220x150?text=DECA+T-Shirt" alt="DECA T-Shirt">
        <h3>DECA T-Shirt</h3>
        <p>$15.00</p>
      </div>
      <div class="product">
        <img src="https://via.placeholder.com/220x150?text=Hoodie" alt="DECA Hoodie">
        <h3>DECA Hoodie</h3>
        <p>$25.00</p>
      </div>
      <div class="product">
        <img src="https://via.placeholder.com/220x150?text=Snacks" alt="Snacks">
        <h3>Snacks</h3>
        <p>Starting at $1.00</p>
      </div>
    </div>
  </section>

  <section id="about">
    <h2>About Us</h2>
    <p>The DECA Store is run by our school’s DECA chapter to promote entrepreneurship and leadership. We’re dedicated to bringing spirit, quality products, and tasty snacks to our students and staff.</p>
    <p>All proceeds help fund DECA events, competitions, and community projects. Every purchase supports our members’ growth as future business leaders!</p>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <p>Have questions or want to place an order? Reach out to us below!</p>

    <form>
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email" required />
      <textarea placeholder="Your Message" required></textarea>
      <button class="btn" type="submit">Send Message</button>
    </form>
  </section>

  <footer>
    <p>© 2025 DECA Store | All Rights Reserved</p>
  </footer>
</body>
</html>
