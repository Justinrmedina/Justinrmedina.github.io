<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Portfolio with Image Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }

        header {
            background-color: #333;
            color: #fff;
            padding: 20px;
            text-align: center;
        }

        section {
            padding: 20px;
        }

        h2 {
            color: #333;
        }

        .project {
            margin-bottom: 20px;
            padding: 15px;
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
            padding: 20px;
        }

        .image-container {
            margin: 10px;
            overflow: hidden;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            cursor: pointer;
            transition: transform 0.3s ease-in-out;
        }

        .image-container:hover {
            transform: scale(1.1);
        }

        .image-container img {
            width: 100%; /* Make the image take the full width of its container */
            height: auto; /* Maintain the aspect ratio */
            max-width: 300px; /* Set a maximum width to control the size */
            border-radius: 8px;
        }

        footer {
            text-align: center;
            padding: 20px;
        }
    </style>
</head>
<body>

    <header>
        <h1>Your Portfolio with Image Gallery</h1>
        <p>Showcasing data projects and beautiful images</p>
    </header>

    <section>
        <h2>Projects</h2>

        <div class="project">
            <h3>Project 1: Data Analysis</h3>
            <p>Description of the project and the tools/technologies used.</p>
            <a href="#">View Project</a>
        </div>

        <div class="project">
            <h3>Project 2: Data Visualization</h3>
            <p>Description of the project and the tools/technologies used.</p>
            <a href="#">View Project</a>
        </div>

        <!-- Add more projects as needed -->

    </section>

    <section>
        <h2>Image Gallery</h2>

        <div class="gallery">
            <!-- Add image containers here -->
            <div class="image-container">
                <img src="images/ANOVA.png" alt="Image 1">
            </div>
            <div class="image-container">
                <img src="images/ANOVA.png" alt="Image 2">
            </div>
            <!-- Add more image containers as needed -->
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Your Portfolio with Image Gallery</p>
    </footer>

</body>
</html>


