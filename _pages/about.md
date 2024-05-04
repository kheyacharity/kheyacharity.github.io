---
layout: about
title: Home
permalink: /
subtitle: 

profile:
  align: center
  image: 
  image_circular: false # crops the image to make it circular
  more_info: >
    

news: false # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page

images:
  compare: true
  slider: true
---


<swiper-container keyboard="true" navigation="true" pagination="true" pagination-clickable="true" pagination-dynamic-bullets="true" rewind="true">
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/kheya0.jpg" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/kheya1.jpg" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/kheya2.jpg" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/kheya3.jpg" class="img-fluid rounded z-depth-1" %}</swiper-slide>
</swiper-container>


## খেয়া – উত্তরণের নিশ্চিত ঠিকানা

একটি স্বেচ্ছাসেবী উদ্যোগ।।

রবিঠাকুর, বিবেকানন্দ, নজরুল, ক্ষুদিরাম, নেতাজী, সুকান্ত থেকে শক্তি-সুনীল আমরা সকলেই কমবেশি ভালোবাসি, পছন্দও করি। স্কুলে বিবেকানন্দ, টেরেজার ছবিও তো আমরা কম কিছু লাগাইনি দেওয়াল জুড়ে, কিন্তু তাতে দেওয়ালের রূপ হয়তো ফিরেছে, কিন্তু মানবজীবনের?? মানবজীবনের কোনো রূপ কি আদৌ ফিরেছে??
হয়তো ফেরেনি, না সত্যিই ফেরেনি।। শুধু দেওয়ালে ছবি লাগালেই হয় না যে, ছবির ভিতরের মানুষের জীবনদর্শনটাকে নিজের মনের দেওয়ালেও যে লেপে নিতে হয়, তাই না??
সেই মনের দেওয়ালেই দর্শন বোধকে বাঁচিয়ে রাখতে ক্ষয়িষ্ণু সমাজের বুকে স্রোতের বিপরীতে ভেসে যাওয়ার মানসিকতার একদল আত্মভোলা পাগলাঘোড়ার জীবনতরী হল আমাদের খেয়া – উত্তরণের নিশ্চিত ঠিকানা ।

আসুন, “সকলের তরে সকলে আমরা, প্রত্যেকে আমরা পরের তরে”র ভাবনায় একবার নিজেদের একবার মেপে দেখি।।

একবার ভেবে দেখি, পাশের বাড়ির অসুস্থ কাকুর ছেলেটার কথা, যখন কাকিমা কাকুর ওষুধের টাকা জোগাড় করতেই হিমসিক খাচ্ছে তখন রমেশের বই কেনার টাকা আসবে কোথা থেকে??

একবার ভেবে দেখি, আমার বোনের জ্বর হলে মা যে মধু টা তুলসিপাতার সাথে মিশিয়ে খেতে দেয়, সুন্দরবনের গভীর জঙ্গলে চাক ভেঙে সেই মধু তুলে আনতে গিয়ে যে লোকটা বাঘের মুখে, কুমিরের মুখে পড়ে প্রাণ হারায় তার পরিবারের পুজোটা কিভাবে কাটে ? সেই লোকটার ও যে একটা ফুটফুটে বাচ্চা ছেলে ছিল, তার পুজোয় একটাও নতুন জামাকাপড় হোলো কি না??

একবার ভেবে দেখি, বন্যায় যখন গ্রামের পর গ্রাম ভেসে গেলো, কাঁচা মাটির বাড়িগুলো যখন সব জলের তলায়, তখন অসহায় মানুষগুলো যখন টানা ১৩ দিন জলবন্দী অবস্থায় মানুষগুলো কি খেয়ে দিন কাটালো??



[//]: # (Animated counter)

<div class="card-container">
  <div class="card">
    <div class="animate-counter">0</div>
    <div class="text">Beneficiaries</div>
  </div>
  <div class="card">
    <div class="animate-counter">0</div>
    <div class="text">Districts Covered</div>
  </div>
</div>

<style>
  .card-container {
    display: flex;
    justify-content: space-between; /* Adjust as needed */
  }

  .card {
    flex: 1;
    margin: 0 10px; /* Adjust margin between cards as needed */
    padding: 20px;
    background-color: #809185;
    border-radius: 50px; /* Adjust this value to control the roundness */
    text-align: center;
  }
</style>

<script>
  const targetElements = document.querySelectorAll('.animate-counter');
  const startValues = [0, 0];
  const endValues = [10000, 10] // Set your desired end values
  const animationDuration = 3000; // Animation duration in milliseconds (adjust as needed)

  const options = {
    threshold: 0.5, // Trigger animation when 50% of the element is visible
  };

  const animateCounters = (entries) => {
    entries.forEach((entry, index) => {
      if (entry.isIntersecting) {
        let currentValue = startValues[index];
        const totalSteps = 100; // Total steps for the animation
        const increment = Math.ceil((endValues[index] - currentValue) / totalSteps); // Adjust increment as needed

        const updateCounter = () => {
          if (currentValue <= endValues[index]) {
            targetElements[index].textContent = currentValue;
            currentValue += increment;
            if (currentValue <= endValues[index]) {
              requestAnimationFrame(updateCounter);
            }
          }
        };

        const startTime = performance.now(); // Get start time
        const update = (currentTime) => {
          const elapsedTime = currentTime - startTime;
          const progress = Math.min(elapsedTime / animationDuration, 1); // Ensure progress doesn't exceed 1
          currentValue = Math.floor(startValues[index] + progress * (endValues[index] - startValues[index]));
          targetElements[index].textContent = currentValue;
          if (progress < 1) {
            requestAnimationFrame(update);
          }
        };

        requestAnimationFrame(update); // Start animation
      }
    });
  };

  const observer = new IntersectionObserver(animateCounters, options);
  targetElements.forEach((element) => {
    observer.observe(element);
  });
</script>

<br/><br/>

[//]: # (Promo Video)



<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; border-radius: 10px;">
    <iframe style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border-radius: 10px;" src="https://www.youtube.com/embed/OmXC3aPr5yg?si=xc2KVgbMNv8UTcC9" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>

<div class="caption" style="border-radius: 10px; background-color: #809185; padding: 10px; margin-top: 10px;">
    Kheya Charity Promo
</div>






# <center>Get in touch with Kheya</center>


[//]: # (Contact Form)

<div id="formkeep-embed" data-formkeep-url="https://formkeep.com/p/cad66ed6943799217508285a3673695f?embedded=1"></div>

<script type="text/javascript" src="https://pym.nprapps.org/pym.v1.min.js"></script>
<script type="text/javascript" src="https://formkeep-production-herokuapp-com.global.ssl.fastly.net/formkeep-embed.js"></script>

<!-- Get notified when the form is submitted, add your own code below: -->
<script>
const formkeepEmbed = document.querySelector('#formkeep-embed')

formkeepEmbed.addEventListener('formkeep-embed:submitting', _event => {
  console.log('Submitting form...')
})

formkeepEmbed.addEventListener('formkeep-embed:submitted', _event => {
  console.log('Submitted form...')
})
</script>