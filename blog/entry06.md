# Entry 6
5/10/25
## Context
It's been a busy few weeks since I started building my website, and I'm finally wrapping up the project. My goal was to create a smooth, responsive layout using Bootstrap and A-Frame for interactive elements. Here's an overview of the key milestones, challenges, and solutions I encountered during this process.

# Code
#### 4/24–4/25: Set up Bootstrap, build Desktop layout (Navbar, Hero Section, Footer). Use placeholders.

```html
<<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Freedom Project</title>

  <!-- Bootstrap -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" />
  <!-- Bootstrap Icons -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons/font/bootstrap-icons.css" rel="stylesheet" />
  <!-- A-Frame -->
  <script src="https://aframe.io/releases/1.4.2/aframe.min.js"></script>
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Bruno+Ace+SC&display=swap" rel="stylesheet" />
  <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@300..700&display=swap" rel="stylesheet" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Bruno+Ace+SC&family=Fira+Code:wght@300..700&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&family=Space+Grotesk:wght@300..700&display=swap" rel="stylesheet">
<!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-light bg-light shadow-sm">
    <div class="container">
      <a class="navbar-brand" href="#">Cooking</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link" href="#">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="#test">About</a></li>
          <li class="nav-item"><a class="nav-link" href="#test2">Content</a></li>
          <li class="nav-item"><a class="nav-link" href="#test3">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Hero Section -->
  <section class="hero p-0">
    <div id="heroCarousel" class="carousel slide" data-bs-ride="carousel" data-bs-interval="3000">
      <div class="carousel-indicators">
        <button type="button" data-bs-target="#heroCarousel" data-bs-slide-to="0" class="active"></button>
        <button type="button" data-bs-target="#heroCarousel" data-bs-slide-to="1"></button>
        <button type="button" data-bs-target="#heroCarousel" data-bs-slide-to="2"></button>
      </div>

      <div class="carousel-inner">
        <div class="carousel-item active">
          <div class="d-flex align-items-center justify-content-center bg-success-subtle">
            <img src="../Photo/chef.jpg" class="d-block w-75" alt="Chef preparing food">
            <h2>Scientific Breakthroughs</h2>
          </div>
        </div>
        <div class="carousel-item">
          <div class="d-flex align-items-center justify-content-center bg-primary-subtle">
            <h2>Cooking Technologies</h2>
            <img src="../Photo/food.jpg" class="d-block w-75" alt="Modern food tech">
          </div>
        </div>
        <div class="carousel-item">
          <div class="d-flex align-items-center justify-content-center bg-warning-subtle">
            <img src="../Photo/rice.jpeg" class="d-block w-75" alt="Sustainable rice farming">
            <h2>Innovative Ideas</h2>
          </div>
        </div>
      </div>

      <button class="carousel-control-prev" type="button" data-bs-target="#heroCarousel" data-bs-slide="prev">
        <span class="carousel-control-prev-icon"></span>
      </button>
      <button class="carousel-control-next" type="button" data-bs-target="#heroCarousel" data-bs-slide="next">
        <span class="carousel-control-next-icon"></span>
      </button>
    </div>
  </section>
  <section class="py-5">
    <div class="container" id="test">
      <div class="card-style text-center">
        <h3>Content</h3>
        <p>This project explores innovative food technologies that can transform how we cook, eat, and sustain ourselves. From 3D-printed meals to molecular recombination, these tools aim to solve real-world problems such as hunger, food waste, and accessibility—paving the way for a smarter, more sustainable future in the kitchen.</p>
      </div>
    </div>
  </section>
```
<p>During these two days, I focused on setting up the core structure of my website using Bootstrap. I created a basic layout with a navigation bar, a hero section, and a footer. Placeholders were used for images, and I set up some simple Bootstrap classes to get the design rolling.</p>

#### 4/26–4/27: Add most content: text blocks, buttons, placeholder images.

html

