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
 <p class="map-title">Website</p>
 <a href="https://youtu.be/_YYmfM2TfUA?feature=shared" target="_blank">
    <img src="/images/rocky.gif" style="width:100%">
</a>
 <div>
 <br>
 <p> Life is like a long marathon, with every step building upon the last.  </p>
 <p> No matter how difficult the path may be, we hope to rely on unwavering faith and effort to eventually reach the ideal destination. </p>
 <p> Through continuous self-improvement, we aspire to create a life that truly belongs to us. </p>
 </div>
</div>

<div class="map">
  <p class="map-title">Personal Map</p>
  <iframe src="https://www.google.com/maps/d/u/0/embed?mid=11uEqrUqviLk2cDmxT0INWQeQCyVYESs&ehbc=2E312F" width="100%" height="480"></iframe>
</div>


<br><br>

<style>
* {box-sizing: border-box}
body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
  margin: 0;
  color: #333;
  line-height: 1.6;
}
.mySlides {display: none}
img {vertical-align: middle;}

/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: 40px auto;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 10px 25px rgba(0,0,0,0.1);
}

/* Next & previous buttons */
.prev, .next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: 40px;
  height: 40px;
  margin-top: -20px;
  color: white;
  font-weight: bold;
  font-size: 18px;
  transition: 0.3s ease;
  border-radius: 50%;
  background-color: rgba(0,0,0,0.3);
  display: flex;
  align-items: center;
  justify-content: center;
  user-select: none;
  text-decoration: none;
}

.next {
  right: 15px;
}

.prev {
  left: 15px;
}

/* On hover, add a black background color with a little bit see-through */
.prev:hover, .next:hover {
  background-color: rgba(0,0,0,0.9);
}

/* Caption text */
.text {
  color: #fff;
  font-size: 16px;
  padding: 15px;
  position: absolute;
  bottom: 0;
  width: 100%;
  text-align: center;
  background: linear-gradient(to top, rgba(0,0,0,0.8), transparent);
  text-shadow: 0 1px 2px rgba(0,0,0,0.8);
}

/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
  background: rgba(0,0,0,0.3);
  border-bottom-right-radius: 8px;
}

/* The dots/bullets/indicators */
.dot {
  cursor: pointer;
  height: 12px;
  width: 12px;
  margin: 0 4px;
  background-color: #ddd;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.3s ease, transform 0.3s ease;
}

.active, .dot:hover {
  background-color: #2E312F;
  transform: scale(1.2);
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

/* Section Styling */
.homepage, .map {
  background: #fff;
  border-radius: 12px;
  box-shadow: 0 10px 25px rgba(0,0,0,0.05);
  overflow: hidden;
  margin-bottom: 40px;
  border: 1px solid #eee;
}

.map {
  margin-top: 40px;
}

.map-title {
  background-color: #2E312F;
  color: white;
  padding: 15px;
  text-align: center;
  font-size: 1.2rem;
  font-weight: 600;
  letter-spacing: 1px;
  margin: 0;
  text-transform: uppercase;
}

.homepage div {
  padding: 20px;
  text-align: center;
}

.homepage div p {
  margin-bottom: 10px;
  color: #555;
}

.homepage img {
  display: block;
  width: 100%;
  height: auto;
  transition: transform 0.3s ease;
}

.homepage a:hover img {
  transform: scale(1.02);
}

/* The Modal (background) */
.modal {
  display: none; 
  position: fixed; 
  z-index: 9999; 
  left: 0;
  top: 0;
  width: 100%; 
  height: 100%; 
  overflow: auto; 
  background-color: rgba(0,0,0,0.6); 
  backdrop-filter: blur(10px);
  align-items: center;
  justify-content: center;
}

/* Modal Content (image) */
.modal-content {
  margin: auto;
  display: block;
  width: auto;
  max-width: 90%;
  max-height: 90vh;
  object-fit: contain;
  border-radius: 8px;
  box-shadow: 0 0 20px rgba(255,255,255,0.1);
  animation-name: zoom;
  animation-duration: 0.6s;
}

@keyframes zoom {
  from {transform:scale(0)} 
  to {transform:scale(1)}
}

/* The Close Button */
.close {
  position: absolute;
  top: 20px;
  right: 35px;
  color: #f1f1f1;
  font-size: 40px;
  font-weight: bold;
  transition: 0.3s;
  z-index: 10000;
}

.close:hover,
.close:focus {
  color: #bbb;
  text-decoration: none;
  cursor: pointer;
}
</style>

<body>

<div class="slideshow-container">

{% assign slide_images = site.static_files | where_exp: "item", "item.path contains '/images/slide/'" %}
{% for image in slide_images %}
<div class="mySlides fade">
  <div class="numbertext">{{ forloop.index }} / {{ slide_images.size }}</div>
  <img src="{{ image.path }}" style="width:100%" onclick="openModal(this)">
  <div class="text"></div>
</div>
{% endfor %}

<a class="prev" onclick="plusSlides(-1)">❮</a>
<a class="next" onclick="plusSlides(1)">❯</a>

</div>
<br>

<div style="text-align:center">
{% for image in slide_images %}
  <span class="dot" onclick="currentSlide({{ forloop.index }})"></span>
{% endfor %}
</div>

<div id="myModal" class="modal">
  <span class="close" onclick="closeModal()">&times;</span>
  <img class="modal-content" id="img01">
</div>

<script>
let slideIndex = 1;
showSlides(slideIndex);

// Move modal to body to ensure it covers the entire screen
var modal = document.getElementById("myModal");
if (modal && modal.parentNode !== document.body) {
  document.body.appendChild(modal);
}

let slideInterval = setInterval(function() { plusSlides(1); }, 3000);

function plusSlides(n) {
  clearInterval(slideInterval);
  showSlides(slideIndex += n);
  slideInterval = setInterval(function() { plusSlides(1); }, 3000);
}

function currentSlide(n) {
  clearInterval(slideInterval);
  showSlides(slideIndex = n);
  slideInterval = setInterval(function() { plusSlides(1); }, 3000);
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

function openModal(element) {
  document.getElementById("myModal").style.display = "flex";
  document.getElementById("img01").src = element.src;
}

function closeModal() {
  document.getElementById("myModal").style.display = "none";
}

// When the user clicks on the modal background (not the image), close it.
document.getElementById('myModal').addEventListener('click', function(event) {
  if (event.target === this) {
    closeModal();
  }
});
</script>