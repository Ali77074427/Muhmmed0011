<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Multipurpose Website with Products </title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
        }

        header {
            background-color: #3498db;
            color: white;
            text-align: center;
            padding: 30px 0;
        }

        header h1 {
            margin: 0;
        }

        nav {
            text-align: center;
            margin: 15px 0;
        }

        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: #3498db;
            font-size: 1.2em;
        }

        .section {
            padding: 50px 20px;
            text-align: center;
            background-color: #fff;
            margin-bottom: 20px;
        }

        .section h2 {
            font-size: 2em;
            color: #333;
        }

        .section p {
            font-size: 1.1em;
            color: #777;
            max-width: 700px;
            margin: 0 auto;
        }

        .products, .videos {
            display: flex;
            justify-content: space-around;
            flex-wrap: wrap;
            margin: 20px auto;
            width: 90%;
        }

        .product-item, .video-item {
            background-color: white;
            width: 30%;
            margin-bottom: 20px;
            box-shadow: 0px 4px 6px rgba(0,0,0,0.1);
            border-radius: 8px;
            text-align: center;
        }

        .product-item img, .video-item iframe {
            width: 100%;
            height: 200px;
            border-radius: 8px 8px 0 0;
        }

        .product-item h3, .video-item h3 {
            font-size: 1.5em;
            margin: 15px 0;
        }

        .testimonials {
            background-color: #f1f1f1;
            padding: 40px;
        }

        .testimonial-item {
            background-color: white;
            padding: 20px;
            margin: 10px;
            box-shadow: 0px 4px 6px rgba(0,0,0,0.1);
            border-radius: 8px;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 20px 0;
        }

        footer a {
            color: #3498db;
            text-decoration: none;
        }
        .payment-form {
            display: none;
            background-color: #eef;
            padding: 30px;
            text-align: center;
        } 

        .login-section, .signup-section {
            background-color: #eef;
            padding: 50px 20px;
            text-align: center;
        }

        .login-section input, .signup-section input {
            margin: 10px;
            padding: 10px;
            width: 250px;
        }

        .social-login {
            margin: 20px;
        }

        .social-login button {
            background-color: #3498db;
            color: white;
            border: none;
            padding: 10px 20px;
            margin: 10px;
            cursor: pointer;
        }
    </style>
</head>
<body>

<!-- Header and Navigation -->
<header>
  <!-- Menu Icon (Left) -->
  <div class="menu-icon" onclick="toggleMenu()">☰</div>

  <!-- Search Bar (Center) -->
  <div class="search-bar">
    <input type="text" placeholder="Search..." />
    <button type="submit">Search</button>
  </div>

  <!-- Start Button (Right) -->
  <div class="start-button">
    <button onclick="startAction()">Start</button>
  </div>

  <!-- Dropdown Menu (Left) -->
  <div id="dropdown-menu" class="dropdown-menu">
    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#about">About Us</a></i></a></li>
      <li><a href="#products">Products</a></a></li>
      <li><a href="#">Login</a></li>
      <li><a href="#videos">Videos</a></a></li>
    </ul>
  </div>
</header>

<script>
  function toggleMenu() {
    var menu = document.getElementById("dropdown-menu");
    menu.style.display = menu.style.display === "block" ? "none" : "block";
  }

  function startAction() {
    alert("Start button clicked!");
  }
</script>

<style>
  /* General Header Styles */
  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: relative;
    height: 60px;
    background-color: #f1f1f1;
    padding: 0 20px;
  }

  /* Menu Icon (Left) */
  .menu-icon {
    font-size: 30px;
    cursor: pointer;
    position: absolute;
    left: 20px;
  }

  /* Search Bar (Center) */
  .search-bar {
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
  }

  .search-bar input {
    padding: 5px;
  }

  /* Start Button (Right) */
  .start-button {
    position: absolute;
    right: 20px;
  }

  .start-button button {
    padding: 10px 15px;
    cursor: pointer;
  }

  /* Dropdown Menu (Left) */
  .dropdown-menu {
    display: none;
    position: absolute;
    left: 20px;
    top: 60px;
    background-color: #f9f9f9;
    box-shadow: 0px 8px 16px rgba(0, 0, 0, 0.2);
  }

  .dropdown-menu ul {
    list-style-type: none;
    padding: 0;
    margin: 0;
  }

  .dropdown-menu ul li a {
    padding: 12px 16px;
    display: block;
    text-decoration: none;
    color: black;
  }

  .dropdown-menu ul li a:hover {
    background-color: #ddd;
  }
</style>

 
    
  </div>
</header>

<script>
  function toggleMenu() {
    var menu = document.getElementById("dropdown-menu");
    menu.style.display = menu.style.display === "block" ? "none" : "block";
  }
</script>


<nav>

</nav>

<!-- About Section -->
<section id="about" class="section">
    <h2>About Our Work</h2>
    <p>We are dedicated to delivering 
    the best projects to our clients.
    Our work spans various industries 
    and includes innovative solutions to everyday challenges.</p>
</section>

