# Veerpal-500224580-Week1Assignment_emerging_dev_technologies
# Part 1:
# HTML:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Flex and Grid Layout</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <!-- Flex Section -->
        <section class="flex-section">
            <h1>Flex Layout</h1>
            <h2>Evenly Spaced Items</h2>
            <div class="flex-container">
                <div class="flex-item">Profile</div>
                <div class="flex-item">Settings</div>
                <div class="flex-item">Messages</div>
                <div class="flex-item">Notifications</div>
            </div>
        </section>

        <!-- Grid Section -->
        <section class="grid-section">
            <h1>Grid Layout</h1>
            <h2>Grid with Four Columns</h2>
            <div class="grid-container">
                <div class="grid-item">Dashboard</div>
                <div class="grid-item">Reports</div>
                <div class="grid-item">Analytics</div>
                <div class="grid-item">Support</div>
            </div>
        </section>
    </div>
</body>
</html>

# css code:
/* General Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f9f9f9;
    color: #333;
}

h1, h2 {
    text-align: center;
    margin-bottom: 10px;
}

.container {
    padding: 20px;
}

/* Flex Section Styles */
.flex-section {
    background-color: #f0f4ff;
    margin-bottom: 20px;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.flex-container {
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    padding: 10px;
}

.flex-item {
    background-color: #4caf50;
    color: #fff;
    padding: 15px 20px;
    margin: 5px;
    border-radius: 4px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    text-align: center;
    flex-grow: 1;
    max-width: 150px;
}

/* Grid Section Styles */
.grid-section {
    background-color: #fff3cd;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.grid-container {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
}

.grid-item {
    background-color: #ff5722;
    color: #fff;
    padding: 15px;
    border-radius: 4px;
    text-align: center;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

/* Responsive Design */
@media (max-width: 768px) {
    .flex-container {
        flex-direction: column;
    }

    .grid-container {
        grid-template-columns: repeat(2, 1fr);
    }
}

@media (max-width: 480px) {
    .grid-container {
        grid-template-columns: 1fr;
    }
}

# Part 2:
# HTML code:
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Personal Portfolio</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header class="flex-section">
        <nav class="flex-container">
            <a href="#about" class="flex-item">About Me</a>
            <a href="#projects" class="flex-item">Projects</a>
            <a href="#contact" class="flex-item">Contact</a>
        </nav>
    </header>

    <section id="about" class="about-section">
        <h1>About Me</h1>
        <p>Hello! As a creative developer, I specialize in crafting engaging, user-friendly websites using HTML, CSS, and JavaScript. I have a passion for designing responsive and aesthetically pleasing web experiences.</p>
    </section>

    <section id="projects" class="grid-section">
        <h1>Projects</h1>
        <h2>Some of My Work</h2>
        <div class="grid-container">
            <div class="grid-item">CodeCrafters</div>
            <div class="grid-item">TaskTrack Pro</div>
            <div class="grid-item">EduLearn</div>
            <div class="grid-item">ShopEase</div>
        </div>
    </section>

    <section id="contact" class="flex-section">
        <h1>Contact</h1>
        <div class="flex-container">
            <div class="flex-item">veerpal242000@gmail.com</div>
            <div class="flex-item">+1 (647) 614-4641</div>
            <div class="flex-item">https://www.linkedin.com/in/veerpal</div>
        </div>
    </section>

    <footer class="flex-section">
        <p>&copy; 2025 My Portfolio. All rights reserved.</p>
    </footer>
</body>
</html>
# styles css code :

/* General Styling */
body {
    font-family: 'Arial', sans-serif;
    margin: 0;
    padding: 0;
    background: #eae7dc;
    color: #444;
    line-height: 1.6;
}

h1, h2 {
    font-family: 'Poppins', sans-serif;
    text-align: center;
    margin: 10px 0;
}

a {
    text-decoration: none;
    color: white;
}

p {
    text-align: center;
    max-width: 800px;
    margin: 0 auto 20px;
    font-size: 1.2em;
}

/* Header Styling */
header {
    background-color: #2a363b;
    padding: 15px 0;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

.flex-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 20px;
}

.flex-item {
    padding: 12px 25px;
    background-color: #e84a5f;
    border-radius: 10px;
    font-weight: bold;
    transition: background-color 0.3s ease, transform 0.3s ease;
}

.flex-item:hover {
    background-color: #ff847c;
    transform: scale(1.1);
}

/* About Section */
.about-section {
    background-color: #99b898;
    color: white;
    padding: 50px 20px;
    text-align: center;
}

/* Projects Section */
.grid-section {
    background-color: #feceab;
    padding: 50px 20px;
}

.grid-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
    gap: 25px;
    padding: 25px;
}

.grid-item {
    background-color: #ff6f69;
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 160px;
    border-radius: 12px;
    font-weight: bold;
    font-size: 1.3em;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.grid-item:hover {
    transform: scale(1.1);
    box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2);
}

/* Contact Section */
#contact {
    background-color: #355c7d;
    color: white;
    padding: 50px 20px;
}

.flex-section .flex-container .flex-item {
    background-color: #f67280;
    color: #fff;
    font-size: 1.2em;
}

.flex-section .flex-container .flex-item:hover {
    background-color: #c06c84;
    color: white;
}

/* Footer Styling */
footer {
    background-color: #6c5b7b;
    color: white;
    text-align: center;
    padding: 15px 0;
    font-size: 0.9em;
}
