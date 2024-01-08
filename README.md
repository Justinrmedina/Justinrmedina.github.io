<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Dynamic Image Gallery with Larger Image</title>
    <style>
        /* Your CSS styles go here */

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
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .gallery {
            display: flex;
            transition: transform 0.3s ease-in-out;
            overflow: hidden;
        }

        .image-container {
            position: center;
            margin: 10px;
            overflow: hidden;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            cursor: pointer;
            transition: transform 0.3s ease-in-out;
            flex: 0 0 auto;
        }

        .image-container:hover {
            transform: scale(1.1);
        }

        .image-container img {
            width: 100%;
            height: auto;
            max-width: 800px;
            max-height: 500px;
            border-radius: 8px;
        }

        .image-link {
            text-decoration: none;
            color: inherit;
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
            margin: 0 10px; /* Add margin to create space between arrows and images */
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
        <h1>Your Dynamic Image Gallery with Larger Image</h1>
        <p>Showcasing data projects and a dynamically generated image gallery</p>
    </header>

    <section>
        <h2>Projects</h2>

        <!-- Example projects -->
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
            <div class="gallery" id="dynamic-gallery">
                <!-- Images will be dynamically added here -->
            </div>
            <button class="next" onclick="scrollGallery(1)">❯</button>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 Your Dynamic Image Gallery</p>
    </footer>

    <script>
        const gallery = document.getElementById('dynamic-gallery');
        const images = [
            'ANOVA small.png',
            'ANOVA small.png',
            'ANOVA small.png',
            'ANOVA small.png',
            // Add more image URLs as needed
        ];

        images.forEach((imageUrl) => {
            const imageContainer = document.createElement('div');
            imageContainer.className = 'image-container';

            const imageLink = document.createElement('a');
            imageLink.href = imageUrl;
            imageLink.target = '_blank';
            imageLink.className = 'image-link';

            const image = document.createElement('img');
            image.src = imageUrl;
            image.alt = 'Gallery Image';

            imageLink.appendChild(image);
            imageContainer.appendChild(imageLink);
            gallery.appendChild(imageContainer);
        });

        let currentIndex = 0;

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







