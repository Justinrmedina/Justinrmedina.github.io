<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Portfolio with Single Image Gallery</title>
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

        .gallery-container {
            position: relative;
            overflow: hidden;
            white-space: nowrap;
            margin-bottom: 20px;
        }

        .gallery {
            display: flex;
            transition: transform 0.3s ease-in-out;
        }

        .image-container {
            margin: 10px;
            overflow: hidden;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            cursor: pointer;
            transition: transform 0.3s ease-in-out;
            flex: 0 0 auto; /* Allow the image to shrink if needed */
        }

        .image-container:hover {
            transform: scale(1.1);
        }

        .image-container img {
            width: 100%;
            height: auto;
            max-width: 750px; /* Adjust this value to control the maximum width of the images */
            max-height: 450px; /* Adjust this value to control the maximum height of the images */
            border-radius: 8px;
        }

        .prev, .next {
            position: absolute;
            top: 50%;
            transform: translateY(-50%);
            font-size: 24px;
            cursor: pointer;
            color: #333;
            background: none;
            border: none;
            outline: none;
        }

        .prev {
            left: 10px;
        }

        .next {
            right: 10px;
        }

        footer {
            text-align: center;
            padding: 20px;
        }
    </style>
</head>
<body>

    <header>
        <h1>Your Portfolio with Single Image Gallery</h1>
        <p>Showcasing data projects and a navigable image gallery with larger images</p>
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

        <div class="gallery-container">
            <button class="prev" onclick="scrollGallery(-1)">❮</button>
            <div class="gallery">
                <!-- Add image containers here -->
                <div class="image-container">
                    <img src="ANOVA small.png" alt="Image 1">
                </div>
                <div class="image-container">
                    <img src="ANOVA small.png" alt="Image 2">
                </div>
                <!-- Add more image containers as needed -->
            </div>
            <button class="next" onclick="scrollGallery(1)">❯</button>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Your Portfolio with Single Image Gallery</p>
    </footer>

    <script>
        let currentIndex = 0;
        const gallery = document.querySelector('.gallery');

        function scrollGallery(direction) {
            const imageContainers = document.querySelectorAll('.image-container');
            const containerWidth = gallery.clientWidth;

            currentIndex += direction;
            if (currentIndex < 0) {
                currentIndex = 0;
            } else if (currentIndex > imageContainers.length - 1) {
                currentIndex = imageContainers.length - 1;
            }

            const translateValue = -currentIndex * containerWidth;
            gallery.style.transform = `translateX(${translateValue}px)`;
        }
    </script>
</body>
</html>




