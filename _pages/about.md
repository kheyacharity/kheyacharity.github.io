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
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/kheya01.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/kheya00.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/kheya02.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/kheya03.png" class="img-fluid rounded z-depth-1" %}</swiper-slide>
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

<div class="counter-container">
  <div class="counter">
    <div class="animate-counter" data-end-value="10000">0</div>
    <div class="text">Beneficiaries</div>
  </div>
  <div class="counter">
    <div class="animate-counter" data-end-value="10">0</div>
    <div class="text">Districts Covered</div>
  </div>
</div>

<style>
  /* Style for counter container */
  .counter-container {
    display: flex;
    justify-content: center;
    gap: 20px;
  }

  /* Style for counter card */
  .counter {
    width: 475px;
    padding: 20px;
    background-color: #f4f4f4;
    border-radius: 10px;
    text-align: center;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* Add shadow */
    transition: transform 0.3s ease-in-out;
  }

  /* Hover effect for counter card */
  .counter:hover {
    transform: translateY(-5px);
  }

  /* Style for animated number */
  .animate-counter {
    font-size: 36px;
    font-weight: bold;
    color: #007bff; /* Adjust color as needed */
  }

  /* Style for counter text */
  .text {
    margin-top: 10px;
    font-size: 18px;
    color: #333; /* Adjust color as needed */
  }
</style>

<script>
  const targetElements = document.querySelectorAll('.animate-counter');

  const animateCounters = (entries) => {
    entries.forEach((entry, index) => {
      if (entry.isIntersecting) {
        const endValue = parseInt(targetElements[index].getAttribute('data-end-value'));
        let startValue = 0;
        const totalSteps = 100; // Total steps for the animation
        const increment = Math.ceil(endValue / totalSteps); // Calculate increment based on end value

        const updateCounter = () => {
          if (startValue <= endValue) {
            const displayedValue = startValue >= 1000 ? startValue.toLocaleString() : startValue;
            targetElements[index].textContent = `${displayedValue}+`;
            startValue += increment;
            if (startValue <= endValue) {
              requestAnimationFrame(updateCounter);
            }
          }
        };

        requestAnimationFrame(updateCounter); // Start animation
      }
    });
  };

  const observer = new IntersectionObserver(animateCounters, { threshold: 0.5 });
  targetElements.forEach((element) => {
    observer.observe(element);
  });
</script>



<br/><br/>



[//]: # (Promo Video)



<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; border-radius: 10px;">
    <iframe style="position: absolute; top: 0; left: 0; width: 100%; height: 100%; border-radius: 10px;" src="https://www.youtube.com/embed/OmXC3aPr5yg?si=xc2KVgbMNv8UTcC9" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
</div>

<br/><br/>






# <center>Get in touch with Kheya</center>


[//]: # (Contact Form)

<div class="form-container">
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
</div>

<style>
  /* Style for form container */
  .form-container {
    border: 2px solid #ddd; /* Border color */
    border-radius: 10px; /* Border radius */
    padding: 20px;
    max-width: 500px; /* Adjust width as needed */
    margin: 0 auto; /* Center the container */
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* Add shadow */
  }
</style>
