name: k.sanjeevpriya
212224040289
# Ex.08 Design of Interactive Image Gallery
## Date:09-05-2025

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial;
}

.column {
  float: left;
  width: 20%;
  padding: 10px;
}


.column img {
  opacity: 0.8; 
  cursor: pointer; 
}

.column img:hover {
  opacity: 1;
}


.row:after {
  content: "";
  display: table;
  clear: both;
}


.container {
  position: relative;
  display: none;
}


#imgtext {
  position: absolute;
  bottom: 15px;
  left: 15px;
  color: white;
  font-size: 20px;
}


.closebtn {
  position: absolute;
  top: 10px;
  right: 15px;
  color: white;
  font-size: 35px;
  cursor: pointer;
}
</style>
</head>
<body>

<div style="text-align:center">
  <h2>Image Gallery</h2>
  <p>Click on the images below:</p>
</div>


<div class="row">
  <div class="column">
    <img src="blue.jpg" alt="Music" style="width:100%" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="music.jpg" alt="Snow" style="width:100%" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="tech.jpg" alt="Mountains" style="width:100%" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="coffeebook.jpg" alt="Lights" style="width:100%" onclick="myFunction(this);">
  </div>
  <div class="column">
    <img src="moon.jpg" alt="Lights" style="width:100%" onclick="myFunction(this);">
  </div>
</div>

<div class="container">
  <span onclick="this.parentElement.style.display='none'" class="closebtn">&times;</span>
  <img id="expandedImg" style="width:100%">
  <div id="imgtext"></div>
</div>

<script>
function myFunction(imgs) {
  var expandImg = document.getElementById("expandedImg");
  var imgText = document.getElementById("imgtext");
  expandImg.src = imgs.src;
  imgText.innerHTML = imgs.alt;
  expandImg.parentElement.style.display = "block";
}
</script>

</body>
</html>
```

## OUTPUT:
![Screenshot 2025-05-09 085024](https://github.com/user-attachments/assets/9f6e0e28-4159-413b-9f3f-270aa13f0aac)


## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
