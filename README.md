# Jalen-Allison.github.io
 BIN +48.8 KB Jalens-Portfolio/images/GitHub.png 

 BIN +545 KB Jalens-Portfolio/images/contactus.jpg 

 BIN +122 KB Jalens-Portfolio/images/curiositypicture.jpg 

 BIN +5.29 MB Jalens-Portfolio/images/video/coding2.mp4 
Binary file not shown.
 126  Jalens-Portfolio/index.html 
@@ -0,0 +1,126 @@
<!DOCTYPE html>
<html>
    <!--Head-->
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width" />
        <title>Jalen Allison</title>
        <link rel="stylesheet" type="text/css" href="stylesheet/portfolio2.css">
    </head>

    <!--Body-->
    <body class="Background">

        <!--Navbar-->
        <div class="Navbar">
            <a class="active" href="#Home">Home</a>
            <a href="#About">About</a>
            <a href="#GitHub">GitHub</a>
            <a href="#Contact">Contact</a>
        </div>

        <br>
        <br>

        <!--Background video-->
        <div id="Home">
            <video autoplay muted loop id="Coding2">
                <source src="images/video/Coding2.mp4" type="video/mp4">
                <!--Display message if video fails to run-->
                Your browser does not support HTML5 video.
            </video>
        </div>

        <!--Video text-->
        <div class="Coding2_Text">
            <h1 class="white-text">Jalens Portfolio</h1>
            <strong>
                <p class="center">
                    <q>Programming isn't about what you know; it's about what you can figure out.</q><br>
                    <br> -Chris Pine
                    <br>
                    <br> My name is Jalen Allison. Welcome to my portfolio website. On it, I will tell you about my background and experience.
                    <br>
                    <br> Thank you for stopping by and enjoy! 
                </p>
            </strong>
        </div>

        <!--About section-->
        <div class="Row" id="About">
            <!--Left column-->
            <div class="Column_2">
                <img src="images/curiositypicture.jpg" alt="curiosity pic">
            </div>
            <!--Right column-->
            <div class="Column_1">
                <h1>About</h1>
                <p>
                    I am a future software developer and work in the admissions department at The Tech Academy. 
                    I was an athlete my whole life and have always loved working towards goals to achieve. 
                    I played football for and graduated with a Bachelor's of Science degree from North Dakota State University. <br>
                    I began working at the The Tech Academy and was introduced to the world of coding. My curiosity and interest 
                    began to grow more and more as I started learning the basics about the different languages. I decided to take 
                    the software development course since it's the most comprehensive and it teaches the most languages which will
                    make me a well rounded developer.
                    I am very excited to continue to learn and develope my skill set as I progress through my career.
                    Follow my portfolio as I learn the languages of HTML & CSS, JavaScript, Python, Database & SQL, C#, C# and .NET along 
                    with a project management course.

                    <br>
                    <br>I am a future graduate of <a href="https://www.learncodinganywhere.com" target="_blank">The Tech Academy</a>’s Software Developer Boot Camp, and trained and experienced in the following web and programming languages: HTML, CSS, JavaScript, SQL, C# and more. 
                    <br>
                    <br>I will be a full-stack developer and would love to work with you on your project. <a href="#Contact">Contact</a> me below!
                </p>
            </div>
        </div>

        <!--GitHub section-->
        <div class="Row" id="GitHub">
            <!--Left column-->
            <div class="Column_1">
                <h1>GitHub</h1>
                <p>
                    You can view my coding projects on my GitHub profile here: 
                    <br>
                    <p class="center"><a href="https://github.com/Jalen-Allison" target="_blank">Jalens Github</a></p>
                </p>
            </div>
            <!--Right column-->
            <div class="Column_2">
                <a href="https://github.com/Jalen-Allison" target="_blank"><img src="images/GitHub.png" alt="GitHub Logo"></a>
            </div>
        </div>

        <!--Contact section-->
        <div class="Row" id="Contact">
            <!--Contact image, left column-->
            <div class="Column_2 Column_tall">
                <img src="images/contactus.jpg" alt="Contact_Image">
            </div>

             <!--Contact form, right column-->
             <div class="Column_1 Column_tall">
                <h1>Contact</h1>

                <form action="" method="POST"> <!-- Here we are utilizing a 3rd party service to submit the contact form data, insert your formspree endpoint in the action attribute -->
                    <label>Name:</label>
                        <input type="text" placeholder="Please enter your name here">
                    <label>Email:</label>
                        <input type="text" id="Email" name="Email" placeholder="Please enter your email here">
                    <label>Message:</label>
                        <input type="text" id="Message" name="Message" placeholder="Please write your message here">
                        <input type="submit" value="SUBMIT">
                </form>
            </div>
        </div>

        <!--Footer section-->
        <footer>
            <p>
                <p class="center">&copy Jalens Website <a href="jalenallisonportfolio.com" target="_blank">Jalens Website</a></p>
                <br>
            </p>
        </footer>
    </body>
