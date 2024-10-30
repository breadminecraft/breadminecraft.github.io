<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lift Man Service</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <h1>Welcome to Lift Man Service</h1>
        <nav>
            <ul>
                <li><a href="#about">About Us</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <section id="about">
        <h2>About Us</h2>
        <p>We provide reliable lift services with various facilities to make your journey comfortable.</p>
    </section>

    <section id="services">
        <h2>Our Services</h2>
        <ul>
            <li>Pickup and Drop Location Services</li>
            <li>24/7 Availability</li>
            <li>Comfortable Vehicles</li>
            <li>Professional Drivers</li>
        </ul>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <form id="contactForm">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            
            <label for="pickup">Pickup Location:</label>
            <input type="text" id="pickup" name="pickup" required>

            <label for="drop">Drop Location:</label>
            <input type="text" id="drop" name="drop" required>
            
            <button type="submit">Submit</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2024 Lift Man Service. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background-color: #007BFF;
    color: white;
    padding: 1rem;
    text-align: center;
}

nav ul {
    list-style-type: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

section {
    padding: 2rem;
    margin: 1rem;
}

form {
    display: flex;
    flex-direction: column;
}

label {
    margin-top: 10px;
}

input {
    padding: 8px;
    margin-top: 5px;
    border: 1px solid #ccc;
    border-radius: 4px;
}

button {
    margin-top: 10px;
    padding: 10px;
    background-color: #28A745;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}

button:hover {
    background-color: #218838;
}

footer {
    text-align: center;
    padding: 1rem;
    background-color: #f8f9fa;
}
3. JavaScript (script.js)
javascript
Copy code
document.getElementById('contactForm').addEventListener('submit', function(event) {
    event.preventDefault();
    
    const name = document.getElementById('name').value;
    const email = document.getElementById('email').value;
    const pickup = document.getElementById('pickup').value;
    const drop = document.getElementById('drop').value;

    alert(Thank you ${name}! We will pick you up from ${pickup} and drop you off at ${drop}.);
    
    // Here you can add code to send the data to your server or database
});
</body>
</html>
