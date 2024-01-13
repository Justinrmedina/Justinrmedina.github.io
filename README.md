<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Medina, J.</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            margin: 0;
            padding: 0;
            position: relative;
            background-image: url('Programming image2 small.png');
            background-size: cover;
            background-position: top;
            width: 100%; /* Set width to cover the entire device width */
            height: 100vh;
        }

        body::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.6);
            z-index: 0;
        }

        header {
            color: white;
            padding: 5px;
            text-align: center;
            margin: 0;
            font-family: 'Arial', sans-serif;
            font-size: 0.9em;
            position: relative;
            z-index: 1;
        }

        nav {
            display: flex;
            justify-content: flex-end;
            align-items: center;
            z-index: 2;
        }

        nav ul {
            list-style: none;
            padding: 0;
            margin: 0;
        }

        nav li {
            display: inline;
            margin-right: 10px;
        }

        nav a {
            text-decoration: none;
            color: white;
        }

        #resume-link {
            color: cornflowerblue;
            padding: 2px 5px;
            border-radius: 50px;
            border: 2px solid cornflowerblue;
            text-decoration: none;
            margin-right: 10px;
        }

        main {
            color: white;
            position: relative;
            z-index: 2;
            margin: 0;
        }

        footer {
            position: absolute;
            bottom: 0;
            width: 100%;
            color: white;
            text-align: center;
            padding: 10px;
            z-index: 1;
        }

        /* Add skip to content link style */
        #skip-link {
            position: absolute;
            top: -40px;
            left: 0;
            background-color: cornflowerblue;
            color: white;
            padding: 5px;
            text-decoration: none;
            z-index: 3;
        }

        #skip-link:focus {
            top: 0;
        }
    </style>
</head>
<body>
    <!-- Skip to content link for accessibility -->
    <a href="#home" id="skip-link">Skip to Content</a>

    <header>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#sinyapps">ShinyApps</a></li>
                <li><a href="#contact">Contact</a></li>
                <li><a href="Medina_Justin_Resume.pdf" id="resume-link" target="_blank">Resume</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <article id="home">
            <h2>Home Section</h2>
            <!-- Content for the home section -->
        </article>

        <article id="about">
            <h2>About Section</h2>
            <!-- Content for the about section -->
        </article>

        <article id="contact">
            <h2>Contact Section</h2>
            <!-- Content for the contact section -->
        </article>
    </main>

    <footer>
        <p>&copy; 2024 J. Medina's Data Portfolio. All rights reserved.</p>
    </footer>
</body>
</html>













