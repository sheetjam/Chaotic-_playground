<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>InSight Services</title>
  <link rel="stylesheet" href="style.css" />
  <style>
    /* ========= Base Styles ========= */

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      background: url("tree.png") center/cover no-repeat;
      font-family: Arial, sans-serif;
      color: #333;
      line-height: 1.6;
    }

    header {
      background: linear-gradient(
        90deg,
        rgba(0, 119, 204, 1) 0%,
        rgba(0, 139, 204, 0.87) 38%,
        rgba(0, 180, 204, 1) 100%
      );
      color: #fff;
      padding: .5em;
    }

    .header-top {
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-wrap: wrap;
    }

    .logo-container {
      display: flex;
      align-items: center;
      gap: 1em;
    }

    .logo {
      width: 70px;
      height: auto;
      max-width: 100%;
    }

    /* ========= Navigation ========= */

    .hamburger {
      display: none;
      font-size: 2rem;
      cursor: pointer;
    }

    nav {
      background: #0077cc;
    }

    nav ul {
      display: flex;
      list-style: none;
      justify-content: center;
      gap: 2rem;
      padding: 1em;
    }

    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: bold;
      padding: 0.5em;
      transition: background 0.3s;
    }

    nav a:hover {
      background: rgba(255, 255, 255, 0.2);
      border-radius: 5px;
    }

    /* ========= Main Layout ========= */

    main {
      display: flex;
      flex-wrap: wrap;
      gap: 1em;
      padding: 1em;
    }

    .content {
      flex: 3 1 60%;
      background: #fff;
      padding: 1em;
      border-radius: 5px;
    }

    .sidebar {
      flex: 1 1 30%;
      background: #d9edf7;
      padding: 1em;
      border-radius: 5px;
    }

    footer {
      background: #333;
      color: #fff;
      text-align: center;
      padding: 1em;
      margin-top: 1em;
    }

    /* ========= Responsive ========= */

    @media (max-width: 768px) {
      .hamburger {
        display: block;
        color: #fff;
      }

      nav {
        display: none;
      }

      nav.show {
        display: block;
      }

      nav ul {
        flex-direction: column;
        align-items: flex-start;
        gap: 0;
        padding: 0;
      }

      nav li {
        width: 100%;
      }

      nav a {
        display: block;
        width: 100%;
        padding: 1em;
        border-bottom: 1px solid rgba(255, 255, 255, 0.2);
      }

      .logo-container {
        flex: 1;
      }
    }
  </style>
</head>
<body>
  <header>
    <div class="header-top">
      <div class="hamburger" onclick="toggleNav()">
        &#9776;
      </div>
      <div class="logo-container">
        <img src="emblem.png" alt="InSight Services Logo" class="logo" />
        <h4>Where dream homes become reality</h4>
      </div>
    </div>
    <nav id="myLinks">
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Placeholder</a></li>
        <li><a href="#">Locations</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <section class="content">
      <h2>About Us</h2>
      <p>
        Thank you for visiting InSight Services. We are a privately owned company
        specializing in the purchasing and selling of properties. For the last
        30 years, we have been serving the people of Northeast Florida. We look
        forward to helping you in your home-buying journey.
      </p>
      <p>
        Additional text can be added here as needed. This is placeholder
        content.
      </p>
      <p>
        We are available 7 days a week. Please call or text us at
        <a href="tel:1234567890">123-456-7890</a> or email us at
        <a href="mailto:thisisatest@gmail.com">thisisatest@gmail.com</a>.
      </p>
    </section>

    <aside class="sidebar">
      <h3>Sidebar</h3>
      <p>This is a sidebar with flexible width.</p>
    </aside>
  </main>

  <footer>
    <p>&copy; InSight Services Inc.</p>
  </footer>

  <script>
    function toggleNav() {
      var nav = document.getElementById("myLinks");
      nav.classList.toggle("show");
    }
  </script>
</body>
</html>
