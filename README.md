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
            position: absolute;
            background-image: url('Programming image2 small.png');
            background-repeat: no-repeat;
            background-attachment: fixed;
            background-size: cover;
            background-position: center center;
            width: 100%; /* Set width to cover the entire device width */
            height: 100vh;
        }

        body::before {
            content: "";
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            background-color: rgba(0, 0, 0, 0.6);
            z-index: 0;
        }

        header {
            color: white;
            padding: 5px;
            text-align: center;
            margin: 0;
            font-family: 'Arial', sans-serif;
            font-size: 1.2em;
            position: relative;
            z-index: 1;
        }

        nav {
            display: flex;
            justify-content: flex-end;
            align-items: center;
            z-index: 2;
            border-bottom: 2px solid white;
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
            margin-right: 10px;
            font-weight: bold;
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
                <li><a href="Medina_Justin_Resume.pdf" id="resume-link" target="_blank">Resume</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <article id="home">
    <div style="display: flex; justify-content: space-between; align-items: start;">
        <div style="flex: 1; text-align: right;">
            <!-- Text content on the left -->
            <h2>Justin R. Medina</h2>
            <p>Applied Biostatistics, Data Analytics, & statistical programming professional.</p>
            <p>"Turning data into insights is my passion."</p>
        </div>
        <div style="flex: 1; text-align: center; padding-top: 10px;">
            <div style="display: inline-block; 
            border: 5px solid white; 
            align-items: stretch;
            overflow: hidden;
            /*border-radius: 8px; */
            /*padding: 4px;*/
            ">
                <img src="Profile Pic small.jpg" alt="Profile Pic" style="width: 400px; 
                height: 450px; 
                margin-bottom: -8px;
                margin-left: -2px;
                margin-right: -2px;
                border-radius: 0px;">
            </div>
        </div>
    </div>
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