```html
<!--accordion-->
<div class="accordion" id="accordion">
  <section class="py-5">
    <div class="container" id="test2">
      <div class="row text-center">

        <!-- Recombinator Card with Accordion on the right -->
        <div class="col-12 col-md-6 d-flex align-items-center">
          <img src="./photo/wasten.png" alt="Recombinator" class="card-img">
        </div>
        <div class="col-12 col-md-6">
          <div class="card-style">
            <h4><i class="bi bi-heart-fill me-2"></i>Recombinator</h4>
            <p>I came up with an item for people who are poor and need nutritious food. The Recombinator is a machine that uses food waste and turns it into a full meal. Using advanced 3D food printing technology, we are able to mix various ingredients to create meals tailored to nutritional needs. This solution not only addresses food scarcity but also reduces waste and makes food more accessible for everyone.</p>
            <!-- Accordion for Recombinator -->
            <div class="accordion" id="accordion1">
              <div class="accordion-item">
                <h2 class="accordion-header" id="headingOne">
                  <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
                    More Details
                  </button>
                </h2>
                <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne" data-bs-parent="#accordion1">
                  <div class="accordion-body">
                    More detailed information about Recombinator will go here.
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- Printer Cooking Station Card with Accordion on the right -->
        <div class="col-12 col-md-6 d-flex align-items-center">
          <img src="./photo/Printer.png" alt="Printer Cooking Station" class="card-img">
        </div>
        <div class="col-12 col-md-6">
          <div class="card-style">
            <h4><i class="bi bi-cup-fill me-2"></i>Printer Cooking Station</h4>
            <p>What if you were stuck in the middle of nowhere, too lazy to cook anything, or just didn't have the time? The Printer Cooking Station is here to solve that problem. This machine uses 3D printing to prepare meals quickly and efficiently. With just a few ingredients and a simple recipe, you can have a freshly made meal printed in front of you. It's fast, customizable, and designed for modern living.</p>
            <!-- Accordion for Printer Cooking Station -->
            <div class="accordion" id="accordion2">
              <div class="accordion-item">
                <h2 class="accordion-header" id="headingTwo">
                  <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="true" aria-controls="collapseTwo">
                    More Details
                  </button>
                </h2>
                <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo" data-bs-parent="#accordion2">
                  <div class="accordion-body">
                    More detailed information about Printer Cooking Station.
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- Digital Item Website Card with Accordion on the right -->
        <div class="col-12 col-md-6 d-flex align-items-center">
          <img src="./photo/Shop.png" alt="Digital Item Website" class="card-img">
        </div>
        <div class="col-12 col-md-6">
          <div class="card-style">
            <h4><i class="bi bi-cart-fill me-2"></i>Digital Item Website</h4>
            <p>Want any item that appears to you without waiting for shipping? Our Digital Item Website has the solution. Whether it's a recipe, a cooking tool, or even a virtual product, we have the infrastructure to create and deliver digital items instantly. This innovative platform uses digital printing and technology to provide you with customized items on demand, all within minutes. No more waiting, just order and receive your digital item.</p>
            <!-- Accordion for Digital Item Website -->
            <div class="accordion" id="accordion3">
              <div class="accordion-item">
                <h2 class="accordion-header" id="headingThree">
                  <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="true" aria-controls="collapseThree">
                    More Details
                  </button>
                </h2>
                <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree" data-bs-parent="#accordion3">
                  <div class="accordion-body">
                    More details about the Digital Item Website.
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- Need Cut Card with Accordion on the right -->
        <div class="col-12 col-md-6 d-flex align-items-center">
          <img src="./photo/katanan.png" alt="Need Cut" class="card-img">
        </div>
        <div class="col-12 col-md-6">
          <div class="card-style">
            <h4><i class="bi bi-cart-fill me-2"></i>Need Cut</h4>
            <p>Anything that needs help being cut? We offer a solution for you! The Need Cut service is a high-tech cutting tool that automates the preparation of food items. Whether you're making a salad or slicing meat, this tool offers precise, fast, and consistent cuts. With specialized cutting techniques, it ensures your meal prep is quick and easy, saving you time and effort in the kitchen. It’s the perfect addition to any modern kitchen!</p>
            <!-- Accordion for Need Cut -->
            <div class="accordion" id="accordion4">
              <div class="accordion-item">
                <h2 class="accordion-header" id="headingFour">
                  <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour" aria-expanded="true" aria-controls="collapseFour">
                    More Details
                  </button>
                </h2>
                <div id="collapseFour" class="accordion-collapse collapse" aria-labelledby="headingFour" data-bs-parent="#accordion4">
                  <div class="accordion-body">
                    More details about Need Cut.
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>
</div>
```
<p>Over the next two days, I added more detailed content to the site, including text blocks, buttons, and placeholder images. I also set up a simple Bootstrap carousel for the interactive element, which will later showcase some of the tech concepts I’m working on. This gave the page more structure and interactivity, even if it’s still using placeholders for now.</p>

