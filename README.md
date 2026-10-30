# Ex02 Commercial Website
## Date:30/10/2026

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

index.html

```
<!DOCTYPE html>
<html>
<head>
    <title>ShopHub - Online Shopping</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>

<header>
    <h1>ShopHub.</h1>
    <p>Everything You Love, All in One Place!</p>
</header>

<nav>
    <a href="#home">Home</a>
    <a href="#products">Products</a>
    <a href="#about">About Us</a>
    <a href="#contact">Contact</a>
    <a href="#account">Account</a>
    <a href="#cart">🛒 Cart (<span id="count">0</span>)</a>
</nav>

<section id="home" class="welcome">
    <h2>Welcome to ShopHub!</h2>
    <h3>Discover Your Style, Shop Your Happiness.</h3>
    <p>Explore amazing products at affordable prices.</p>
    <a href="#products" class="shop">Shop Now</a>
</section>

<section id="products">
    <h2>✨ Our Trending Products ✨</h2>

    <div class="container">

        <div class="product">
            <img src="https://images.unsplash.com/photo-1539109136881-3be0616acf4b?w=400" alt="Dress">
            <h3>Women's Dress</h3>
            <p>₹999</p>
            <button onclick="addCart()">Add to Cart</button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1594633312681-425c7b97ccd1?w=400" alt="Kurti">
            <h3>Designer Kurti</h3>
            <p>₹799</p>
            <button onclick="addCart()">Add to Cart</button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1585487000160-6ebcfceb0d03?w=400" alt="Saree">
            <h3>Traditional Saree</h3>
            <p>₹1499</p>
            <button onclick="addCart()">Add to Cart</button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1590736969955-71cc94901144?w=400" alt="Abaya">
            <h3>Elegant Abaya</h3>
            <p>₹1299</p>
            <button onclick="addCart()">Add to Cart</button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1542291026-7eec264c27ff?w=400" alt="Shoes">
            <h3>Sports Shoes</h3>
            <p>₹1199</p>
            <button onclick="addCart()">Add to Cart</button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1548036328-c9fa89d128fa?w=400" alt="Handbag">
            <h3>Stylish Handbag</h3>
            <p>₹899</p>
            <button onclick="addCart()">Add to Cart</button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30?w=400" alt="Watch">
            <h3>Luxury Watch</h3>
            <p>₹699</p>
            <button onclick="addCart()">Add to Cart</button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1505740420928-5e560c06d30e?w=400" alt="Headphones">
            <h3>Headphones</h3>
            <p>₹1499</p>
            <button onclick="addCart()">Add to Cart</button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1541643600914-78b084683601?w=400" alt="Perfume">
            <h3>Luxury Perfume</h3>
            <p>₹599</p>
            <button onclick="addCart()">Add to Cart</button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1526170375885-4d8ecf77b99f?w=400" alt="Camera">
            <h3>Digital Camera</h3>
            <p>₹2499</p>
            <button onclick="addCart()">Add to Cart</button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1571781926291-c477ebfd024b?w=400" alt="Beauty">
            <h3>Beauty Products</h3>
            <p>₹499</p>
            <button onclick="addCart()">Add to Cart</button>
        </div>

        <div class="product">
            <img src="https://images.unsplash.com/photo-1511499767150-a48a237f0083?w=400" alt="Sunglasses">
            <h3>Stylish Sunglasses</h3>
            <p>₹399</p>
            <button onclick="addCart()">Add to Cart</button>
        </div>

    </div>
</section>

<section id="about">
    <h2>About ShopHub</h2>
    <p>ShopHub is your one-stop online shopping destination.
    We offer trendy fashion, accessories and lifestyle products
    at affordable prices.</p>
</section>

<section id="contact">
    <h2>Contact Us</h2>
    <p>Email: shophub@gmail.com</p>
    <p>Phone: 9876543210</p>
</section>

<section id="account">
    <h2>My Account</h2>
    <p>Welcome to ShopHub! Happy Shopping.</p>
</section>

<section id="cart">
    <h2>🛒 My Shopping Cart</h2>
    <p>Total Products Added: <span id="cartItems">0</span></p>
</section>

<footer>
    <h2>ShopHub.</h2>
    <p>Follow Us: Instagram | Facebook | YouTube</p>
    <p>© 2026 ShopHub. All Rights Reserved.</p>
    <p>Designed with ❤️ for Shopping Lovers</p>
</footer>

<script>
    var total = 0;

    function addCart() {
        total++;

        document.getElementById("count").innerHTML = total;

        document.getElementById("cartItems").innerHTML = total;

        alert("Product added to your cart!");
    }
</script>

</body>
</html>

```
style.html
```

* {
    box-sizing: border-box;
}

body {
    margin: 0;
    font-family: Arial, sans-serif;
    background-color: #fff5f8;
}

header {
    background: linear-gradient(to right, #d63384, #8e44ad);
    color: white;
    text-align: center;
    padding: 20px;
}

header h1 {
    font-size: 40px;
    margin: 5px;
}

header p {
    font-size: 16px;
}

nav {
    background-color: #292338;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    padding: 15px;
}

nav a {
    color: white;
    text-decoration: none;
    margin: 10px 18px;
    font-weight: bold;
}

nav a:hover {
    color: #ff80ab;
}

.welcome {
    background: linear-gradient(to right, #ffe0eb, #ead7ff);
    text-align: center;
    padding: 60px 20px;
}

.welcome h2 {
    color: #9c2674;
    font-size: 35px;
}

.welcome h3 {
    color: #623477;
}

.welcome p {
    font-size: 18px;
}

.shop {
    display: inline-block;
    background-color: #d63384;
    color: white;
    text-decoration: none;
    padding: 12px 30px;
    border-radius: 25px;
    margin-top: 15px;
}

.shop:hover {
    background-color: #8e44ad;
}

#products {
    text-align: center;
    padding: 35px 20px;
}

#products h2 {
    color: #a52a75;
    font-size: 30px;
}

.container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 25px;
}

.product {
    background-color: white;
    width: 230px;
    padding: 15px;
    border-radius: 12px;
    box-shadow: 0 3px 10px #ddd;
    transition: 0.3s;
}

.product img {
    width: 100%;
    height: 180px;
    object-fit: cover;
    border-radius: 10px;
}

.product h3 {
    color: #333;
}

.product p {
    color: #d63384;
    font-size: 20px;
    font-weight: bold;
}

.product button {
    background-color: #d63384;
    color: white;
    border: none;
    padding: 10px 20px;
    border-radius: 20px;
    cursor: pointer;
}

.product button:hover {
    background-color: #8e44ad;
}

.product:hover {
    transform: translateY(-8px);
    box-shadow: 0 6px 15px #c9a2c9;
}

section:not(.welcome):not(#products) {
    background-color: white;
    margin: 20px;
    padding: 30px;
    text-align: center;
    border-radius: 10px;
}

section h2 {
    color: #a52a75;
}

footer {
    background-color: #292338;
    color: white;
    text-align: center;
    padding: 25px;
}

footer h2 {
    color: #ff80ab;
}



```

## OUTPUT

<img width="1917" height="1132" alt="Screenshot 2026-10-30 110648" src="https://github.com/user-attachments/assets/e7c1e79a-06ce-4bbb-8130-621622ca0a4a" />

<img width="1917" height="1148" alt="Screenshot 2026-10-30 110708" src="https://github.com/user-attachments/assets/02d4fc0b-d03b-434a-94d6-e7bb49ec818f" />

<img width="1917" height="1140" alt="Screenshot 2026-10-30 110736" src="https://github.com/user-attachments/assets/13db7352-d064-41a4-ac3d-f9326e262ab5" />

<img width="1917" height="1137" alt="Screenshot 2026-10-30 110749" src="https://github.com/user-attachments/assets/e0e5739d-f4c3-4af8-90d0-18bd325a02bb" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
