# HappyBDayMom
Just a quick program for my mom's birthday

Cool

<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8">
        <title>Happy Birthday Mom!</title>
        
<link href="https://fonts.googleapis.com/css?family=Anton|Lobster|Pacifico&display=swap" rel="stylesheet">

    
    
<style>
            body {
                font-family: "Pacifico", sans-serif;
                text-align: center;
                text-shadow: 2px 3px black;
                font-size: 32px;
            }
            .banner {
                margin: 0px;
                padding: 31px;
                background-color: rgb(87, 191, 34);
                color: white;
            }
            p {
                font-family: Arial;
            }
            footer {
                padding: 30px;
                background-color: rgb(27, 189, 27);
                color: white;
            }
            a {
                text-decoration: underline;
                color: blue;
            }
            .action-button {
                background:rgb(255, 0, 0);
                display:inline-block;
                width:130px;
                margin:10px;
                padding:10px;
                text-align:center;
                text-decoration:none;
            }
            .action-button:hover {
                background:rgb(42, 112, 25);
                transition:0.3s;
                color:white;
                cursor:pointer;
            }
            span {
                color: rgb(214, 197, 214);
            }
            li {
                text-align: center;
            }
            * {box-sizing: border-box}
body {font-family: Pacifico, sans-serif; margin:0}
.mySlides {display: none}
img {vertical-align: middle;}
margin-top {
    10px;
}

/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
  margin-top: 10px;
}

/* Next & previous buttons */
.prev, .next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  padding: 16px;
  margin-top: -22px;
  color: black;
  font-weight: bold;
  font-size: 18px;
  transition: 0.6s ease;
  border-radius: 0 3px 3px 0;
  user-select: none;
}
.prev {
    left: 30px;
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
    font-family: "Anton", sans-serif;
  color: black;
  font-size: 15px;
  padding: 8px 12px;
  position: absolute;
  bottom: 8px;
  width: 100%;
  text-align: center;
  text-shadow: none;
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
  -webkit-animation-name: fade;
  -webkit-animation-duration: 1.5s;
  animation-name: fade;
  animation-duration: 1.5s;
}

@-webkit-keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

@keyframes fade {
  from {opacity: .4} 
  to {opacity: 1}
}

/* On smaller screens, decrease text size */
@media only screen and (max-width: 300px) {
  .prev, .next,.text {font-size: 11px}
}
.msg {
    font-family: "Lobster", sans-serif;
    font-size: 30px;
    color: white;
    background-color: red;
    border-radius: 5px;
    margin: 75px;
}
        </style>
        </head>
        <body>
        <div class="banner">
          <h1>Happy Birthday Mom!</h1>
          
          </div>
          <div class="slideshow-container">

<div class="mySlides fade">
  <div class="numbertext">1 / 3</div>
  <img src="https://www.happybirthdaymsg.com/wp-content/uploads/2016/03/Happy-Birthdaymom.-Frame-of-flowers-and-hearts..jpg" style="width:100%">
  <div class="text">Happy Birthday!</div>
</div>

<div class="mySlides fade">
  <div class="numbertext">2 / 3</div>
  <img src="https://image.tfgmedia.co.za/image/1/process/486x486?source=http://cdn.tfgmedia.co.za/15/ProductImages/201032.jpg" style="width:100%">
  <div class="text">Love You!</div>
</div>

<div class="mySlides fade">
  <div class="numbertext">3 / 3</div>
  <img src="https://www.hoopoequotes.com/media/k2/items/cache/0bd9408b3575b2a1e58036ba9ed75f5c_XL.jpg" style="width:100%">
  <div class="text">Have a great day!</div>
</div>

<a class="prev" onclick="plusSlides(-1)">&#10094;</a>
<a class="next" onclick="plusSlides(1)">&#10095;</a>

</div>
<br>

<div style="text-align:center">
  <span class="dot" onclick="currentSlide(1)"></span> 
  <span class="dot" onclick="currentSlide(2)"></span> 
  <span class="dot" onclick="currentSlide(3)"></span> 
</div>
<div class="msg">
<p class="msg">Have a wonderful birthday Mom! We love you so much! <br>Bryce</p>
</div>


          <footer>
             &copy; Bryce S. 2019  
          </footer>
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
  var dots = document.getElementsByClassName("dot");
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
    </body>
</html>
