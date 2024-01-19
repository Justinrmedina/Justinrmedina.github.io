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
            width: 100%;
            height: 100%;
            overflow: hidden;
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

        #home {
            overflow: hidden; /* Hide overflow for the Home section */
        }

        .falling-shapes-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            overflow: hidden;
            z-index: 1;
            pointer-events: none; /* Make falling shapes not interactable */
        }

        .falling-shapes {
            position: absolute;
            width: 20px;
            height: 20px;
            background-color: white;
            border: 1px solid black; /* Black outline */
            animation: fall 2s linear infinite;
        }

        @keyframes fall {
            to {
                transform: translateY(100vh);
            }
        }

        main {
            overflow-y: auto;
            position: relative;
            z-index: 2;
        }

        header {
            color: white;
            padding: 1px;
            text-align: center;
            margin: 0;
            font-family: 'Arial', sans-serif;
            font-size: 1em;
            position: sticky;
            top: 0;
            z-index: 3;
        }

        nav {
            display: flex;
            justify-content: flex-end;
            align-items: center;
            z-index: 2;
            border-bottom: 1px solid white;
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
            margin: 20px 0px;
            padding-bottom: 40px;
        }

        #home {
            background-color: rgba(0, 0, 0, 0.6); /* Transparent black background */
            border-radius: 10px; /* Round edges */
            padding: 20px; /* Add padding for better visibility */
        }

        #home .quote-text {
            text-align: center;
            font-size: 1.7em; /* Adjust the font size as needed */
            font-style: italic; /* Italicize the text */
            margin-top: 60px;
        }

        .projects-button {
            display: block;
            margin: 20px auto 0px auto;
            background-color: cornflowerblue;
            color: white;
            padding: 5px 8px;
            border: none;
            border-radius: 10px;
            font-size: 1.2em;
            cursor: pointer;
        }

        .projects-button a {
            text-decoration: none;
            color: white;
        }

        footer {
            position: fixed;
            bottom: 0;
            width: 100%;
            color: white;
            text-align: center;
            padding: 10px;
            z-index: 3;
        }

        /* Rest of your existing styles remain unchanged */

    </style>
</head>
<body>
    
    <header>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#my-projects">My Projects</a></li>
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
                    <h1>Justin R. Medina</h1>
                    <p>Applied Biostatistics, Data Analytics, & Statistical Programming Professional.</p>
                    <p class="quote-text">"Turning data into insights is my passion."</p>
                    <button class="projects-button"><a href="#my-projects">My Projects</a></button>
                </div>
                <div style="flex: 1; text-align: center; padding-top: 10px;">
                    <div style="display: inline-block; 
                    border: 5px solid white; 
                    align-items: stretch;
                    overflow: hidden;
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
            <!-- Falling shapes container -->
            <div class="falling-shapes-container">
                <!-- Falling shapes elements -->
                <div class="falling-shapes"></div>
                <div class="falling-shapes"></div>
                <div class="falling-shapes"></div>
                <div class="falling-shapes"></div>
                <!-- You can add more falling shapes as needed -->
            </div>
        </article>

        <article id="about">
            <h2>About Section</h2>
            <!-- Content for the about section -->
        </article>

        <article id="my-projects">
            <h2>My Projects</h2>
            <!-- Content for the projects section -->
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




