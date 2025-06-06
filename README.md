# Ex.08 Design of Interactive Image Gallery
# Date: 12.05.2025
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

```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Image Gallery</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background-image: url('bg3.jpg');
            background-repeat: no-repeat;
            background-size: cover;
        }

        header {
            text-align: center;
            font-size: 30px;
            font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
            color: white;
        }

        div img {
            width: 300px;
            height: 300px;
            cursor: pointer;
            border-radius: 10px;
        }
        .img{
            overflow: hidden;
        }
        div{
            transition: 0.25s;
        }

        div :hover {
            transform: scale(1.1);
            border-radius: 10px;
        }
        
        
        .col1 {
            display: flex;
            gap: 30px;
            margin-top: 30px;
            justify-content: center;
        }
        .col2 {
            display: flex;
            gap: 30px;
            margin-top: 30px;
            justify-content: center;
        }

        

        span {
            color: white;
            position: absolute;
            top: 5%;
            right: 5%;
            font-size: 50px;
            cursor: pointer;
        }
        #dis{
            width: 100%;
            height: 100%;
            background: rgba(0,0,0,0.8);
            position: fixed;
            top: 0;
            bottom: 0;
            display: none;
            align-items: center;
            justify-content: center;
            z-index: 100;
        }
        #dis img{
            width: 500px;
            height: 600px;
        }
        .footer{
            text-align: center;
            margin-bottom:5%;
            background-color:whitesmoke;
            color:rgb(11, 10, 10);
            font-family:'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif;
            font-size: 25px;
        }
    </style>
    
</head>

<body>
    <header>
        <h1>My Image Gallery</h1>
    </header>
    <section id="dis">
        <img src="bg3.jpg" alt="" id="disimg">
        <span class="cls" onclick="closes()">&times;</span>
        
    </section>
    <div class="col1">
        <div class="img">
            <img src="img1.jpg" opens(this.src)" id="img1" alt="">
        </div>
        <div class="img">
            <img src="img2.jpg" opens(this.src)" id="img2" alt="">
        </div>
        <div class="img">
            <img src="img3.jpg" onclick="opens(this.src)" id="img3" alt="">
        </div>
        <div class="img">
            <img src="img4.jpg" onclick="opens(this.src)" id="img4" alt="">
        </div>
    </div>
    <div class="col2">
        <div class="img">
            <img src="img5.jpg" onclick="opens(this.src)" id="img5" alt="">
        </div>
        <div class="img">
            <img src="img6.jpg" onclick="opens(this.src)" id="img6" alt="">
        </div>
        <div class="img">
            <img src="img7.jpg" onclick="opens(this.src)" id="img7" alt="">
        </div>
        <div class="img">
            <img src="img8.jpg" onclick="opens(this.src)" id="img8" alt="">
        </div>

    </div>
    <div class="footer">
        <footer>
            Designed by Asin Renix V &copy; 2024 
       </footer>
    </div>
    

    <script>
        var dis=document.getElementById("dis");
        var disimg=document.getElementById("disimg");
        function opens(image){
            dis.style.display="flex";
            disimg.src=image;
        }
        function closes(){
            dis.style.display="none";

        }
    </script>

</body>

</html>

```
# OUTPUT:
![image](https://github.com/user-attachments/assets/f7976511-e3df-46d3-9b14-b5ac2c52c3c9)

![image](https://github.com/user-attachments/assets/09f89565-d14b-44fc-b703-7f13e40d74ab)

![image](https://github.com/user-attachments/assets/051033c1-06fc-41c2-86d1-0e21a2070455)


# RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
