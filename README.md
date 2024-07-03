<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SipSmart Water Bottle</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>SipSmart Water Bottle</h1>
        <p class="slogan">Hydrate Smarter, Live Better</p>
    </header>
    
    <section class="product-info">
        <h2>About SipSmart Water Bottle</h2>
        <img src="sipsmart-bottle.jpg" alt="SipSmart Water Bottle" class="product-image">
        <p>The SipSmart Water Bottle is designed to help you stay hydrated effortlessly with smart tracking and stylish design.</p>
        <p class="price">Price: 450 RM</p>
        <a href="#order-form" class="order-button">Order Now</a>
    </section>

    <section id="order-form" class="order-form">
        <h2>Order Your SipSmart Water Bottle</h2>
        <form id="orderForm">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>

            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>

            <label for="address">Shipping Address:</label>
            <textarea id="address" name="address" required></textarea>

            <label for="quantity">Quantity:</label>
            <input type="number" id="quantity" name="quantity" min="1" value="1" required>

            <button type="submit">Submit Order</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2024 SipSmart. All Rights Reserved.</p>
    </footer>

    <script>
        document.getElementById('orderForm').addEventListener('submit', function(event) {
            event.preventDefault();
            alert('Thank you for your order! We will contact you soon.');
            document.getElementById('orderForm').reset();
        });
    </script>
</body>
</html>