</html> 
 285  Jalens-Portfolio/portfolio2.css 
@@ -0,0 +1,285 @@
/***** GENERAL STYLING *****/
/* Body */
body {
    margin: 0%  /* This ensures our site displays all the way to the edge of the browser screen */
}

/* Styling for portfolio title text */
.white-text {
    color: goldenrod; /* This is used to change the color of the portfolio title text */
}

/***** NAVBAR STYLING *****/
.Navbar {
overflow: hidden; 
background-color: rgb(20, 20, 20);
position: fixed;
top: 0;
width: 100%;
z-index: 1;
-webkit-animation: moveNav 5s;
animation: moveNav 5s;
}

/* moveNav animation effect for moving the nav bar in from the left of the screen */
@keyframes moveNav {
    from {left: -100vw;}
    to {left: 0vw}
}


.Navbar a {
    float: left;
    display: block;
    color: silver;
    padding: 14px 16px;
    text-decoration: none;
    font-family: Avant Garde, Helvetica;
    font-size: 20px;
    text-align: center;
    position: relative;
    -webkit-animation: moveNavText 5.75s;
    animation: moveNavText 5.75s;
}

@keyframes moveNav {
    from {left: -100vw;}
    to {left: 0vw}
}

@media screen and (max-width: 576px) {
    .Navbar a{
        width: 25%; /* This makes each link take up 1/4 of the navbar */
        font-size: 12px;
    }
}

.Navbar a:hover {
    background-color: black; 
    color: goldenrod; 
    font-weight: bold;
}

.Navbar a.active {
    background-color: rgba(192, 192, 192, 0.644);
}
/***** END OF NAVBAR STYLING *****/

/***** VIDEO STYLING *****/
/* Formatting for background video */
#Coding2 {
    position: fixed;
    right: 0;
    bottom: 0;
    min-width: 100%;
    z-index: -1;
}

/* Screens that are 576px and smaller will not display the background video */
@media screen and (max-width: 576px) {
    #Coding2 {
        display: none;
    }
}

/* Texts over the video */
.Coding2_Text {
    background: rgba(0, 0, 0, 0.5);
    color: white;
    width: 100%;
    padding: 20px;
    position: relative;
    -webkit-animation: moveVideoText 5.75s;
    animation: moveVideoText 5.75s;
}

@keyframes moveVideoText {
    from {top: -100vw;} /* This sets the position of the video text to above the viewport */
    to {top: 0vw;} /* This moves the video text to the normal positioning on the viewport */
}
/***** END OF VIDEO STYLING *****/

/***** TABLE STYLING*/
* { /* The asterisk is a universal selector that applies this effect to all elements on the page */
    box-sizing: border-box;
}

.Column_1 {
    float: left;
    width: 50%;
    padding: 10px;
    padding-top: 3%;
    height: 400px;
    background-color: goldenrod;
}

/* Screens 576px and smaller will display a scroll bar if the text overflows the column height */
@media screen and (max-width: 576px) {
    .Column_1 {
        overflow: auto;
    }
}

.Column_2 {
    float: left;
    width: 50%;
    padding: 10px;
    padding-top: 1.9%;
    height: 400px;
    background-color: rgba(0, 0, 0, 0.856);
}

/* This class is applied to the columns in the final row, overriding the height and padding to provide more room for the contact form  while keeping the rest of the formatting from Column_1 or Column_2 */
.Column_tall {
    padding-top: 3.5%;
    height: 450px;
}

/* This inserts something after the content of selected elements (in this case the elements with class "Row") */
.Row:after {
    content: "";
    display: table;
    clear: both;
}
/***** END OF TABLE STYLING *****/

/* Image elements */
img {
    filter: grayscale(70%);
    border-radius: 8px;
    max-width: 100%;
    height: 340px;
    display: block;
    margin-left: auto;
    margin-right: auto;
}

/* Image element hover effects */
img:hover {
    filter: grayscale(5%);
    transition: transform 1s;
    transform: scale(1.03);
}

@media screen and (max-width: 576px) {
    img {
        height: 100px;
        margin-top: 150px;
    }
}

/* Heading 1 elements */
h1 {
    text-transform: uppercase;
    font-family: "Trebuchet MS", Optima;
    text-align: center;
    margin-top: 2%;
    color: white;
}

