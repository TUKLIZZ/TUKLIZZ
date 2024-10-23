<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="../css/comerce.css">
    <title>Buytopia - Your Online Gadget Shop</title>
</head>
<body>
    <header>
        <div class="header-container">
          
        <h1>Welcome to Buytopia</h1>
        <nav>
            <ul>
                <button><li><a href="#" onclick="showSection('home')">Home</a></li></button>
                <button> <li><a href="#" onclick="showSection('products')">Products</a></li></button>
                    <button> <li><a href="#" onclick="showSection('about')">About Us</a></li></button>
                        <button><li><a href="#" onclick="showSection('contact')">Contact</a></li></button>
            </ul>
        </nav>
    </header>

    <main>
        <section id="home" class="active">
            <h2>Welcome to Buytopia!</h2>
            <p>Your one-stop shop for the latest gadgets. Explore our products and find the best deals.</p>
        </section>

        <section id="products" style="display: none;">
            <h2>Featured Gadgets</h2>
            <div>
            
            <div>
                <div class="product">
                    <img src="../HTML/phone.jpg" width="150px" height="150px" alt="Smartphone">
                    <h3>Phone</h3>
                    <a href="../HTML/smartphone.html">Click more details</a>
                    <p>Price: $199.99</p>
                    
                </div>
            
                <div class="product">
                    <img src="../HTML/watch.jpg" width="150px" height="150px" alt="Smartwatch">
                    <h3>Watch Y</h3>
                    <a href="../HTML/watch.html">Click more details</a>
                    <p>Price: $149.99</p>
                
                </div>
            
                <div class="product">
                    <img src="../HTML/headphone.jpg" width="150px" height="150px" alt="Headphone">
                    <h3>Headphone Z</h3>
                    <a href="../HTML/Heaphone.html">Click more details</a>
                    <p>Price: $149.99</p>
                    
                </div>
            
             
         
           </div>
        </section>

        <section id="about" style="display: none;">
            <h2>About Us</h2>
            <p>Buytopia is dedicated to bringing you the latest and greatest in gadget technology.</p>
        </section>

        <section id="contact" style="display: none;">
            <h2>Contact Us</h2>
            <p>If you have any questions, feel free to reach out to us at support@buytopia.com.</p>
        </section>
    
    </main>

    <footer>
        <p>&copy; 2024 Buytopia. All rights reserved.</p>
    </footer>

    <script>
        function showSection(sectionId) {
            // Hide all sections
            const sections = document.querySelectorAll('main > section');
            sections.forEach(section => {
                section.style.display = 'none';
            });
            // Show the selected section
            const activeSection = document.getElementById(sectionId);
            activeSection.style.display = 'block';
            
        }
    </script>
</body>
</html>
