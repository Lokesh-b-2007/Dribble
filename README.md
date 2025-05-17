# Project Responsive Web Design using Bootstrap
## Date:17.05.2025

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
home.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Samsung Clone</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"/>
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;600;700&display=swap" rel="stylesheet">

  <style>
    body {
      margin: 0;
      font-family: 'Outfit', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }

    .hero-section {
      position: relative;
      height: 100vh;
      overflow: hidden;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
    }

    .hero-video {
      position: absolute;
      top: 50%;
      left: 50%;
      width: 100%;
      height: 100%;
      object-fit: cover;
      transform: translate(-50%, -50%);
      z-index: -1;
    }

    .hero-content {
      z-index: 2;
      color: white;
      background: rgba(0, 0, 0, 0.5);
      padding: 2rem;
      border-radius: 15px;
      max-width: 90%;
    }

    .hero-content h1 {
      font-size: 3rem;
      font-weight: 700;
    }

    .hero-content p {
      font-size: 1.25rem;
      margin-bottom: 1rem;
    }

    .products img {
      height: 300px;
      object-fit: cover;
    }

    footer {
      background-color: #000;
      color: #fff;
      padding: 20px 0;
    }
  </style>
</head>
<body>


  <nav class="navbar navbar-expand-lg bg-dark navbar-dark fixed-top">
    <div class="container">
      <a class="navbar-brand" href="#">Samsung</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
        data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false"
        aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item"><a class="nav-link" href="home.html">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="galaxy.html">Galaxy</a></li>
          <li class="nav-item"><a class="nav-link" href="phones.html">Phones</a></li>
          <li class="nav-item"><a class="nav-link" href="tablets.html">Tablets</a></li>
          <li class="nav-item"><a class="nav-link" href="wearables.html">Wearables</a></li>
          <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <header class="hero-section">
    <video autoplay muted loop playsinline class="hero-video">
      <source src="samsung_bg.mp4" type="video/mp4" />
    </video>
    <div class="hero-content">
      <h1>Galaxy S25 Ultra</h1>
      <p>Smarter. Sharper. Sleeker.</p>
      <a href="galaxy.html" class="btn btn-light">Explore Now</a>
    </div>
  </header>

  <section class="products py-5">
    <div class="container">
      <h2 class="text-center mb-5 fw-bold">Featured Products</h2>
      <div class="row g-4">
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="image.png" class="card-img-top" alt="Galaxy Tab S9">
            <div class="card-body">
              <h5 class="card-title fw-bold">Galaxy Tab S9 FE+</h5>
              <p class="card-text">Power and portability in perfect harmony.</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="ini2.jpg" class="card-img-top" alt="Galaxy Watch 6">
            <div class="card-body">
              <h5 class="card-title fw-bold">Galaxy Watch 7</h5>
              <p class="card-text">Your health, powered by Samsung.</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="25.jpg" class="card-img-top" alt="Galaxy S24 Ultra">
            <div class="card-body">
              <h5 class="card-title fw-bold">Galaxy S25 Ultra</h5>
              <p class="card-text">AI at your fingertips.</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <footer class="text-center">
    <p class="mb-0">© 2025 Samsung Clone. Designed for educational purposes.</p>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

~~~
galaxy.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Galaxy | Samsung</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"/>
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;600;700&display=swap" rel="stylesheet"/>

  <style>
    body {
      margin: 0;
      font-family: 'Outfit', sans-serif;
    }

    .hero-section {
      position: relative;
      height: 100vh;
      overflow: hidden;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      color: white;
    }

    .hero-video {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
      z-index: -1;
    }

    .hero-content {
      position: relative;
      z-index: 1;
      background: rgba(0, 0, 0, 0.5);
      padding: 2rem;
      border-radius: 12px;
    }

    .hero-content h1 {
      font-size: 3.5rem;
      font-weight: 700;
    }

    .products img {
      height: 250px;
      object-fit: cover;
      border-radius: 8px 8px 0 0;
    }

    .card {
      transition: transform 0.3s ease;
    }

    .card:hover {
      transform: translateY(-5px);
    }

    footer {
      background-color: #000;
      color: #fff;
      padding: 20px 0;
      font-size: 0.95rem;
    }
  </style>
