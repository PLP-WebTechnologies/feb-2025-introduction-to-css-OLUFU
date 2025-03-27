# Introduction to CSS

## Objectives
Link an external CSS file to an HTML document.
Apply basic styling using selectors.
Use colors, fonts, and spacing effectively.

## Instructions

Create a style.css file.
Apply CSS to a HTML page.
Style elements using:
Classes and IDs.
Color and typography.
Margins, paddings, and borders.

>[!NOTE]
>  - Include at least:
>  - Use of 3 selectors
>  - Style an image
>  - Margin, Padding & Borders
>  - Different font

# Tasks
 - Link an external CSS file.
 - Apply at least 3 different selectors.
 - Improve readability and aesthetics.

Happy Coding! 💻✨

ANSWERS

1.style.css
file and apply CSS to a sample HTML page, demonstrating classes, IDs, color, typography, margins, padding, and borders.

1. HTML (index.html):

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Styling Example</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <header id="main-header">
        <h1>Welcome to My Website</h1>
        <p>A simple demonstration of CSS styling.</p>
    </header>

    <div class="container">
        <section class="content">
            <h2>About Us</h2>
            <p>This is some example content.  We're learning CSS and having fun!</p>
            <a href="#" class="button">Learn More</a>
        </section>

        <aside class="sidebar">
            <h3>Sidebar</h3>
            <ul>
                <li><a href="#">Link 1</a></li>
                <li><a href="#">Link 2</a></li>
                <li><a href="#">Link 3</a></li>
            </ul>
        </aside>
    </div>

    <footer id="main-footer">
        <p>&copy; 2023 My Website</p>
    </footer>

</body>
</html>


2. CSS (style.css):

/* General Styles */
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    background-color: #f4f4f4;
    color: #333;
}

/* Header Styles (ID) */
#main-header {
    background-color: #333;
    color: #fff;
    padding: 1rem 0; /* 1rem top and bottom, 0 left and right */
    text-align: center;
    border-bottom: 3px solid #008080; /* Teal border */
}

#main-header h1 {
    margin: 0; /* Remove default heading margin */
    font-size: 2.5rem;
}

#main-header p {
    font-style: italic;
}

/* Container Styles (Class) */
.container {
    width: 80%;
    margin: auto; /* Centers the container */
    overflow: hidden; /* Prevents content from overflowing */
    padding: 1rem 0; /* Add some padding */
}

/* Content Area Styles (Class) */
.content {
    float: left;
    width: 70%;
    padding: 1rem;
}

.content h2 {
    color: #008080; /* Teal Heading */
    margin-bottom: 0.5rem;
}

.content p {
    margin-bottom: 1rem;
}

/* Sidebar Styles (Class) */
.sidebar {
    float: right;
    width: 25%;
    background-color: #ddd;
    color: #333;
    padding: 1rem;
    margin-top: 1rem; /* Add top margin */
    border: 1px solid #ccc;
}

.sidebar ul {
    list-style: none; /* Remove bullet points */
    padding: 0;
}

.sidebar li {
    margin-bottom: 0.5rem;
}

.sidebar a {
    color: #008080;
    text-decoration: none;
}

.sidebar a:hover {
    text-decoration: underline;
}

/* Button Styles (Class) */
.button {
    background-color: #008080; /* Teal Background */
    color: #fff;
    padding: 0.5rem 1rem;
    text-decoration: none;
    border: none;
    border-radius: 5px; /* Rounded corners */
    cursor: pointer; /* Changes the cursor to a pointer on hover */
    display: inline-block; /* Allows setting width and height */
    margin-top: 10px;
}

.button:hover {
    background-color: #006666; /* Darker Teal on Hover */
}

/* Footer Styles (ID) */
#main-footer {
    background-color: #333;
    color: #fff;
    text-align: center;
    padding: 1rem 0;
    margin-top: 2rem;
