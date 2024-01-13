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
            /*min-height: 100vh;*/
            background-image: url('Programming image2 small.png');
            background-size: cover;
            background-position: top;
        }

        body::before {
            content: "";
            position: absolute;
            top: -10%;
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

        section {
            color: white;
            position: relative;
            z-index: 2;
            margin: 0; /* Add this to remove margin */
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
    </style>
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#sinyapps">ShinyApps</a></li>
                <li><a href="#contact">Contact</a></li>
                <a href="Medina_Justin_Resume.pdf" id="resume-link" target="_blank">Resume</a>
            </ul>
        </nav>
    </header>
    <section id="home">
        <h2>Home Section</h2>
        <!-- Content for the home section -->
    </section>
    <section id="about">
        <h2>About Section</h2>
        <!-- Content for the about section -->
    </section>
    <section id="contact">
        <h2>Contact Section</h2>
        <!-- Content for the contact section -->
    </section>
    <footer>
        <p>&copy; 2024 J. Medina's Data Portfolio. All rights reserved.</p>
    </footer>
</body>
</html>












