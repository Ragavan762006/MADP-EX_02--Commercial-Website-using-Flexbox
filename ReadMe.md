# Ex02 Commercial Website
## Date:10-8-2025

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
## index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flexbox Commercial Website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header class="header">
        <div class="logo">WoodShop</div>
        <nav class="nav">
    <a href="index.html">Home</a>
    <a href="products.html">Products</a>
    <a href="about.html">About</a>
    <a href="contact.html">Contact</a>
</nav>

    </header>
    <section class="hero">
        <h1>Welcome to WoodWorld</h1>
        <p>Quality products at unbeatable prices.</p>
        <a href="https://www.woodsala.com/" class="btn" target="_blank">Visit Now</a>
    </section>

    <section class="products">
        <div class="product-card">
            <img src="product1.avif" alt="Product 1">
            <h3>Product 1</h3>
            <p>High-quality and affordable.</p>
            <a href="https://razorpay.com/payment-links/?" class="btn">Buy Now</a>
        </div>
        <div class="product-card">
            <img src="product2.jpg" alt="Product 2">
            <h3>Product 2</h3>
            <p>Designed for everyday use.</p>
            <a href="https://razorpay.com/payment-links/?" class="btn">Buy Now</a>
        </div>
        <div class="product-card">
            <img src="product3.jpeg" alt="Product 3">
            <h3>Product 3</h3>
            <p>Durable and stylish.</p>
            <a href="https://razorpay.com/payment-links/?" class="btn">Buy Now</a>
        </div>
    </section>

    <footer class="footer">
        <p>&copy; 2025 WoodShop. All rights reserved.</p>
    </footer>

</body>
</html>

```
## products.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Products - WoodShop</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header>
        <div class="logo">WoodShop</div>
        <nav>
            <a href="index.html">Home</a>
            <a href="products.html" class="active">Products</a>
            <a href="about.html">About</a>
            <a href="contact.html">Contact</a>
        </nav>
    </header>

    <section class="products-section">
        <h1>Our Products</h1>
        <div class="product-container">
            <div class="product-card">
                <img src="p1.jpg" alt="Product 1">
                <h3>Product 1</h3>
                <p>High-quality and affordable.</p>
                <button>Buy Now</button>
            </div>

            <div class="product-card">
                <img src="p2.jpg" alt="Product 2">
                <h3>Product 2</h3>
                <p>Designed for everyday use.</p>
                <button>Buy Now</button>
            </div>

            <div class="product-card">
                <img src="p3.jpg" alt="Product 3">
                <h3>Product 3</h3>
                <p>Durable and stylish.</p>
                <button>Buy Now</button>
            </div>
        </div>
    </section>

    <footer>
        <p>© 2025 WoodShop. All rights reserved.</p>
    </footer>

</body>
</html>

```
## about.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About - WoodShop</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <div class="logo">WoodShop</div>
        <nav>
            <a href="index.html">Home</a>
            <a href="products.html">Products</a>
            <a href="about.html" class="active">About</a>
            <a href="contact.html">Contact</a>
        </nav>
    </header>

    <section class="about-section">
        <h1>About Us</h1>
        <p>
            Welcome to <strong>WoodShop</strong> – your one-stop destination for premium quality wooden products.
            We pride ourselves on craftsmanship, sustainability, and delivering unbeatable value to our customers.
        </p>
        <p>
            Our mission is to bring warmth and elegance to your home with unique, handcrafted wooden items.
            From functional kitchen boards to stylish furniture, every product is made with care.
        </p>
    </section>

    <footer>
        <p>© 2025 WoodShop. All rights reserved.</p>
    </footer>

</body>
</html>

```
## style.css
```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
}

.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px 30px;
    background-color: #222;
    color: white;
}
.header .nav a {
    color: white;
    text-decoration: none;
    margin-left: 20px;
}
.header .nav a:hover {
    text-decoration: underline;
}

