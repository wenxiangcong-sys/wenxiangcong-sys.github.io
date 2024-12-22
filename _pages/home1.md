---
title: "Intellimaging Tech - Home"
layout: homelay
excerpt: "Developing artificial intelligence technologies for medical imaging"
sitemap: false
permalink: /
---

<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {box-sizing: border-box;}
body {font-family: Verdana, sans-serif;}
.mySlides {display: none;}
img {vertical-align: middle;}

/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
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
  height: 15px;
  width: 15px;
  margin: 0 2px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}

.active {
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
  .text {font-size: 11px}
}
</style>
</head>
<body>

<h2>Automatic Slideshow</h2>
<p>Change image every 2 seconds:</p>

<div class="slideshow-container">

<div class="mySlides fade">
  <div class="numbertext">1 / 3</div>
  <img src="img_nature_wide.jpg" style="width:100%">
  <div class="text">Caption Text</div>
</div>

<div class="mySlides fade">
  <div class="numbertext">2 / 3</div>
  <img src="img_snow_wide.jpg" style="width:100%">
  <div class="text">Caption Two</div>
</div>

<div class="mySlides fade">
  <div class="numbertext">3 / 3</div>
  <img src="img_mountains_wide.jpg" style="width:100%">
  <div class="text">Caption Three</div>
</div>

</div>
<br>

<div style="text-align:center">
  <span class="dot"></span> 
  <span class="dot"></span> 
  <span class="dot"></span> 
</div>

<script>
let slideIndex = 0;
showSlides();

function showSlides() {
  let i;
  let slides = document.getElementsByClassName("mySlides");
  let dots = document.getElementsByClassName("dot");
  for (i = 0; i < slides.length; i++) {
    slides[i].style.display = "none";  
  }
  slideIndex++;
  if (slideIndex > slides.length) {slideIndex = 1}    
  for (i = 0; i < dots.length; i++) {
    dots[i].className = dots[i].className.replace(" active", "");
  }
  slides[slideIndex-1].style.display = "block";  
  dots[slideIndex-1].className += " active";
  setTimeout(showSlides, 2000); // Change image every 2 seconds
}
</script>

</body>
</html> 



<p style="text-align: justify;">We have proposed a novel score-matching formula to derive a new score function through deep learning on an image dataset. By integrating our new score function into the image reconstruction process, we have developed a new iterative reconstruction method within the MAP estimation framework to enhance image quality. We have evaluated the performance of our image reconstruction method on both public medical CT datasets and clinical raw datasets. Our reconstruction method consistently produced higher quality images in terms of PSNR and SSIM metrics across diverse datasets. Notably, on Siemens and GE clinical CT raw datasets, our proposed approach achieved superior denoising and deblurring effects over the competing methods, illustrating remarkable generalizability and stability. Our proposed score matching formula holds potential in image denoising, deblurring, and generation.</p>   

<p style="text-align: justify;">Our focus is on medical imaging, with an emphasis on X-ray tomographic imaging, photoacoustic imaging, and image reconstruction and analysis. We are developing theories, methods, software, and hardware systems for clinical applications. We are excited to collaborate with partners and funding agencies on innovative and impactful projects, especially [National Institutes of Health](https://www.nih.gov/).</p>


<div markdown="0" id="carousel" class="carousel slide" data-ride="carousel" data-interval="2500" data-pause="hover" >
    <!-- Menu -->
    <ol class="carousel-indicators">
        <li data-target="#carousel" data-slide-to="0" class="active"></li>
        <li data-target="#carousel" data-slide-to="1"></li>
        <li data-target="#carousel" data-slide-to="2"></li>
        <li data-target="#carousel" data-slide-to="3"></li>
    </ol>

  <!--
  <a class="left carousel-control" role="button" data-slide="prev">
    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" role="button" data-slide="next">
    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
  -->

  <!--
  <a class="left carousel-control" role="button" data-slide="prev" onclick="moveCarousel('prev')">
    <span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </a>
  <a class="right carousel-control" role="button" data-slide="next" onclick="moveCarousel('next')">
    <span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </a>
  -->

    <!-- Items -->
    <div class="carousel-inner" markdown="0">
        
        <div class="item active">
            <a href="https://www.cell.com/patterns/fulltext/S2666-3899(20)30169-0">
              <img src="{{ site.url }}{{ site.baseurl }}/images/home0.PNG" alt="Slide 1" width="800" height="600"/>
            </a>
        </div>

        <!-- Second Slide -->
        <div class="item">
            <a href="https://arxiv.org/pdf/2306.08610v7">
                <img src="{{ site.url }}{{ site.baseurl }}/images/Slide1.PNG" alt="Slide 2" width="800" height="600"/>
            </a>
        </div>

        <!-- Third Slide -->
        <div class="item">
            <a href="https://arxiv.org/pdf/2306.08610v7">
                <img src="{{ site.url }}{{ site.baseurl }}/images/Slide2.PNG" alt="Slide 3" width="800" height="600"/>
            </a>
        </div>

        <!-- Fourth Slide -->
        <div class="item">
            <a href="https://www.cell.com/patterns/fulltext/S2666-3899(20)30169-0">
                <img src="{{ site.url }}{{ site.baseurl }}/images/Slide3.png" alt="Slide 4" width="800" height="600"/>
            </a>
        </div>
  </div>

</div>

<!-- jQuery (necessary for Bootstrap's JavaScript plugins) -->
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.12.4/jquery.min.js"></script>
<!-- Include all compiled plugins (below), or include individual files as needed -->
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js"></script>


