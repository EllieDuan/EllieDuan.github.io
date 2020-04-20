---
layout: default
---

<html>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
body {
  font-family: Arial;
  margin: 0;
}

/* Add CSS */
* {
  box-sizing: border-box;
}

img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}

/* Position the image container (needed to position the left and right arrows) */

.container {
  position: relative;
}

/* Hide the images by default */
.mySlides {
  display: none;
}

/* Add a pointer when hovering over the thumbnail images */
.cursor {
  cursor: pointer;
}

/* Next & previous buttons */
.prev,
.next {
  cursor: pointer;
  position: absolute;
  top: 40%;
  width: auto;
  padding: 16px;
  margin-top: -50px;
  color: black;
  font-weight: bold;
  font-size: 20px;
  border-radius: 0 3px 3px 0;
  user-select: none;
  -webkit-user-select: none;
}

/* Position the "next button" to the right */
.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}

/* On hover, add a black background color with a little bit see-through */
.prev:hover,
.next:hover {
  background-color: rgba(0, 0, 0, 0.8);
}

/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}

/* Container for image text */
.caption-container {
  text-align: center;
  background-color: #222;
  padding: 2px 16px;
  color: white;
}


.row:after {
  content: "";
  display: table;
  clear: both;
}

/* 9 columns side by side */
.column {
  float: left;
  width: 11.11%;
}

/* Add a transparency effect for thumnbail images */
.demo {
  opacity: 0.6;
}

.active,
.demo:hover {
  opacity: 1;
}
</style>

<body>
<h2 style="text-align:center">Adobe Illustrator Design</h2>

<!-- Container for the image gallery -->
<div class="container">

  <!-- Full-width images with number text -->
  <div class="mySlides">
    <div class="numbertext">1 / 9</div>
    <img src="/img/adobe_illustrator/class8_homework_ellie_happyholoday.png"  style="width:auto, height:500px">
  </div>
  
  <div class="mySlides">
    <div class="numbertext">2 / 9</div>
    <img src="/img/adobe_illustrator/Ellie_mooncake.png" style="width:auto, height:500px">
  </div>

  <div class="mySlides">
    <div class="numbertext">3 / 9</div>
    <img src="/img/adobe_illustrator/hungarian_door_Ellie.png" style="width:auto, height:500px">
  </div>

  <div class="mySlides">
    <div class="numbertext">4 / 9</div>
    <img src="/img/adobe_illustrator/homework3_ellie.png" style="width:auto, height:500px">
  </div>
 
  <div class="mySlides">
    <div class="numbertext">5 / 9</div>
    <img src="/img/adobe_illustrator/Roger_william_zoo_Ellie.png" style="width:auto, height:500px">
  </div>

  <div class="mySlides">
    <div class="numbertext">6 / 9</div>
    <img src="/img/adobe_illustrator/Ellie_menu.png" style="width:auto, height:500px">
  </div>
    
   <div class="mySlides">
    <div class="numbertext">7 / 9</div>
    <img src="/img/adobe_illustrator/Asset_3.png" style="width:auto, height:500px">
  </div>
  
   <div class="mySlides">
    <div class="numbertext">8 / 9</div>
    <img src="/img/adobe_illustrator/Asset_4.png" style="width:auto, height:500px">
  </div>
  
   <div class="mySlides">
    <div class="numbertext">9 / 9</div>
    <img src="/img/adobe_illustrator/Final_project_ellie.png" style="width:auto, height:500px">
  </div>
  
  <!-- Next and previous buttons -->
  <a class="prev" onclick="plusSlides(-1)">❮</a>
  <a class="next" onclick="plusSlides(1)">❯</a>
  
  <!-- Image text -->
  <div class="caption-container">
    <p id="caption"></p>
  </div>
  
  <!-- Thumbnail images -->
  <div class="row">
    <div class="column">
    <img class="demo cursor" src="/img/adobe_illustrator/class8_homework_ellie_happyholoday.png" style="width:auto, height:500px" onclick="currentSlide(6)" alt="Happy Holidays">
    </div>
    <div class="column">
      <img class="demo cursor" src="/img/adobe_illustrator/Ellie_mooncake.png" style="width:auto, height:500px" onclick="currentSlide(1)" alt="Moon cake">
    </div>
    <div class="column">
      <img class="demo cursor" src="/img/adobe_illustrator/hungarian_door_Ellie.png" style="width:auto, height:500px" onclick="currentSlide(2)" alt="Hungarian door">
    </div>
    <div class="column">
      <img class="demo cursor" src="/img/adobe_illustrator/homework3_ellie.png" style="width:auto, height:500px" onclick="currentSlide(3)" alt="Llama in the farm">
    </div>
    <div class="column">
      <img class="demo cursor" src="/img/adobe_illustrator/Roger_william_zoo_Ellie.png" style="width:auto, height:500px" onclick="currentSlide(4)" alt="Roger william zoo map">
    </div>
    <div class="column">
      <img class="demo cursor" src="/img/adobe_illustrator/Ellie_menu.png" style="width:auto, height:500px" onclick="currentSlide(5)" alt="Pizza restaurant takeout menu">
    </div>    
    <div class="column">
    <img class="demo cursor" src="/img/adobe_illustrator/Asset_3.png" style="width:auto, height:500px" onclick="currentSlide(7)" alt="Happy Halloween!">
    </div>
     <div class="column">
      <img class="demo cursor" src="/img/adobe_illustrator/Asset_4.png" style="width:auto, height:500px" onclick="currentSlide(8)" alt="Spring birds">
    </div>
    <div class="column">
      <img class="demo cursor" src="/img/adobe_illustrator/Final_project_ellie.png" style="width:auto, height:500px" onclick="currentSlide(9)" alt="Texas Eyeball">
    </div>
  </div>
</div>


<script>
var slideIndex = 1;
showSlides(slideIndex);

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  var i;
  var slides = document.getElementsByClassName("mySlides");
  var dots = document.getElementsByClassName("demo");
  var captionText = document.getElementById("caption");
  if (n > slides.length) {slideIndex = 1}
  if (n < 1) {slideIndex = slides.length}
  for (i = 0; i < slides.length; i++) {
      slides[i].style.display = "none";
  }
  for (i = 0; i < dots.length; i++) {
      dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";
  dots[slideIndex-1].className += " active";
  captionText.innerHTML = dots[slideIndex-1].alt;
}
</script>

</body>