.hero {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    background: linear-gradient(to right, #4facfe, #00f2fe);
    height: 350px;
    color: white;
    text-align: center;
    padding: 20px;
}
.hero .btn {
    display: inline-block;
    margin-top: 20px;
    padding: 10px 20px;
    background-color: white;
    color: #333;
    text-decoration: none;
    border-radius: 4px;
}
.hero .btn:hover {
    background-color: #f1f1f1;
}

.products {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
    padding: 40px 20px;
    background-color: #f9f9f9;
}
.product-card {
    background: white;
    border-radius: 8px;
    padding: 20px;
    width: 250px;
    margin: 10px;
    text-align: center;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}
.product-card img {
    max-width: 100%;
    border-radius: 5px;
}
.product-card .btn {
    display: inline-block;
    margin-top: 10px;
    padding: 8px 15px;
    background-color: #4facfe;
    color: white;
    text-decoration: none;
    border-radius: 4px;
}
.product-card .btn:hover {
    background-color: #3a9bdc;
}
.footer {
    text-align: center;
    padding: 15px;
    background-color: #222;
    color: white;
}
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
}

body {
    background-color: #f8f8f8;
    color: #333;
}

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #111;
    padding: 15px 30px;
}

.logo {
    color: white;
    font-size: 1.4rem;
    font-weight: bold;
}

nav a {
    color: white;
    text-decoration: none;
    margin-left: 20px;
    font-size: 1rem;
    transition: color 0.3s ease;
}

nav a:hover,
nav a.active {
    color: #00bfff;
}

.hero {
    background: linear-gradient(90deg, #4facfe, #00f2fe);
    color: white;
    text-align: center;
    padding: 60px 20px;
}

.hero h1 {
    font-size: 2rem;
    margin-bottom: 10px;
}

.hero p {
    margin-bottom: 20px;
}

.hero button {
    background-color: white;
    color: black;
    padding: 10px 20px;
    border: none;
    border-radius: 4px;
    font-size: 1rem;
    cursor: pointer;
    transition: background 0.3s ease;
}

.hero button:hover {
    background-color: #ddd;
}

.products-section {
    padding: 40px 20px;
    text-align: center;
}

.products-section h1 {
    margin-bottom: 30px;
    font-size: 2rem;
}

.product-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 20px;
}

.product-card {
    background: white;
    border-radius: 8px;
    padding: 20px;
    width: 280px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    text-align: center;
    transition: transform 0.3s ease;
}

.product-card:hover {
    transform: translateY(-5px);
}

.product-card img {
    width: 100%;
    border-radius: 6px;
    margin-bottom: 10px;
}

.product-card h3 {
    margin-bottom: 5px;
}

.product-card p {
    font-size: 0.9rem;
    margin-bottom: 15px;
}

.product-card button {
    background-color: #4facfe;
    color: white;
    padding: 8px 15px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    transition: background 0.3s ease;
}

.product-card button:hover {
    background-color: #00bfff;
}
/* Reset & Base */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body {
    font-family: Arial, sans-serif;
    background-color: #f8f8f8;
}


header {
    background-color: #111;
    color: white;
    padding: 15px 30px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.logo {
    font-size: 1.4rem;
    font-weight: bold;
}
nav a {
    color: white;
    text-decoration: none;
    margin-left: 20px;
}
nav a.active {
    color: #00bfff;
}
nav a:hover {
    color: #00bfff;
}
.about-section {
    min-height: calc(100vh - 120px);
    background: linear-gradient(90deg, #4facfe, #00f2fe);
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 40px;
    color: white;
    text-align: center;
}
.about-content {
    max-width: 800px;
}
.about-content h1 {
    font-size: 2.5rem;
    margin-bottom: 20px;
}
.about-content p {
    margin-bottom: 15px;
    font-size:35px;
    line-height: 1.6;
}

footer {
    background-color: #111;
    color: white;
    text-align: center;
    padding: 10px;
}

```
## OUTPUT
![WhatsApp Image 2025-08-11 at 08 03 47_b8762086](https://github.com/user-attachments/assets/a277695b-c283-4b87-aa59-12f2ff1ae9a1)
![WhatsApp Image 2025-08-11 at 08 03 47_b728cbfd](https://github.com/user-attachments/assets/5104e6a6-fe52-46f5-8cfd-037ffe152457)


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
