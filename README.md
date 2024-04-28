
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio</title>
    <link rel="stylesheet" href="styles.css">
</head>

<body>
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#interests">Areas of Interest</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
    <header id="home">
        <h1>Your Name</h1>
        <p>Web Developer | Data Analyst | AI Enthusiast</p>
    </header>
    <section id="about">
        <h2>About Me</h2>
        <p>Add your about me content here</p>
    </section>
    <section id="interests">
        <h2>Areas of Interest</h2>
        <p>Add your areas of interest content here</p>
    </section>
    <section id="skills">
        <h2>Skills</h2>
        <p>Add your skills content here</p>
    </section>
    <section id="projects">
        <h2>Projects</h2>
        <p>Add your projects content here</p>
    </section>
    <section id="contact">
        <h2>Contact Me</h2>
        <p>Add your contact me content here</p>
    </section>
    <script src="script.js"></script>
</body>

</html>

/* styles.css */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    scroll-behavior: smooth;
}

nav {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background-color: #333;
}

nav ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
}

nav ul li {
    float: left;
}

nav ul li a {
    display: block;
    color: white;
    text-align: center;
    padding: 14px 20px;
    text-decoration: none;
}

nav ul li a:hover {
    background-color: #ddd;
    color: black;
}

header {
    background-color: #111;
    color: white;
    text-align: center;
    padding: 100px 0;
}

section {
    background-color: #f4f4f4;
    padding: 50px 0;
    text-align: center;
}

h1, h2 {
    margin-bottom: 20px;
}

p {
    font-size: 1.2em;
}

/* Add more styling as needed */

// script.js
window.addEventListener('DOMContentLoaded', (event) => {
    const navLinks = document.querySelectorAll('nav a');

    navLinks.forEach(link => {
        link.addEventListener('click', function(e) {
            e.preventDefault();
            const targetId = this.getAttribute('href').substring(1);
            const targetSection = document.getElementById(targetId);
            targetSection.scrollIntoView({ behavior: 'smooth' });
        });
    });
});

