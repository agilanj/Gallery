# Ex.08 Design of Interactive Image Gallery
# Date: 14-12-2024
# AIM:
To design a web application for an inteactive image gallery with minimum five images.

# DESIGN STEPS:
## Step 1:
Clone the github repository and create Django admin interface.

## Step 2:
Change settings.py file to allow request from all hosts.

## Step 3:
Use CSS for positioning and styling.

## Step 4:
Write JavaScript program for implementing interactivity.

## Step 5:
Validate the HTML and CSS code.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Image Gallery</title>
    <style>
        #flexbox
        {
            /* border: 5px solid pink; */
            padding: 170px;
            background-image: url("footback.jpeg");
            background-repeat: no-repeat;
            background-size: cover;
        }
        #container1
        {
            /* margin-left:25%; */
            display: flex;
            background-color: whitesmoke; 
            gap: 20px;
            justify-content: center;
            padding: 20px;
            box-shadow: 0 2px 3px;
        }
        #container2
        {
            gap: 20px;
            display: flex;
            background-color: whitesmoke; 
            justify-content: center;
            /* border: 5px inset black; */
            padding: 10px;
            box-shadow:0 2px 3px;
        }
        .img
        {
            height: 190px;
            width: 260px;
            /* transform: rotate(-10deg); */
            image-rendering:optimizeQuality;    
            border: 2px inset whitesmoke;    
            border-radius: 10px;
            box-shadow:  0 0 10px black ;
            transition: 0.5s;
        }
        .img:hover
        {
            content: 'hello';
            transform: scale(1.3);
        }
        #divs
        {
            display: inline;
        }
        #image
        {
            z-index: 100;
            display: none;
            background: rgba(0,0,0,0.5);
            position: fixed;
            width: 100%;
            /* transform: rotate(20deg); */
            height: 100%;
            top: 0;
            bottom: 0;
            align-items: center;
            justify-content: center;    
        }
        #image img{
            width: 600px;
            height: auto;
        }
        #title
        {
            background-color: lightskyblue;
            border-radius: 10px;
            width: 500px;
            box-shadow: 0 3px 10px;
            position: absolute;
            top: 20px;
            left: 500px;
        }
    </style>
</head>
<body style="background-color:brown;">
    <section id="image">
            <img src="footback.jpeg" alt="" id="display" onclick="closes()">
    </section>
<div id="flexbox">

    <h1 align="center" ><span id="title"> Photo Gallery </span></h1>

    <div id="container1">
        <div class="divs"><img class="img" src="dhoni.webp" onclick="opens(this.src)" alt=""></div>
        <div class="divs"><img class="img" src="rutu.jpg" onclick="opens(this.src)"   alt=""></div>
        <div class="divs"><img class="img" src="jaddu.webp"  onclick="opens(this.src)"  alt=""></div>
        <div class="divs" ><img class="img" src="conway.webp" onclick="opens(this.src)"   alt=""></div>
    </div>
    <div id="container2">
        <div class="divs" ><img class="img" src="rachin.jpg" onclick="opens(this.src)"  alt=""></div>
        <div class="divs"><img class="img" src="dube.avif" onclick="opens(this.src)"  alt=""></div>
        <div class="divs" ><img class="img" src="ashwinr.png" onclick="opens(this.src)"  alt=""></div>
       <div class="divs"><img class="img" src="athirana.avif" onclick="opens(this.src)"  alt=""> </div>
    </div>
    
</div>
<footer align="center" style="background-color:grey">
    <p>Designed & Developed by Ameen Basha &copy; </p>
</footer>
    <script>
            var a =document.getElementById("image");
            var b=document.getElementById("display");
            function opens(c)
            {
                a.style.display='flex';
                b.src=c;
            }
            function closes()
            {
                a.style.display='none';
            }
    </script>
</body>
</html>
~~~
# OUTPUT:

![Screenshot (112)](https://github.com/user-attachments/assets/7add3ce9-b2a4-4f94-b968-55e8b56850d5)

![Screenshot (119)](https://github.com/user-attachments/assets/9ea3fef5-fd73-4a84-8eca-286fea49a704)

![Screenshot (120)](https://github.com/user-attachments/assets/df6f8ff1-b0dd-4b92-a7a6-25f6efd9c354)



# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
