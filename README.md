<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Liquid Layout Template</title>
    <link rel="stylesheet" href="style.css" />
<style>
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    background-image: url("tree.png");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    font-family: Arial, sans-serif;
    line-height: 1.6;
    background: #ffffff;
    color: #333;
}

header, nav, main, footer {
    padding: 1em;
}

header {
    background: #ffffff;
    background: linear-gradient(90deg,rgba(0, 119, 204, 1) 0%, rgba(0, 139, 204, 0.87) 38%, rgba(0, 180, 204, 1) 100%);
    color: white;
    padding: 1em;
}

.logo-container {
    display: flex;
    align-items: center;
    gap: 1em;
}

.logo {
    height: auto;
    width: 180px; /* Responsive size */
    max-width: 100%;
}

nav {
    background: #e0e0e0;
}

nav ul {
    list-style: none;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
}

nav a {
    text-decoration: none;
    color: #333;
    padding: 0.5em;
}

main {
    display: flex;
    flex-wrap: wrap;
    margin-top: 1em;
}

.content {
    flex: 3 1 60%;
    padding: 1em;
    background: #ffffff;
    margin-right: 1em;
}

.sidebar {
    flex: 1 1 30%;
    padding: 1em;
    background: #d9edf7;
}

footer {
    background: #333;
    color: white;
    text-align: center;
    padding: 1em;
    margin-top: 1em;
}
.listing-card {
    background: white;
    max-width: 800px;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s ease;
}

.listing-card:hover {
  transform: scale(1.01);
}

.image-gallery {
    width: 100%;
    height: 400px;
    overflow: hidden;
}

.image-gallery .main-image {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.details {
    padding: 1.5rem;
}

.details h2 {
    margin: 0;
    font-size: 2rem;
    color: #2c3e50;
}

.location {
    color: #888;
    font-size: 0.95rem;
    margin-bottom: 1rem;
}

.description {
    margin-bottom: 1.5rem;
    color: #333;
}

.features {
    list-style: none;
    padding: 0;
    margin: 0 0 1.5rem 0;
    display: flex;
    flex-wrap: wrap;
    gap: 1rem;
}

.features li {
    background: #eaf1f8;
    padding: 0.5rem 1rem;
    border-radius: 5px;
    font-size: 0.95rem;
}

.btn {
    display: inline-block;
    background: #3498db;
    color: white;
    padding: 0.75rem 1.5rem;
    border-radius: 5px;
    text-decoration: none;
    transition: background 0.3s;
}

.btn:hover {
    background: #2980b9;
}

</style>
</head>
<body>
<header>
    <div class="logo-container">
        <img src="emblem.png" alt="Company Logo" class="logo" />
        <h1>website v1</h1>
    </div>
</header>

    <nav>
        <ul>
            <li><a href="#">Home</a></li>
            <li><a href="#">About</a></li>
            <li><a href="#">Services</a></li>
            <li><a href="#">Contact</a></li>
        </ul>
    </nav>

    <main>
        <section class="content">
            <h2>About us</h2>
            <p>Thank you for visiting Insight services. We are a privately owned company that specializes
                in the purchasing and selling of properties. For the last 30 years, we have been serving the
                people of north east, fl. We are looking forward to helping you in your home buying journey.
            </p>
            <p>Text to be added here. This can go as far or even be modified. Placeholder.
            </p>
            <p>We are available 7 days a week.
            Please call or text us at 123-456-7890. Email us at Thisisatest@gmail.com
            </p>
        </section>
        <aside class="sidebar">
            <h3>sidebar</h3>
            <p>This is a sidebar with flexible width.</p>
        </aside>
    </main>

    <footer>
        <p>InSight Services inc</p>
    </footer>
</body>
</html>