/* Heading 1 element hover effect */
h1:hover {
    filter: grayscale(5%);
    transform: scale(1.1);
    transition: transform 1s;
}

/* Paragraph elements */
p {
    font-family: Optima;
    text-align: center;
    letter-spacing: 1px;
    font-size: 14px;
    padding-left: 12px;
    padding-right: 12px;
    padding-bottom: 15px;
}

/* Paragraph element hover effect */
p:hover {
    transition: transform 1s;
    transform: scale(1.05);
}

/* Center class - this applies to all elements with the class "center" */
.center {
    text-align: center; /* This center aligns the text */
}

.center {
    text-align: center; /* This center aligns the text */
}

/* Center class hover effect - This only affects the quote, github link, and footer */
.center:hover {
    transition: transform 2s;
    transform: scale(1.1);
}

/* Anchor elements */
a {
    color: blue; /* This ensures all links are blue */
}

/* Quotation elements */
q {
    font-style: italic; /* This makes the quote italicized */
}

/* Styling for footer element */
footer {
    padding: 2%; /* This gives the footer padding that is equal to 2% of the width of the element's area */
    background-color: white;
}
/***** END OF GENERAL STYLING *****/

/***** CONTACT FORM STYLING *****/
/* input[type=text] targets all text input sections of the contact form */
input[type=text] {
    width: 100%;
    padding: 12px;
    border: 1px solid white;
    border-radius: 4px;
    box-sizing: border-box;
    margin-top: 6px;
    margin-bottom: 16px;
    resize: vertical;
    font-family: Perpetua, Rockwell Extra Bold;
}

/* Hover effects for input boxes */
input[type=text]:hover {
    box-shadow: 0 0 10px goldenrod inset; /* This creates a golden shadow in the text box when hovered over by the user */
}

/* Submit button */
input[type=submit] {
    background-color: black;
    color: white;
    font-weight: bold;
    padding: 12px 20px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    display: block;
    margin-left: auto;
    margin-right: auto;
    font-family: Perpetua, Rockwell Extra Bold;
}

/* Hover effect for submit button */
input[type=submit]:hover {
    background-color: white;
    color: black;
    transform: scale(1.5);
    transition: transform 1.5s;
}

/* Form element */
form {
    border-radius: 5px; /* Rounds the corners of the contact form */
    background-color: #f2f2f2; 
    padding: 10px; /* Adds padding to the contact form */
    font-family: "Trebuchet MS", Optima;
}
/***** END OF CONTACT FORM STYLING *****/ 
 285  Jalens-Portfolio/stylesheet/portfolio2.css 
@@ -0,0 +1,285 @@
/***** GENERAL STYLING *****/
/* Body */
body {
    margin: 0%  /* This ensures our site displays all the way to the edge of the browser screen */
}

/* Styling for portfolio title text */
.white-text {
    color: goldenrod; /* This is used to change the color of the portfolio title text */
}

/***** NAVBAR STYLING *****/
.Navbar {
overflow: hidden; 
background-color: rgb(20, 20, 20);
position: fixed;
top: 0;
width: 100%;
z-index: 1;
-webkit-animation: moveNav 5s;
animation: moveNav 5s;
}

/* moveNav animation effect for moving the nav bar in from the left of the screen */
@keyframes moveNav {
    from {left: -100vw;}
    to {left: 0vw}
}


.Navbar a {
    float: left;
    display: block;
    color: silver;
    padding: 14px 16px;
    text-decoration: none;
    font-family: Avant Garde, Helvetica;
    font-size: 20px;
    text-align: center;
    position: relative;
    -webkit-animation: moveNavText 5.75s;
    animation: moveNavText 5.75s;
}

@keyframes moveNav {
    from {left: -100vw;}
    to {left: 0vw}
}

@media screen and (max-width: 576px) {
    .Navbar a{
        width: 25%; /* This makes each link take up 1/4 of the navbar */
        font-size: 12px;
    }
}

.Navbar a:hover {
    background-color: black; 
    color: goldenrod; 
    font-weight: bold;
}

.Navbar a.active {
    background-color: rgba(192, 192, 192, 0.644);
}
/***** END OF NAVBAR STYLING *****/

/***** VIDEO STYLING *****/
/* Formatting for background video */
#Coding2 {
    position: fixed;
    right: 0;
    bottom: 0;
    min-width: 100%;
    z-index: -1;
}

/* Screens that are 576px and smaller will not display the background video */
@media screen and (max-width: 576px) {
    #Coding2 {
        display: none;
    }
}

/* Texts over the video */
.Coding2_Text {
    background: rgba(0, 0, 0, 0.5);
    color: white;
    width: 100%;
    padding: 20px;
    position: relative;
    -webkit-animation: moveVideoText 5.75s;
    animation: moveVideoText 5.75s;
}

