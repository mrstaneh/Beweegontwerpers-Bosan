<script>
	import { onMount } from 'svelte';

  let slideIndex = 1;

  export let photos = undefined;
  export let id = undefined;
  export let maxwidth = 1000;

  function showSlides(n) {
      var i;
      var slides = document.getElementsByClassName(`mySlides-${id}`);
      var dots = document.getElementsByClassName(`dot-${id}`);
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

  // Next/previous controls
  function plusSlides(n) {
      showSlides(slideIndex += n);
  }

  // Thumbnail image controls
  function currentSlide(n) {
      showSlides(slideIndex = n);
  }

  onMount(async () => {
      showSlides(slideIndex);
  });
</script>

<!-- Slideshow container -->
<div class="slideshow-container-{id} slideshow-container" style="max-width: {maxwidth}px;">
    <!-- Full-width images with number and caption text -->
    {#each photos as photo, i}
      <div class="mySlides-{id} mySlides fade">
        <div class="numbertext">{i + 1} / {photos.length}</div>
        <img src="{photo.path}" alt="{photo.alt}" style="width:100%">
      </div>
    {/each}

    <!-- Next and previous buttons -->
    <!-- svelte-ignore a11y-missing-attribute -->
    <a class="prev" on:click={() => {plusSlides(-1)}}><i class="arrow fa-solid fa-angle-left"></i></a>
    <!-- svelte-ignore a11y-missing-attribute -->
    <a class="next" on:click={() => {plusSlides(1)}}><i class="arrow fa-solid fa-angle-right"></i></a>
</div>

<br>
  
<!-- The dots/circles -->
<div style="text-align:center; margin-bottom: 1rem;">
  {#each photos as photo, i}
    <span class="dot-{id} dot" on:click={() => {currentSlide(i + 1)}}></span>
  {/each}
</div>

<style>
    * {box-sizing:border-box}

/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
}

.arrow{
    font-size: 24px;
}

/* Hide the images by default */
.mySlides {
  display: none;
}

/* Next & previous buttons */
.prev, .next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  margin-top: -22px;
  padding: 16px;
  color: white;
  font-weight: bold;
  font-size: 18px;
  transition: 0.6s ease;
  border-radius: 0 3px 3px 0;
  user-select: none;
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
</style>