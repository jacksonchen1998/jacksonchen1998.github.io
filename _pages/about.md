---
permalink: /
title: ""
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
<div>

<!-- <a href="https://hackmd.io/GbY28RBLQQWtuam7axGfGg" title="Optional Title">CGU CS Course & some tools</a><br><br> -->

<div class="homepage">
 <p class="map-title">My Website</p>
 <p> Life is like a long marathon, with every step building upon the last.  </p>
 <p> No matter how difficult the path may be, we hope to rely on unwavering faith and effort to eventually reach the ideal destination. </p>
 <p> Through continuous self-improvement, we aspire to create a life that truly belongs to us. </p>
</div>

<div class="github">
  <p class="map-title">My Github</p>
  <div class="center">
  <a href="https://github.com/jacksonchen1998">
      <img class="img-fluid" src="https://github-readme-stats.vercel.app/api/?username=jacksonchen1998&theme=default&show_icons=true" alt="jacksonchen1998">
    </a>
</div>

<div class="row">
    <div class="column">
    <a href="https://github.com/jacksonchen1998/Awesome-CGU-CS-AI">
      <img class="img-fluid" src="https://github-readme-stats.vercel.app/api/pin/?username=jacksonchen1998&repo=Awesome-CGU-CS-AI&theme=default&show_owner=false" alt="awesome">
    </a>
  </div>
    <div class="column">
    <a href="https://github.com/jacksonchen1998/Empowering-NLG">
      <img class="img-fluid" src="https://github-readme-stats.vercel.app/api/pin/?username=jacksonchen1998&repo=Empowering-NLG&theme=default&show_owner=false" alt="awesome">
    </a>
</div>
      <div class="column">
    <a href="https://github.com/jacksonchen1998/Multi-turn-Dialogue-Response">
      <img class="img-fluid" src="https://github-readme-stats.vercel.app/api/pin/?username=jacksonchen1998&repo=Multi-turn-Dialogue-Response&theme=default&show_owner=false" alt="awesome">
    </a>
  </div>
  <div class="column">
    <a href="https://github.com/jacksonchen1998/LLaMA-Paper-List">
      <img class="img-fluid" src="https://github-readme-stats.vercel.app/api/pin/?username=jacksonchen1998&repo=LLaMA-Paper-List&theme=default&show_owner=false" alt="awesome">
    </a>
  </div>
</div>

<br><br><br><br><br><br>

<div class="map">
  <p class="map-title">My Personal Map</p>
  <iframe src="https://www.google.com/maps/d/u/0/embed?mid=11uEqrUqviLk2cDmxT0INWQeQCyVYESs&ehbc=2E312F" width="100%" height="480"></iframe>
</div>


<br><br>
</div>

<style>
* {box-sizing: border-box}
body {font-family: Verdana, sans-serif; margin:0}
.mySlides {display: none}
img {vertical-align: middle;}

/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
}

.bold {
  font-weight: bold;
  font-size: 20px;
}

/* Next & previous buttons */
.prev, .next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  padding: 16px;
  margin-top: -22px;
  color: white;
  font-weight: bold;
  font-size: 18px;
  transition: 0.6s ease;
  border-radius: 0 3px 3px 0;
  user-select: none;
}

.github{
  margin-down: 50px;
}

.map {
  margin-top: 150px;
}

.map-title {
  background-color: #2E312F;
  color: white;
  padding: 16px;
  text-align: center;
  font-size: 20px;
  font-family: "Lucida Console", Courier, monospace;
}

/* Position the "next button" to the right */
.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}

/* On hover, add a black background color with a little bit see-through */
.prev:hover, .next:hover {
  background-color: rgba(0,0,0,0.8);
}

/* Caption text */
.text {
  color: #f2f2f2;
  font-size: 15px;
  padding: 8px 12px;
  position: absolute;
  bottom: 8px;
  width: 100%;
  text-align: center;
}

/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}

/* The dots/bullets/indicators */
.dot {
  cursor: pointer;
  height: 15px;
  width: 15px;
  margin: 0 2px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}

.active, .dot:hover {
  background-color: #717171;
}

/* Fading animation */
.fade {
  animation-name: fade;
  animation-duration: 1.5s;
}

@keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

/* On smaller screens, decrease text size */
@media only screen and (max-width: 300px) {
  .prev, .next,.text {font-size: 11px}
}

.column {
  float: left;
  width: 50%;
  padding: 10px;
}

.center {
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: 50%;
}

.img-fluid {
  width: 100%;
  height: auto;
}
</style>

<body>

<div class="slideshow-container">

<div class="mySlides fade">
  <div class="numbertext">1 / 3</div>
  <img src="/images/scence.png" style="width:100%">
  <div class="text">Flying to the unknown</div>
</div>

<div class="mySlides fade">
  <div class="numbertext">2 / 3</div>
  <img src="/images/scence2.png" style="width:100%">
  <div class="text">Australian Beach</div>
</div>

<div class="mySlides fade">
  <div class="numbertext">3 / 3</div>
  <img src="/images/scence3.png" style="width:100%">
  <div class="text">Street View of Central Park, New York</div>
</div>

<a class="prev" onclick="plusSlides(-1)">❮</a>
<a class="next" onclick="plusSlides(1)">❯</a>

</div>
<br>

<div style="text-align:center">
  <span class="dot" onclick="currentSlide(1)"></span> 
  <span class="dot" onclick="currentSlide(2)"></span> 
  <span class="dot" onclick="currentSlide(3)"></span> 
</div>

<script>
let slideIndex = 1;
showSlides(slideIndex);

function plusSlides(n) {
  showSlides(slideIndex += n);
}

function currentSlide(n) {
  showSlides(slideIndex = n);
}

function showSlides(n) {
  let i;
  let slides = document.getElementsByClassName("mySlides");
  let dots = document.getElementsByClassName("dot");
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
}
</script>