@keyframes moveVideoText {
    from {top: -100vw;} /* This sets the position of the video text to above the viewport */
    to {top: 0vw;} /* This moves the video text to the normal positioning on the viewport */
}
/***** END OF VIDEO STYLING *****/

/***** TABLE STYLING*/
* { /* The asterisk is a universal selector that applies this effect to all elements on the page */
    box-sizing: border-box;
}

.Column_1 {
    float: left;
    width: 50%;
    padding: 10px;
    padding-top: 3%;
    height: 400px;
    background-color: goldenrod;
}

/* Screens 576px and smaller will display a scroll bar if the text overflows the column height */
@media screen and (max-width: 576px) {
    .Column_1 {
        overflow: auto;
    }
}

.Column_2 {
    float: left;
    width: 50%;
    padding: 10px;
    padding-top: 1.9%;
    height: 400px;
    background-color: rgba(0, 0, 0, 0.856);
}

/* This class is applied to the columns in the final row, overriding the height and padding to provide more room for the contact form  while keeping the rest of the formatting from Column_1 or Column_2 */
.Column_tall {
    padding-top: 3.5%;
    height: 450px;
}

/* This inserts something after the content of selected elements (in this case the elements with class "Row") */
.Row:after {
    content: "";
    display: table;
    clear: both;
}
/***** END OF TABLE STYLING *****/

/* Image elements */
img {
    filter: grayscale(70%);
    border-radius: 8px;
    max-width: 100%;
    height: 340px;
    display: block;
    margin-left: auto;
    margin-right: auto;
}

/* Image element hover effects */
img:hover {
    filter: grayscale(5%);
    transition: transform 1s;
    transform: scale(1.03);
}

@media screen and (max-width: 576px) {
    img {
        height: 100px;
        margin-top: 150px;
    }
}

/* Heading 1 elements */
h1 {
    text-transform: uppercase;
    font-family: "Trebuchet MS", Optima;
    text-align: center;
    margin-top: 2%;
    color: white;
}

/* Heading 1 element hover effect */
h1:hover {
    filter: grayscale(5%);
    transform: scale(1.1);
    transition: transform 1s;
}

/* Paragraph elements */
p {
    font-family: Optima;
    text-align: center;
    letter-spacing: 1px;
    font-size: 14px;
    padding-left: 12px;
    padding-right: 12px;
    padding-bottom: 15px;
}

/* Paragraph element hover effect */
p:hover {
    transition: transform 1s;
    transform: scale(1.05);
}

/* Center class - this applies to all elements with the class "center" */
.center {
    text-align: center; /* This center aligns the text */
}

.center {
    text-align: center; /* This center aligns the text */
}

/* Center class hover effect - This only affects the quote, github link, and footer */
.center:hover {
    transition: transform 2s;
    transform: scale(1.1);
}

/* Anchor elements */
a {
    color: blue; /* This ensures all links are blue */
}

/* Quotation elements */
q {
    font-style: italic; /* This makes the quote italicized */
}

/* Styling for footer element */
footer {
    padding: 2%; /* This gives the footer padding that is equal to 2% of the width of the element's area */
    background-color: white;
}
/***** END OF GENERAL STYLING *****/

/***** CONTACT FORM STYLING *****/
/* input[type=text] targets all text input sections of the contact form */
input[type=text] {
    width: 100%;
    padding: 12px;
    border: 1px solid white;
    border-radius: 4px;
    box-sizing: border-box;
    margin-top: 6px;
    margin-bottom: 16px;
    resize: vertical;
    font-family: Perpetua, Rockwell Extra Bold;
}

/* Hover effects for input boxes */
input[type=text]:hover {
    box-shadow: 0 0 10px goldenrod inset; /* This creates a golden shadow in the text box when hovered over by the user */
}

/* Submit button */
input[type=submit] {
    background-color: black;
    color: white;
    font-weight: bold;
    padding: 12px 20px;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    display: block;
    margin-left: auto;
    margin-right: auto;
    font-family: Perpetua, Rockwell Extra Bold;
}

/* Hover effect for submit button */
input[type=submit]:hover {
    background-color: white;
    color: black;
    transform: scale(1.5);
    transition: transform 1.5s;
}

/* Form element */
form {
    border-radius: 5px; /* Rounds the corners of the contact form */
    background-color: #f2f2f2; 
    padding: 10px; /* Adds padding to the contact form */
    font-family: "Trebuchet MS", Optima;
}
/***** END OF CONTACT FORM STYLING *****/ 
