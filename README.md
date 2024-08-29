<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Big Orange Carpet Cleaners</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f7f7f7;
        }
        header {
            background-color: #ff6600;
            color: white;
            padding: 20px;
            text-align: center;
        }
        nav {
            display: flex;
            justify-content: center;
            background-color: #333;
        }
        nav a {
            color: white;
            padding: 14px 20px;
            text-decoration: none;
            text-align: center;
        }
        nav a:hover {
            background-color: #ff6600;
        }
        .hero {
            background-image: url('carpet-cleaning.jpg');
            height: 300px;
            background-size: cover;
            background-position: center;
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 2rem;
            text-shadow: 2px 2px 8px rgba(0,0,0,0.8);
        }
        .content {
            padding: 20px;
        }
        .services, .about, .contact, .book {
            margin-bottom: 40px;
        }
        form {
            display: flex;
            flex-direction: column;
            max-width: 400px;
            margin: auto;
        }
        form label {
            margin-top: 10px;
        }
        form input, form select, form textarea {
            padding: 10px;
            margin-top: 5px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        form button {
            background-color: #ff6600;
            color: white;
            border: none;
            padding: 10px;
            margin-top: 20px;
            cursor: pointer;
        }
        form button:hover {
            background-color: #333;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
        }
    </style>
</head>
<body>

    <header>
        <h1>Big Orange Carpet Cleaners</h1>
        <p>Your trusted partner for spotless carpets</p>
    </header>

    <nav>
        <a href="#home">Home</a>
        <a href="#services">Services</a>
        <a href="#about">About Us</a>
        <a href="#contact">Contact</a>
        <a href="#book">Book Appointment</a>
    </nav>

    <div class="hero" id="home">
        <h2>We Make Your Carpets Look Brand New!</h2>
    </div>

    <div class="content">
        <section class="services" id="services">
            <h2>Our Services</h2>
            <ul>
                <li>Residential Carpet Cleaning</li>
                <li>Commercial Carpet Cleaning</li>
                <li>Stain Removal</li>
                <li>Upholstery Cleaning</li>
                <li>Pet Odor Removal</li>
            </ul>
        </section>

        <section class="about" id="about">
            <h2>About Us</h2>
            <p>Big Orange Carpet Cleaners has been serving the community for over 15 years. Our expert team uses eco-friendly products to ensure your home is safe for your family and pets, while also making your carpets look brand new.</p>
        </section>

        <section class="contact" id="contact">
            <h2>Contact Us</h2>
            <p>Email: info@bigorangecarpetcleaners.com</p>
            <p>Phone: (555) 123-4567</p>
            <p>Location: 123 Main Street, Orange City, FL</p>
        </section>

        <section class="book" id="book">
            <h2>Book an Appointment</h2>
            <form action="/submit-appointment" method="POST">
                <label for="name">Full Name:</label>
                <input type="text" id="name" name="name" required>

                <label for="email">Email Address:</label>
                <input type="email" id="email" name="email" required>

                <label for="phone">Phone Number:</label>
                <input type="tel" id="phone" name="phone" required>

                <label for="service">Select Service:</label>
                <select id="service" name="service" required>
                    <option value="residential">Residential Carpet Cleaning</option>
                    <option value="commercial">Commercial Carpet Cleaning</option>
                    <option value="stain_removal">Stain Removal</option>
                    <option value="upholstery">Upholstery Cleaning</option>
                    <option value="pet_odor">Pet Odor Removal</option>
                </select>

                <label for="date">Preferred Appointment Date:</label>
                <input type="date" id="date" name="date" required>

                <label for="message">Additional Comments:</label>
                <textarea id="message" name="message" rows="4"></textarea>

                <button type="submit">Submit</button>
            </form>
        </section>
    </div>

    <footer>
        <p>&copy; 2024 Big Orange Carpet Cleaners. All Rights Reserved.</p>
    </footer>

</body>
</html>