</head>
<body>

  
  <nav class="navbar navbar-expand-lg bg-dark navbar-dark fixed-top">
    <div class="container">
      <a class="navbar-brand fw-bold" href="index.html">Samsung</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
        data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false"
        aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item"><a class="nav-link active" href="home.html">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="galaxy.html">Galaxy</a></li>
          <li class="nav-item"><a class="nav-link" href="phones.html">Phones</a></li>
          <li class="nav-item"><a class="nav-link" href="tablets.html">Tablets</a></li>
          <li class="nav-item"><a class="nav-link" href="wearables.html">Wearables</a></li>
          <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  
  <header class="hero-section">
    <video autoplay muted loop playsinline class="hero-video">
      <source src="bbgg.mp4" type="video/mp4" />
    </video>
    <div class="hero-content">
      <h1>Galaxy S25 Ultra</h1>
      <p>Epic in every way.</p>
      <a href="phones.html" class="btn btn-light mt-3">Explore Now</a>
    </div>
  </header>

  
  <section class="products py-5">
    <div class="container">
      <h2 class="text-center mb-5 fw-bold">Galaxy Lineup</h2>
      <div class="row g-4">
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="25.jpg" class="card-img-top" alt="Galaxy S24 Ultra">
            <div class="card-body">
              <h5 class="card-title fw-bold">Galaxy S25 Ultra</h5>
              <p class="card-text">Ultimate power and AI smarts.</p>
              <p class="text-muted fw-semibold">$1,199</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="image.png" class="card-img-top" alt="Galaxy Tab S9">
            <div class="card-body">
              <h5 class="card-title fw-bold">Galaxy Tab S9 FE+</h5>
              <p class="card-text">Built for creators and pros.</p>
              <p class="text-muted fw-semibold">$899</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card border-0 shadow text-center">
            <img src="ini2.jpg" class="card-img-top" alt="Galaxy Watch 6">
            <div class="card-body">
              <h5 class="card-title fw-bold">Galaxy Watch 7</h5>
              <p class="card-text">Smarter health on your wrist.</p>
              <p class="text-muted fw-semibold">$299</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  
  <section class="features py-5 bg-light">
    <div class="container">
      <h2 class="text-center fw-bold mb-5">Why Galaxy?</h2>
      <div class="row g-4">
        <div class="col-md-4 text-center">
          <img src="https://img.icons8.com/ios-filled/100/000000/artificial-intelligence.png" width="60" alt="AI Icon" />
          <h5 class="mt-3 fw-semibold">Galaxy AI</h5>
          <p>Next-gen intelligence to boost your productivity and creativity.</p>
        </div>
        <div class="col-md-4 text-center">
          <img src="https://img.icons8.com/ios-filled/100/000000/fingerprint-scan.png" width="60" alt="Security Icon" />
          <h5 class="mt-3 fw-semibold">Advanced Security</h5>
          <p>Samsung Knox keeps your data safe and your privacy protected.</p>
        </div>
        <div class="col-md-4 text-center">
          <img src="https://img.icons8.com/ios-filled/100/000000/smartphone-tablet.png" width="60" alt="Ecosystem Icon" />
          <h5 class="mt-3 fw-semibold">Galaxy Ecosystem</h5>
          <p>Seamlessly connect your devices to stay in sync wherever you go.</p>
        </div>
      </div>
    </div>
  </section>

  
  <footer class="text-center mt-5">
    <p class="mb-0">© 2025 Samsung Clone | Galaxy Page | Educational Use Only</p>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