#### 4/28–4/29: Finalize Desktop & Mobile views. Make it fully responsive. Adjust margins/paddings.

```html
@media (max-width: 768px) {
  .hero .carousel-item {
    height: 250px;
  }

  .aframe-container {
    height: 250px;
  }

  .footer .img {
    width: 60px;
  }

  .card-style {
    margin-bottom: 30px;
  }

  .navbar-brand {
    font-size: 1.2rem;
  }

  .carousel h2 {
    font-size: 1.25rem;
    text-align: center;
  }
}
```
<p>In these two days, I spent a lot of time adjusting the margins, paddings, and breakpoints for mobile and desktop views. The goal was to ensure that the site was fully responsive and that elements like the hero section and carousel displayed well on all screen sizes. I used Bootstrap’s built-in grid system to handle most of the layout changes but added a few custom media queries to fine-tune things.</p>
#### 5/4: Test the site: fix mobile spacing, font issues, broken links.

```html
<!-- Mobile adjustments -->
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
<p>On May 4th, I focused on testing the site on both mobile and desktop devices. I noticed that some mobile views had issues with font sizes and spacing, so I adjusted the padding and font-size properties in the CSS. I also fixed a few broken links that were causing errors when navigating the site. It was a bit tedious, but it was important to ensure the site worked smoothly for all users.</p>

#### 5/5: Last review and submit Freedom Project.
<p>After all the testing, I did a final review of the site, ensuring that all elements were functioning as expected. I made sure that all interactive features (like the carousel) were working and that all the images and text content were in place. After fixing a couple of last-minute issues, I submitted the project as part of my Freedom Project. It was great to see everything come together after weeks of hard work!</p>

#### This is my entire website
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Freedom Project</title>

  <!-- Bootstrap -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet" />
  <!-- Bootstrap Icons -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons/font/bootstrap-icons.css" rel="stylesheet" />
  <!-- A-Frame -->
  <script src="https://aframe.io/releases/1.4.2/aframe.min.js"></script>
  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Bruno+Ace+SC&display=swap" rel="stylesheet" />
  <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@300..700&display=swap" rel="stylesheet" />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Bruno+Ace+SC&family=Fira+Code:wght@300..700&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&family=Space+Grotesk:wght@300..700&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Bruno Ace SC', sans-serif;
      margin: 0;
      padding: 0;
    }

    code, pre {
      font-family: 'Fira Code', monospace;
    }

    .navbar-brand {
      font-size: 1.5rem;
    }

    .hero .carousel-item {
      height: 400px;
    }

    .hero .carousel-item > div {
      height: 100%;
    }

    .aframe-container {
      width: 100%;
      height: 400px;
      margin: 50px 0;
    }

    .card-style {
      background: #f8f9fa;
      border-radius: 10px;
      padding: 2rem;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      height: 100%;
      margin-bottom: 20px;
    }

    footer {
      background-color: #93827F;
      color: white;
      padding: 20px 0;
      text-align: center;
    }

    footer img {
      width: 80px;
      margin-top: 10px;
    }

    /* Responsive Design */
    @media (max-width: 768px) {
      .hero .carousel-item {
        height: 250px;
      }

      .aframe-container {
        height: 250px;
      }

      footer img {
        width: 60px;
      }

      .card-style {
        margin-bottom: 30px;
      }

      .navbar-brand {
        font-size: 1.2rem;
      }

      .carousel h2 {
        font-size: 1.25rem;
        text-align: center;
      }
    }

    .card-img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      border-radius: 10px;
    }
  </style>
</head>

<body>
  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-light bg-light shadow-sm">
    <div class="container">
      <a class="navbar-brand" href="#">Cooking</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link" href="#">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="#test">About</a></li>
          <li class="nav-item"><a class="nav-link" href="#test2">Content</a></li>
          <li class="nav-item"><a class="nav-link" href="#test3">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Hero Section -->
  <section class="hero p-0">
    <div id="heroCarousel" class="carousel slide" data-bs-ride="carousel" data-bs-interval="3000">
      <div class="carousel-indicators">
        <button type="button" data-bs-target="#heroCarousel" data-bs-slide-to="0" class="active"></button>
        <button type="button" data-bs-target="#heroCarousel" data-bs-slide-to="1"></button>
        <button type="button" data-bs-target="#heroCarousel" data-bs-slide-to="2"></button>
      </div>

      <div class="carousel-inner">
        <div class="carousel-item active">
          <div class="d-flex align-items-center justify-content-center bg-success-subtle">
            <img src="../Photo/chef.jpg" class="d-block w-75" alt="Chef preparing food">
            <h2>Scientific Breakthroughs</h2>
          </div>
        </div>
        <div class="carousel-item">
          <div class="d-flex align-items-center justify-content-center bg-primary-subtle">
            <h2>Cooking Technologies</h2>
            <img src="../Photo/food.jpg" class="d-block w-75" alt="Modern food tech">
          </div>
        </div>
        <div class="carousel-item">
          <div class="d-flex align-items-center justify-content-center bg-warning-subtle">
            <img src="../Photo/rice.jpeg" class="d-block w-75" alt="Sustainable rice farming">
            <h2>Innovative Ideas</h2>
          </div>
        </div>
      </div>

      <button class="carousel-control-prev" type="button" data-bs-target="#heroCarousel" data-bs-slide="prev">
        <span class="carousel-control-prev-icon"></span>
      </button>
      <button class="carousel-control-next" type="button" data-bs-target="#heroCarousel" data-bs-slide="next">
        <span class="carousel-control-next-icon"></span>
      </button>
    </div>
  </section>
  <section class="py-5">
    <div class="container" id="test">
      <div class="card-style text-center">
        <h3>Content</h3>
        <p>This project explores innovative food technologies that can transform how we cook, eat, and sustain ourselves. From 3D-printed meals to molecular recombination, these tools aim to solve real-world problems such as hunger, food waste, and accessibility—paving the way for a smarter, more sustainable future in the kitchen.</p>
      </div>
    </div>
  </section>
  <!-- A-Frame Section -->
  <section class="aframe-container">
    <a-scene embedded cursor="rayOrigin: mouse">

      <!-- Floor -->
      <a-plane position="0 0 -5" rotation="-90 0 0" width="10" height="10" color="#cccccc"></a-plane>

      <!-- Walls -->
      <a-box position="0 2.5 -10" width="10" height="5" depth="0.1" color="#f0e6d2"></a-box> <!-- Back wall -->
      <a-box position="-5 2.5 -5" width="0.1" height="5" depth="10" color="#f0e6d2"></a-box> <!-- Left wall -->
      <a-box position="5 2.5 -5" width="0.1" height="5" depth="10" color="#f0e6d2"></a-box> <!-- Right wall -->
      <a-box position="0 5 -5" width="10" height="0.1" depth="10" color="#dddddd"></a-box> <!-- Ceiling -->

      <!-- Kitchen Items -->
      <a-box position="-2 1 -6" width="2" height="1" depth="1" color="#8B4513"></a-box> <!-- Kitchen counter -->
      <a-box position="0 1 -6" width="1" height="1.5" depth="1" color="#aaa"></a-box> <!-- Fridge -->
      <a-box position="2 0.75 -6" width="1.5" height="0.5" depth="1" color="#555"></a-box> <!-- Stove -->
      <a-cylinder position="2 1.2 -6" radius="0.1" height="0.1" color="red"></a-cylinder> <!-- Pot on stove -->

      <!-- Table -->
      <a-box position="0 0.75 -3" width="2" height="0.1" depth="1" color="#deb887"></a-box> <!-- Table top -->
      <a-cylinder position="-0.8 0.375 -2.6" radius="0.05" height="0.75" color="#654321"></a-cylinder>
      <a-cylinder position="0.8 0.375 -2.6" radius="0.05" height="0.75" color="#654321"></a-cylinder>
      <a-cylinder position="-0.8 0.375 -3.4" radius="0.05" height="0.75" color="#654321"></a-cylinder>
      <a-cylinder position="0.8 0.375 -3.4" radius="0.05" height="0.75" color="#654321"></a-cylinder>

      <!-- Lighting -->
      <a-light type="ambient" color="#ffffff" intensity="0.5"></a-light>
      <a-light type="point" intensity="1" position="0 4 -5" color="#fff"></a-light>

      <!-- Camera Rig -->
      <a-entity id="rig" movement-controls="fly: true">
        <a-entity camera position="0 1.6 0" look-controls></a-entity>
      </a-entity>

      <!-- Sky -->
      <a-sky color="#ECECEC"></a-sky>

    </a-scene>
  </section>
<!--accordion-->
<div class="accordion" id="accordion">
  <section class="py-5">
    <div class="container" id="test2">
      <div class="row text-center">

        <!-- Recombinator Card with Accordion on the right -->
        <div class="col-12 col-md-6 d-flex align-items-center">
          <img src="./photo/wasten.png" alt="Recombinator" class="card-img">
        </div>
        <div class="col-12 col-md-6">
          <div class="card-style">
            <h4><i class="bi bi-heart-fill me-2"></i>Recombinator</h4>
            <p>I came up with an item for people who are poor and need nutritious food. The Recombinator is a machine that uses food waste and turns it into a full meal. Using advanced 3D food printing technology, we are able to mix various ingredients to create meals tailored to nutritional needs. This solution not only addresses food scarcity but also reduces waste and makes food more accessible for everyone.</p>
            <!-- Accordion for Recombinator -->
            <div class="accordion" id="accordion1">
              <div class="accordion-item">
                <h2 class="accordion-header" id="headingOne">
                  <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
                    More Details
                  </button>
                </h2>
                <div id="collapseOne" class="accordion-collapse collapse show" aria-labelledby="headingOne" data-bs-parent="#accordion1">
                  <div class="accordion-body">
                    More detailed information about Recombinator will go here.
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- Printer Cooking Station Card with Accordion on the right -->
        <div class="col-12 col-md-6 d-flex align-items-center">
          <img src="./photo/Printer.png" alt="Printer Cooking Station" class="card-img">
        </div>
        <div class="col-12 col-md-6">
          <div class="card-style">
            <h4><i class="bi bi-cup-fill me-2"></i>Printer Cooking Station</h4>
            <p>What if you were stuck in the middle of nowhere, too lazy to cook anything, or just didn't have the time? The Printer Cooking Station is here to solve that problem. This machine uses 3D printing to prepare meals quickly and efficiently. With just a few ingredients and a simple recipe, you can have a freshly made meal printed in front of you. It's fast, customizable, and designed for modern living.</p>
            <!-- Accordion for Printer Cooking Station -->
            <div class="accordion" id="accordion2">
              <div class="accordion-item">
                <h2 class="accordion-header" id="headingTwo">
                  <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseTwo" aria-expanded="true" aria-controls="collapseTwo">
                    More Details
                  </button>
                </h2>
                <div id="collapseTwo" class="accordion-collapse collapse" aria-labelledby="headingTwo" data-bs-parent="#accordion2">
                  <div class="accordion-body">
                    More detailed information about Printer Cooking Station.
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- Digital Item Website Card with Accordion on the right -->
        <div class="col-12 col-md-6 d-flex align-items-center">
          <img src="./photo/Shop.png" alt="Digital Item Website" class="card-img">
        </div>
        <div class="col-12 col-md-6">
          <div class="card-style">
            <h4><i class="bi bi-cart-fill me-2"></i>Digital Item Website</h4>
            <p>Want any item that appears to you without waiting for shipping? Our Digital Item Website has the solution. Whether it's a recipe, a cooking tool, or even a virtual product, we have the infrastructure to create and deliver digital items instantly. This innovative platform uses digital printing and technology to provide you with customized items on demand, all within minutes. No more waiting, just order and receive your digital item.</p>
            <!-- Accordion for Digital Item Website -->
            <div class="accordion" id="accordion3">
              <div class="accordion-item">
                <h2 class="accordion-header" id="headingThree">
                  <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseThree" aria-expanded="true" aria-controls="collapseThree">
                    More Details
                  </button>
                </h2>
                <div id="collapseThree" class="accordion-collapse collapse" aria-labelledby="headingThree" data-bs-parent="#accordion3">
                  <div class="accordion-body">
                    More details about the Digital Item Website.
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- Need Cut Card with Accordion on the right -->
        <div class="col-12 col-md-6 d-flex align-items-center">
          <img src="./photo/katanan.png" alt="Need Cut" class="card-img">
        </div>
        <div class="col-12 col-md-6">
          <div class="card-style">
            <h4><i class="bi bi-cart-fill me-2"></i>Need Cut</h4>
            <p>Anything that needs help being cut? We offer a solution for you! The Need Cut service is a high-tech cutting tool that automates the preparation of food items. Whether you're making a salad or slicing meat, this tool offers precise, fast, and consistent cuts. With specialized cutting techniques, it ensures your meal prep is quick and easy, saving you time and effort in the kitchen. It’s the perfect addition to any modern kitchen!</p>
            <!-- Accordion for Need Cut -->
            <div class="accordion" id="accordion4">
              <div class="accordion-item">
                <h2 class="accordion-header" id="headingFour">
                  <button class="accordion-button" type="button" data-bs-toggle="collapse" data-bs-target="#collapseFour" aria-expanded="true" aria-controls="collapseFour">
                    More Details
                  </button>
                </h2>
                <div id="collapseFour" class="accordion-collapse collapse" aria-labelledby="headingFour" data-bs-parent="#accordion4">
                  <div class="accordion-body">
                    More details about Need Cut.
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>
</div>




  <!-- Footer -->
  <footer>
    <p>&copy; 2025 Derrick Chen. All Rights Reserved.</p>
    <img src="../photo/logo.png" alt="Logo">
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```
# Engineering Design Process
I’m currently finalizing all the content for the website as part of my engineering design process. This involves refining text, optimizing images, and ensuring a user-friendly layout to enhance the overall user experience and functionality.
# Source
* `Bootstrap`:[here](https://getbootstrap.com/)
* `Accordion`:[here](https://getbootstrap.com/docs/5.3/migration/#accordion)
* `Navbar`:[here](https://getbootstrap.com/docs/5.3/components/scrollspy/#navbar)
* `Carousel`:[here](https://getbootstrap.com/docs/5.3/components/carousel/#how-it-works)
* `A-Frame`:[here](https://aframe.io/docs/1.7.0/introduction/)
* `Wireframe Mobile`:[here](https://wireframe.cc/q2BTod)
* `Wireframe Desktop`:[here](https://wireframe.cc/cfbx8R)

# Skill:
## Time Management
Time management was critical throughout this project. With multiple tasks to complete in a short time frame, I had to stay organized and prioritize each step. I used tools like Trello and Google Calendar to break down the project into manageable chunks and stay on track.

## Problem Solving
I ran into a few roadblocks along the way—broken links, spacing issues, and layout bugs. The key to overcoming these challenges was persistence. I took breaks when needed, googled for solutions, and consulted the official documentation to troubleshoot and resolve the issues.

## Takeaway
Even though I started with basic placeholders and rough layouts, I was able to build a fully functional, responsive website by focusing on one task at a time. This project taught me the importance of organization and testing as I went along. In the future, I’ll give myself more time to focus on the finer details, but overall, I’m really happy with the result!





[Previous](entry05.md) | [Next](entry07.md)

[Home](../README.md)
