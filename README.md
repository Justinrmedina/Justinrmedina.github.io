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
            background-image: url('Programming Image small.jpg');
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
            background-color: rgba(0, 0, 0, 0.5);
            z-index: 0;
        }

        header {
            color: white;
            font-family: 'Arial', sans-serif;
            font-size: 1.2em;
            position: sticky;
            z-index: 3;
            margin-top: 0px;
      
        }

        nav {
            display: flex;
            padding-top: 20px;
            justify-content: flex-end;
            align-items: center;
            z-index: 2;
            background-color: rgba(0, 0, 0, 0.6);
      		height: 60px;
        }

        nav ul {
            list-style: none;
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
            font-family: 'Arial', sans-serif;
            font-weight: bold;
        }

        main {
            color: white;
            position: relative;
            z-index: 2;
            padding-bottom: 40px;
        }

        #home {
            background-color: rgba(0, 0, 0, 0.6); /* Transparent black background */
            border-radius: 10px; /* Round edges */
            padding: 20px; /* Add padding for better visibility */
            margin: 20px 0px 20px;
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

        #about {
            background-color: rgba(0, 0, 0, 0.6); /* Transparent black background */
            border-radius: 10px; /* Round edges */
            padding: 20px; /* Add padding for better visibility */
            margin: 20px 0px 20px;
        }

        #my-projects {
            background-color: rgba(0, 0, 0, 0.6);
            border-radius: 10px;
            padding: 20px;
        }

        .project-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 20px;
        }

        .project-cell {
            text-align: center;
            border: 2px solid white;
            border-radius: 10px;
            padding: 10px;
        }

        .image-scroll {
            display: flex;
            white-space: nowrap; /* Prevent images from wrapping to the next line */
            overflow-x: scroll;
        }

        .project-cell img {
            width: 400px; /* Adjust the width as needed */
            border-radius: 8px;
            margin: 0px, 20px, 0px; /* Adjust the spacing between images */
            
        }

        .project-cell p {
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
                <img src="Profile Pic small.jpg" alt="Profile Pic" style="width: 370px; 
                height: 400px; 
                margin-bottom: -8px;
                margin-left: -2px;
                margin-right: -2px;
                border-radius: 0px;">
                </div>
                </div>
            </div>
        </article>


        <article id="about">
    <div style="display: flex; justify-content: space-between; align-items: start;">
        <div style="flex: 1; text-align: left;">
            <!-- Text content on the left -->
            <h1>About Me</h1>
            <p></p>
        </div>
        <div style="flex: 1; text-align: center; padding-top: 10px;">
            <div style="display: inline-block; 
            border: 5px solid white; 
            align-items: stretch;
            overflow: hidden;
            /*border-radius: 8px; */
            /*padding: 4px;*/
            ">
                <img src="About_Me.jpg" alt="About Pic" style="width: 300px; 
                height: 550px; 
                margin-bottom: -8px;
                margin-left: -2px;
                margin-right: -2px;
                border-radius: 0px;">
                </div>
                </div>
            </div>
        </article>


       <article id="my-projects">
            <h2>My Projects</h2>
            
            <div class="project-grid">
                <div class="project-cell">
                    <div class="image-scroll">
                        <img src="PowerBI_dash1.png" alt="Project 1.1" style="margin: 0px 20px 10px;">
                        <img src="PowerBI_dash2.png" alt="Project 1.2" style="margin: 0px 20px 10px;">
                        <img src="PowerBI_dash3.png" alt="Project 1.3" style="margin: 0px 20px 10px;">
                    </div>
                    <p>Power BI report to visualize product status in product development pipeline</p>
                </div>


                <div class="project-cell">
                    <div class="image-scroll">
                        <img src="PowerBI_report.png" alt="Project 2.1" style="margin: 0px 20px 10px;
                        height: 200px;">
                        <img src="RMarkdown.png" alt="Project 2.2" style="margin: 0px 20px 10px;
                        height: 200px;">
                    </div>
                    <p>Paginated reports using Power BI Report Builder & R Markdown</p>
                </div>


                <div class="project-cell">
                    <img src="RShiny.png" alt="Project 3">
                    <p>Web based data visualization/analysis tools using R Shiny</p>
                </div>

                <div class="project-cell">
                    <img src="Rvisual_multipane2.png" alt="Project 4">
                    <p>Description for Project 4</p>
                </div>

                <div class="project-cell">
                    <img src="Rvisual_regression.png" alt="Project 5">
                    <p>Description for Project 5</p>
                </div>

                <div class="project-cell">
                    <img src="RMarkdown.png" alt="Project 6">
                    <p>Description for Project 6</p>
                </div>
            </div>
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