~~~
phones.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Galaxy Phones</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"/>
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;600;700&display=swap" rel="stylesheet"/>

  <style>
    body {
      font-family: 'Outfit', sans-serif;
    }

    .page-header {
      background: #000;
      color: #fff;
      padding: 4rem 0;
      text-align: center;
    }

    .product img {
      height: 250px;
      object-fit: cover;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg bg-dark navbar-dark fixed-top">
    <div class="container">
      <a class="navbar-brand fw-bold" href="index.html">Samsung</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
        data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false"
        aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item"><a class="nav-link" href="home.html">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="galaxy.html">Galaxy</a></li>
          <li class="nav-item"><a class="nav-link active" href="phones.html">Phones</a></li>
          <li class="nav-item"><a class="nav-link" href="tablets.html">Tablets</a></li>
          <li class="nav-item"><a class="nav-link" href="wearables.html">Wearables</a></li>
          <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Header -->
  <header class="page-header">
    <h1>Galaxy Phones</h1>
    <p>Explore the latest Galaxy innovations</p>
  </header>

  <!-- Phones Section -->
  <section class="py-5">
    <div class="container">
      <div class="row g-4">
        <div class="col-md-4">
          <div class="card product text-center shadow">
            <img src="24.png" class="card-img-top" alt="Galaxy S24 Ultra">
            <div class="card-body">
              <h5 class="fw-bold">Galaxy S24 Ultra</h5>
              <p>AI-powered camera. Titanium frame.</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card product text-center shadow">
            <img src="pp.png" class="card-img-top" alt="Galaxy Z Flip5">
            <div class="card-body">
              <h5 class="fw-bold">Galaxy Z Flip5</h5>
              <p>Pocket-sized style. Big features.</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card product text-center shadow">
            <img src="ss.jpg" class="card-img-top" alt="Galaxy Z Fold5">
            <div class="card-body">
              <h5 class="fw-bold">Galaxy Z Fold5</h5>
              <p>Unfold productivity like never before.</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <footer class="text-center bg-dark text-white py-3">
    <p class="mb-0">© 2025 Samsung Clone | Phones Page | Educational Use Only</p>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

~~~
tablets.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Galaxy Tablets</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"/>
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;600;700&display=swap" rel="stylesheet"/>

  <style>
    body {
      font-family: 'Outfit', sans-serif;
    }

    .page-header {
      background: #111;
      color: #fff;
      padding: 4rem 0;
      text-align: center;
    }

    .product img {
      height: 250px;
      object-fit: cover;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg bg-dark navbar-dark fixed-top">
    <div class="container">
      <a class="navbar-brand fw-bold" href="index.html">Samsung</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
        data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false"
        aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item"><a class="nav-link" href="home.html">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="galaxy.html">Galaxy</a></li>
          <li class="nav-item"><a class="nav-link" href="phones.html">Phones</a></li>
          <li class="nav-item"><a class="nav-link active" href="tablets.html">Tablets</a></li>
          <li class="nav-item"><a class="nav-link" href="wearables.html">Wearables</a></li>
          <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Header -->
  <header class="page-header">
    <h1>Galaxy Tablets</h1>
    <p>Powerful tools for work and creativity</p>
  </header>

  <!-- Tablets Section -->
  <section class="py-5">
    <div class="container">
      <div class="row g-4">
        <div class="col-md-6">
          <div class="card product text-center shadow">
            <img src="ee.avif" class="card-img-top" alt="Galaxy Tab S9">
            <div class="card-body">
              <h5 class="fw-bold">Galaxy Tab S9</h5>
              <p>Vivid AMOLED display with S Pen.</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
        <div class="col-md-6">
          <div class="card product text-center shadow">
            <img src="dd.avif" class="card-img-top" alt="Galaxy Tab A9+">
            <div class="card-body">
              <h5 class="fw-bold">Galaxy Tab A9+</h5>
              <p>Affordable performance for everyday use.</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <footer class="text-center bg-dark text-white py-3">
    <p class="mb-0">© 2025 Samsung Clone | Tablets Page | Educational Use Only</p>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

~~~
wearables.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Galaxy Wearables</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"/>
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;600;700&display=swap" rel="stylesheet"/>

  <style>
    body {
      font-family: 'Outfit', sans-serif;
    }

    .page-header {
      background: #000;
      color: #fff;
      padding: 4rem 0;
      text-align: center;
    }

    .product img {
      height: 250px;
      object-fit: cover;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg bg-dark navbar-dark fixed-top">
    <div class="container">
      <a class="navbar-brand fw-bold" href="index.html">Samsung</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
        data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false"
        aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item"><a class="nav-link" href="home.html">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="galaxy.html">Galaxy</a></li>
          <li class="nav-item"><a class="nav-link" href="phones.html">Phones</a></li>
          <li class="nav-item"><a class="nav-link" href="tablets.html">Tablets</a></li>
          <li class="nav-item"><a class="nav-link" href="wearables.html">Wearables</a></li>
          <li class="nav-item"><a class="nav-link" href="contact.html">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Header -->
  <header class="page-header mt-5">
    <h1>Galaxy Wearables</h1>
    <p>Smart, stylish, and connected</p>
  </header>

  <!-- Wearables Section -->
  <section class="py-5">
    <div class="container">
      <div class="row g-4">
        <div class="col-md-4">
          <div class="card product text-center shadow">
            <img src="ini2.jpg" class="card-img-top" alt="Galaxy Watch6">
            <div class="card-body">
              <h5 class="fw-bold">Galaxy Watch 7</h5>
              <p>Advanced health monitoring and sleek design.</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card product text-center shadow">
            <img src="hh.png" class="card-img-top" alt="Galaxy Watch6 Classic">
            <div class="card-body">
              <h5 class="fw-bold">Galaxy Ring</h5>
              <p>Technology in finger.</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card product text-center shadow">
            <img src="rr.avif" class="card-img-top" alt="Galaxy Buds2 Pro">
            <div class="card-body">
              <h5 class="fw-bold">Galaxy Buds2 Pro</h5>
              <p>Hi-fi sound and intelligent noise canceling.</p>
              <a href="#" class="btn btn-dark">Buy</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <footer class="text-center bg-dark text-white py-3">
    <p class="mb-0">© 2025 Samsung Clone | Wearables Page | Educational Use Only</p>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

~~~
contact.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Contact Us - Samsung Clone</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"/>
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;600;700&display=swap" rel="stylesheet"/>

  <style>
    body {
      font-family: 'Outfit', sans-serif;
    }

    .contact-header {
      background: #222;
      color: white;
      padding: 3rem 0;
      text-align: center;
    }

    .form-section {
      max-width: 700px;
      margin: 0 auto;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg bg-dark navbar-dark fixed-top">
    <div class="container">
      <a class="navbar-brand fw-bold" href="index.html">Samsung</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse"
        data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false"
        aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse justify-content-end" id="navbarNav">
        <ul class="navbar-nav">
          <li class="nav-item"><a class="nav-link" href="home.html">Home</a></li>
          <li class="nav-item"><a class="nav-link" href="galaxy.html">Galaxy</a></li>
          <li class="nav-item"><a class="nav-link" href="phones.html">Phones</a></li>
          <li class="nav-item"><a class="nav-link" href="tablets.html">Tablets</a></li>
          <li class="nav-item"><a class="nav-link" href="wearables.html">Wearables</a></li>
          <li class="nav-item"><a class="nav-link active" href="contact.html">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Contact Header -->
  <header class="contact-header mt-5">
    <h1>Contact Us</h1>
    <p>We'd love to hear from you</p>
  </header>

  <!-- Contact Form -->
  <section class="py-5">
    <div class="container form-section">
      <form>
        <div class="mb-3">
          <label for="name" class="form-label">Full Name</label>
          <input type="text" class="form-control" id="name" placeholder="Your name" required>
        </div>
        <div class="mb-3">
          <label for="email" class="form-label">Email Address</label>
          <input type="email" class="form-control" id="email" placeholder="name@example.com" required>
        </div>
        <div class="mb-3">
          <label for="message" class="form-label">Your Message</label>
          <textarea class="form-control" id="message" rows="5" placeholder="How can we help?" required></textarea>
        </div>
        <button type="submit" class="btn btn-dark w-100">Send Message</button>
      </form>
    </div>
  </section>

  <footer class="text-center bg-dark text-white py-3">
    <p class="mb-0">© 2025 Samsung Clone | Contact Page | Educational Use Only</p>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

~~~

## OUTPUT:
![alt text](<Screenshot 2025-05-17 212209.png>)
![alt text](<Screenshot 2025-05-17 212219.png>)
![alt text](<Screenshot 2025-05-17 212300.png>)
![alt text](<Screenshot 2025-05-17 212307.png>)
![alt text](<Screenshot 2025-05-17 212317.png>)
![alt text](<Screenshot 2025-05-17 212325.png>)
![alt text](<Screenshot 2025-05-17 212332.png>)
![alt text](<Screenshot 2025-05-17 212343.png>)
## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