<!-- Products Section -->
<section id="products" class="section">
    <h2>Our Products</h2>
    <div class="products">
        <!-- Product 1: Women's Watch -->
        <div class="product-item">
            <img src="https://images.pexels.com/photos/4111503/pexels-photo-4111503.jpeg" alt="Women's Watch">
            <h3>Women's Watch</h3>
            <p>Elegant women's watch with a stainless steel bracelet and classic design.</p>
            <button class="order-button" onclick="showPaymentForm()">Order No
        </div>
       <!-- Product 2: Women's Watch -->
        <div class="product-item">
            <img src="https://images.pexels.com/photos/1538853/pexels-photo-1538853.jpeg" alt="Women's Watch">
            <h3>Women's Watch</h3>
            <p>Elegant women's watch with a stainless steel bracelet and classic design.</p>
            <button class="order-button" onclick="showPaymentForm()">Order Now
        </div>
        <!-- Product 3: Men's Jacket -->
        <div class="product-item">
            <img src="https://images.unsplash.com/photo-1506031549314-bf8a6f69d8c3?crop=entropy&cs=tinysrgb&fit=max&ixid=MnwzNjUyOXwwfDF8c2VhcmNofDJ8fG1lbnxlbnwwfHx8fDE2NTY1NzY2&ixlib=rb-1.2.1&q=80&w=400" alt="Men's Jacket">
            <h3>Men's Jacket</h3>
            <p>Comfortable and stylish men's jacket, ideal for casual and outdoor wear.</p>
            <button class="order-button" onclick="showPaymentForm()">Order Now
        </div>
        <!-- Product 4: Women's Dress -->
        <div class="product-item">
            <img src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e?crop=entropy&cs=tinysrgb&fit=max&ixid=MnwzNjUyOXwwfDF8c2VhcmNofDJ8fG1lbmJvfGVufDB8fHx8MTY1NzEwNzY1&ixlib=rb-1.2.1&q=80&w=400" alt="Women's Dress">
            <h3>Women's Dress</h3>
            <p>Chic and elegant women's dress, perfect for formal events or special occasions.</p>
            <button class="order-button" onclick="showPaymentForm()">Order Now
        </div>
               <!-- Product 5: Men's Shoes -->
        <div class="product-item">
            <img src="https://images.pexels.com/photos/414779/pexels-photo-414779.jpeg" alt="Men's Shoes">
            <h3>Men's Shoes</h3>
            <p>High-quality men's shoes with a sleek design and durable material. Suitable for everyday wear.</p>
              <button class="order-button" onclick="showPaymentForm()">Order Now</button>
              <!-- Payment Form -->
<div id="payment-form" class="payment-form">
    <h2>Payment Information</h2>
    <form>
        <input type="text" placeholder="Card Number" required><br>
        <input type="text" placeholder="Expiration Date" required><br>
        <input type="text" placeholder="CVV" required><br>
        <button type="submit">Pay Now</button>
    </form>
</div>
        </div>
        <script>
    function showPaymentForm() {
        document.getElementById("payment-form").style.display = "block";
    }
</script>
    </div>
</section>

<!-- Videos Section -->
<section id="videos" class="section">
    <h2>Our Video Projects</h2>
    <div class="videos">
        <!-- Video 1 -->
        <div class="video-item">
            <iframe src="https://www.youtube.com/embed/Gq6uKjPWDcY?si=PIxwomFoHa1snT2V" title="PUBG Montage" allowfullscreen></iframe>
            <h3></h3>
            <p>ابرهيم الملصي  و عزالدين الداوي - وين ساير - ( حصري ) | 2024</p>
        </div>
        <!-- Video 2 -->
        <div class="video-item">
            <iframe src="https://www.youtube.com/embed/1mgGHlzNFDA?si=SOc3z8z_bKwcXOQn" title="Video 2" allowfullscreen></iframe>
            <h3></h3>
            <p>ابراهيم الملصي ل بعد الجدل 2024 ابراهيم الملسي</p>
        </div>
        <!-- Video 3 -->
        <div class="video-item">
            <iframe src="https://WWW.youtube.com/embed/rvgymuyADv4?si=6sTSOhChtDdAcF1z" title="Video 3" allowfullscreen></iframe>
            <h3></h3>
            <p></p>
        </div>
    </div>
</section>

<!-- Testimonials Section -->
<section id="clients" class="testimonials">
    <h2>Our Clients Love Us</h2>
    <div class="testimonial-item">
        <p>"Fantastic service and amazing projects! Highly recommend."</p>
        <p>- Client 1</p>
    </div>
    <div class="testimonial-item">
        <p>"Truly innovative solutions that helped us scale our business."</p>
        <p>- Client 2</p>
    </div>
    <div class="testimonial-item">
        <p>"Professional and dedicated team with great attention to detail."</p>
        <p>- Client 3</p>
    </div>
</section>
<!-- Footer Section with Login, Signup, and Contact -->
<footer>
    <div style="text-align: center;">
        <!-- Login / Signup Section #black-->
<section id="login-signup" class="login-signup-form" style="text-align: center; background-color:mintcream; padding: 20px;">
    <h2>Login / Signup</h2>
    <form action="/login" method="post">
        <input type="email" placeholder="Email" required><br>
        <input type="password" placeholder="Password" required><br>
        <button type="submit">Login</button>
        <p>or</p>
        <button>Sign in with Facebook</button>
        <button>Sign in with Google</button>
    </form>
</section>

<!-- Contact Information Section -->
<section id="contact" style="background-color:black; padding: 20px; text-align: left; position: relative;">
    <h2>Contact Us</h2>
    <p>Name: Αℓi мσнαєɒ  Αℓ _ Ɒαiℓαмi </p>
    <p>Phone: +967 770 744 273</p>
    <p>Email: ‏bxvxksbwidvdid@gmail.com‏</p>
</section>

     




    </ul>
    
  </div>
  <div class="footer-bottom">
  </div>
</footer>
     <p style="text-align: center;">&copy; 2024 Top Corner Store. All rights reserved.</p>
</footer>
</nav>
<!-- /Footer Section -->
