# Week-8-final-project
index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Home - Faheem7</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <header>
        <h1>Welcome to My Website</h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section>
        <h2>Introduction</h2>
        <p>This is a responsive, interactive website built with HTML, CSS, and JavaScript.</p>
        <button onclick="showMessage()">Click Me</button>
    </section>

    <script src="js/script.js"></script>
</body>
</html>
about.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About - My Website</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <header>
        <h1>About Us</h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section>
        <h2>Who We Are</h2>
        <p>We build awesome websites using the latest technologies.</p>
    </section>
</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact - My Website</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <header>
        <h1>Contact Us</h1>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="about.html">About</a></li>
                <li><a href="contact.html">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section>
        <h2>Get in Touch</h2>
        <form id="contactForm">
            <label for="name">Name:</label>
            <input type="text" id="name" required>
            
            <label for="email">Email:</label>
            <input type="email" id="email" required>

            <button type="submit">Submit</button>
        </form>
    </section>

    <script src="js/script.js"></script>
</body>
</html>
styles.css
body {
    font-family: Arial, sans-serif;
    text-align: center;
    background-color: #f4f4f4;
    margin: 0;
}

header {
    background-color: #333;
    color: white;
    padding: 15px;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav a {
    text-decoration: none;
    color: white;
}

section {
    padding: 20px;
}

button {
    padding: 10px 15px;
    background-color: #007bff;
    color: white;
    border: none;
    cursor: pointer;
    transition: transform 0.3s;
}

button:hover {
    transform: scale(1.1);
    background-color: #0056b3;
}
script.js
function showMessage() {
    alert("Welcome to my interactive website!");
}

// Form validation
document.getElementById("contactForm").addEventListener("submit", function(event) {
    event.preventDefault(); // Prevent form from submitting

    let name = document.getElementById("name").value;
    let email = document.getElementById("email").value;

    if (name === "" || email === "") {
        alert("Please fill in all fields!");
    } else {
        alert("Thank you, " + name + "! Your message has been received.");
    }
});




