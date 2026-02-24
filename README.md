# Ex02 Commercial Website
## Date:23/02/2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM

```
index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Laptop Store</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
</head>
<body>

<!-- Navigation -->
<header>
    <div class="logo">LaptopHub</div>
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#products">Laptops</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#contact">Contact</a></li>
            <li><a href="#account">Account</a></li>
        </ul>
    </nav>
</header>

<!-- Homepage -->
<section id="home" class="section hero">
    <h1>IPLANET</h1>
    <p>Best deals on top brands with fast delivery.</p>
    </section>

<!-- Products Section -->
<section id="products" class="section">
    <h2>Featured Laptops</h2>
    <div class="flex-container">

        <div class="card">
            <img src="gaming_laptops_img.webp" alt="Gaming Laptop">
            <h3>Gaming Pro X</h3>
            <p>16GB RAM | 1TB SSD | RTX Graphics</p>
            <p class="price">75,299</p>
            <button>Buy Now</button>
        </div>

        <div class="card">
            <img src="lap 1.jpg" alt="Business Laptop">
            <h3>Business Elite</h3>
            <p>8GB RAM | 512GB SSD | Intel i7</p>
            <p class="price">55,999</p>
            <button>Buy Now</button>
        </div>

        <div class="card">
            <img src="lap apple.jpg" alt="Student Laptop">
            <h3>Student Air</h3>
            <p>8GB RAM | 256GB SSD | Lightweight</p>
            <p class="price">39,999</p>
            <button>Buy Now</button>
        </div>

    </div>
</section>

<!-- About -->
<section id="about" class="section">
    <h2>About LaptopHub</h2>
    <p>We provide high-quality laptops at competitive prices with secure checkout and fast shipping.</p>
</section>

<!-- Contact -->
<section id="contact" class="section">
    <h2>Contact Us</h2>
    <p>Email: vichuvishva2007@gmail.com</p>
    <p>Phone: +91 8870955014</p>
</section>

<!-- User Account -->
<section id="account" class="section">
    <h2>Login / Register</h2>
    <form>
        <input type="email" placeholder="Email" required>
        <input type="password" placeholder="Password" required>
        <button type="submit">Login</button>
    </form>
</section>

<!-- Footer -->
<footer>
    <div class="social-links">
        <a href="#">Facebook</a>
        <a href="#">Twitter</a>
        <a href="#">Instagram</a>
    </div>
    <p>© 2026 LaptopHub. All Rights Reserved.</p>
</footer>

</body>
</html>
```
```
style.css

/* Global Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    background: #f4f6f9;
    color: #333;
}

.section {
    padding: 70px 20px;
    text-align: center;
}

/* Header */
header {
    background: #111827;
    color: white;
    padding: 15px 40px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 24px;
    font-weight: bold;
}

nav ul {
    list-style: none;
    display: flex;
}

nav ul li {
    margin-left: 25px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    transition: 0.3s;
}

nav ul li a:hover {
    color: #3b82f6;
}

/* Hero */
.hero img {
    width: 60%;
    margin-top: 20px;
}

/* Flexbox Layout */
.flex-container {
    display: flex;
    justify-content: center;
    gap: 30px;
    flex-wrap: wrap;
    margin-top: 40px;
}

/* Product Cards */
.card {
    background: white;
    width: 280px;
    padding: 20px;
    border-radius: 12px;
    box-shadow: 0 6px 15px rgba(0,0,0,0.08);
    transition: transform 0.3s, box-shadow 0.3s;
}

.card img {
    width: 100%;
    border-radius: 10px;
}

.price {
    font-size: 20px;
    color: #3b82f6;
    margin: 10px 0;
    font-weight: bold;
}

.card button {
    padding: 10px 20px;
    border: none;
    background: #3b82f6;
    color: white;
    cursor: pointer;
    border-radius: 6px;
    transition: 0.3s;
}

.card button:hover {
    background: #1e40af;
}

/* Hover Effect */
.card:hover {
    transform: translateY(-8px);
    box-shadow: 0 12px 25px rgba(0,0,0,0.15);
}

/* Form */
form {
    display: flex;
    flex-direction: column;
    align-items: center;
}

form input {
    width: 260px;
    padding: 10px;
    margin: 10px 0;
}

form button {
    padding: 10px 25px;
    background: #3b82f6;
    border: none;
    color: white;
    cursor: pointer;
    border-radius: 6px;
}

form button:hover {
    background: #1e40af;
}

/* Footer */
footer {
    background: #111827;
    color: white;
    padding: 25px;
    text-align: center;
}

.social-links a {
    margin: 0 12px;
    color: white;
    text-decoration: none;
    transition: 0.3s;
}

.social-links a:hover {
    color: #3b82f6;
}
```

## OUTPUT

![alt text](<Screenshot 2026-02-23 161248.png>)
![alt text](<Screenshot 2026-02-23 161446.png>)

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
