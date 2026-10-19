Aim: To create an image section on a portfolio webpage using HTML and display images with correct paths and meaningful alternative text.

Question 1: Create a folder named images in your project.

Answer:

First, create a project folder named Assignment-3.2. Inside this folder, create an HTML file named index.html and another folder named images.

The folder structure will be:

Assignment-3.2/
│
├── index.html
│
└── images/
    ├── profile.jpg
    ├── coding.jpg
    └── webdesign.jpg

The images folder stores all the images used on the portfolio webpage.

Question 2: Add at least 3 images.

Answer:

Add the following three image files to the images folder:

profile.jpg — A profile photograph.

coding.jpg — An image showing programming or coding.

webdesign.jpg — An image related to website design.

These images can be downloaded from a suitable source or selected from your computer. Make sure that the filenames and extensions match the HTML code.

Question 3: Use src, alt, width, and height in the <img> tag.

Answer:

The HTML <img> tag is used to display images on a webpage. The src attribute specifies the image path, alt provides alternative text, and width and height define the image dimensions.

Example:

<img
    src="images/profile.jpg"
    alt="Profile photograph representing the portfolio owner"
    width="250"
    height="180">

Explanation:

src: Specifies the location of the image file.

alt: Describes the image for accessibility and when the image cannot load.

width: Sets the image width to 250 pixels.

height: Sets the image height to 180 pixels.

Question 4: Keep image paths correct.

Answer:

Image paths must correctly point to the location of the image files. Since all three images are stored inside the images folder, their relative paths are:

<img src="images/profile.jpg" alt="Profile photograph">
<img src="images/coding.jpg" alt="Computer screen displaying programming code">
<img src="images/webdesign.jpg" alt="Website design workspace">

The index.html file and the images folder must be inside the same project folder. Filenames, extensions, and uppercase or lowercase letters must match the actual files.

Question 5: Write meaningful alt text for each image.

Answer:

The alt attribute provides a text description of an image. It helps screen-reader users understand the image and provides alternative text if the image fails to load.

Examples of meaningful alt text:

<img
    src="images/profile.jpg"
    alt="Profile photograph representing the portfolio owner"
    width="250"
    height="180">

<img
    src="images/coding.jpg"
    alt="Computer screen displaying programming code"
    width="250"
    height="180">

<img
    src="images/webdesign.jpg"
    alt="Web design workspace showing a website layout on a computer"
    width="250"
    height="180">

Each alt description explains the purpose or content of its corresponding image.

Question 6: Check that images are loading properly in the browser.

Answer:

Follow these steps to verify that all images load correctly:

Save the index.html file.

Place all three images inside the images folder.

Open index.html in a web browser or use Live Server in Visual Studio Code.

Check that all three images appear correctly on the portfolio webpage.

If an image does not appear, verify its filename, extension, folder location, and path in the src attribute.

After checking all images, take a screenshot of the working webpage for submission.

Complete HTML Code

Create a file named index.html and paste the following code into it.

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio - Images in HTML</title>

    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            background-color: #f4f7fb;
            color: #333;
        }

        header {
            background-color: #174ea6;
            color: white;
            text-align: center;
            padding: 25px;
        }

        main {
            max-width: 1000px;
            margin: 30px auto;
            padding: 20px;
        }

        h2 {
            color: #174ea6;
            text-align: center;
        }

        .gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }

        .image-card {
            width: 270px;
            padding: 15px;
            background-color: white;
            text-align: center;
            border-radius: 10px;
            box-shadow: 0 3px 10px #00000015;
        }

        .image-card img {
            width: 250px;
            height: 180px;
            object-fit: cover;
            border-radius: 8px;
        }

        footer {
            background-color: #123b7a;
            color: white;
            text-align: center;
            padding: 15px;
        }
    </style>
</head>

<body>

    <header>
        <h1>My Personal Portfolio</h1>
        <p>Welcome to My Portfolio Website</p>
    </header>

    <main>
        <section>
            <h2>About Me</h2>
            <p>
                Hello! I am a B.Tech Computer Science student
                interested in programming, technology, and
                web development. This portfolio demonstrates
                how images can be added using HTML.
            </p>
        </section>

        <section>
            <h2>My Image Gallery</h2>

            <div class="gallery">

                <div class="image-card">
                    <img
                        src="images/profile.jpg"
                        alt="Profile photograph representing the portfolio owner"
                        width="250"
                        height="180">
                    <h3>My Profile</h3>
                    <p>A profile image for my portfolio.</p>
                </div>

                <div class="image-card">
                    <img
                        src="images/coding.jpg"
                        alt="Computer screen displaying programming code"
                        width="250"
                        height="180">
                    <h3>Coding</h3>
                    <p>Programming is used to develop software and websites.</p>
                </div>

                <div class="image-card">
                    <img
                        src="images/webdesign.jpg"
                        alt="Web design workspace showing a website layout on a computer"
                        width="250"
                        height="180">
                    <h3>Web Development</h3>
                    <p>Web development helps create useful websites.</p>
                </div>

            </div>
        </section>
    </main>

    <footer>
        <p>Copyright 2026 | My Personal Portfolio</p>
    </footer>

</body>
</html>

Result

A portfolio webpage with three images was created using HTML and CSS. Each image has a correct source path, suitable dimensions, and meaningful alternative text. All images are checked in the browser.

Submission

Submit the following files:

index.html

The images folder containing profile.jpg, coding.jpg, and webdesign.jpg.

A screenshot showing the portfolio page with all three images displayed correctly.