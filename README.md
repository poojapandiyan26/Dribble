# Project Responsive Web Design using Bootstrap
## Date:25.12.2024

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
```
index.html

.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dribbble Clone</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <!-- Navigation Bar -->
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container">
      <a class="navbar-brand" href="#">Dribbble</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link" href="#">Explore</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Blog</a></li>
          <li class="nav-item"><a class="nav-link text-primary" href="#">Sign Up</a></li>
          <li class="nav-item"><a class="nav-link" href="#">Log In</a></li>
        </ul>
      </div>
    </div>
  </nav>

  <!-- Hero Section -->
  <header class="hero-section text-center text-white d-flex align-items-center justify-content-center">
    <div class="container">
      <h1 class="display-4 fw-bold">Personalized Interiors, Perfectly You.</h1>
      <p class="lead">Transforming Spaces, Elevating Lives.</p>
    <form class="d-flex justify-content-center mt-3">
        <input type="text" class="form-control w-50" placeholder="Search" />
      </form>
    </div>
  </header>

  <!-- Trending Searches Section -->
  <section class="py-5 text-center">
    <div class="container">
      <h2>Trending Searches</h2>
      <div class="d-flex flex-wrap justify-content-center mt-3">
        <a href="#" class="btn btn-primary m-1">Architectural Design</a>
        <a href="#" class="btn btn-outline-primary m-1">Interior Design</a>
        <a href="#" class="btn btn-outline-primary m-1">Supervision & Furnishing</a>
        <a href="#" class="btn btn-outline-primary m-1">top designer</a>
        <a href="#" class="btn btn-outline-primary m-1">dashboard</a>
        <a href="#" class="btn btn-outline-primary m-1">icons</a>
      </div>
    </div>
  </section>

  <!-- Featured Designs Section -->
  <section class="py-5 bg-light">
    <div class="container">
      <div class="row g-4">
        <!-- Example Card -->
        <div class="col-md-4">
            <div class="card shadow-sm">
              <img src="balcony.jpg" class="card-img-top" alt="balcony">
              <div class="card-body">
                <h5 class="card-title">balcony</h5>
                <p class="card-text text-muted">Emote Team | 7.2k Views</p>
              </div>
            </div>
          </div>
        <div class="col-md-4">
          <div class="card shadow-sm">
            <img src="kitchen.jpg" class="card-img-top" alt="kitchen">
            <div class="card-body">
              <h5 class="card-title">kitchen</h5>
              <p class="card-text text-muted">Emote Team | 8.2k Views</p>
            </div>
          </div>
        </div>
        <!-- Repeat for other cards -->
        <div class="col-md-4">
          <div class="card shadow-sm">
            <img src="bedroom.jpg" class="card-img-top" alt="bedroom">
            <div class="card-body">
              <h5 class="card-title">bedroom</h5>
              <p class="card-text text-muted">Emote Team | 9.2k Views</p>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card shadow-sm">
            <img src="living area.jpg" class="card-img-top" alt="living area">
            <div class="card-body">
              <h5 class="card-title">living area</h5>
              <p class="card-text text-muted">Emote Team | 5.2k Views</p>
            </div>
          </div>
        </div>
        <div class="col-md-4">
            <div class="card shadow-sm">
              <img src="swimming.jpg" class="card-img-top" alt="swimming">
              <div class="card-body">
                <h5 class="card-title">swimming</h5>
                <p class="card-text text-muted">Emote Team | 100k Views</p>
              </div>
            </div>
          </div>
          <div class="col-md-4">
            <div class="card shadow-sm">
              <img src="dining.jpg" class="card-img-top" alt="dining">
              <div class="card-body">
                <h5 class="card-title">dining</h5>
                <p class="card-text text-muted">Emote Team | 105k Views</p>
              </div>
            </div>
          </div>
        <!-- Add more cards -->
      </div>
    </div>
  </section>
 
  <footer class="bg-dark text-center text-white py-3">
    <p>&copy; 2024 Designed by POOJA SRI P</p>
  </footer>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

style.css

.hero-section {
    background: url('interior bg.jpg') center center / cover no-repeat;
    height: 400px;
  }
  
  .hero-section h1 {
    color: rgb(255, 255, 255);
    text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7);
  }
  
  .hero-section p {
    color: rgba(255, 255, 255, 0.9);
    text-shadow: 1px 1px 3px rgba(7, 37, 12, 0.7);
  }
  
  .btn-outline-primary {
    border-color: #004917;
    color: #005513;
  }
  
  .btn-outline-primary:hover {
    background-color: #007bff;
    color: #ffffff;
  }
  body {
    background-color: #d6cc37; /* Replace this with your desired color */
    margin: 0; /* Remove default margin */
    height: 500%; /* Ensure full-page height */
  }
  html, body {
    height: 100%;
    background-color: #d4c245; /* Replace with your preferred color */
  }
  /* Apply background color to the entire page */
body {
    background-color: #d4c245; /* Replace with your preferred color */
    margin: 0;
    padding: 0;
  }
  
  /* Ensure sections also inherit the background */
  section {
    background-color: transparent; /* Allow body color to show through */
  }
  
  /* For padding adjustments */
  .header, .trending, .featured {
    padding: 20px;
  }
/* Style for the hero section heading */
.hero-section h1 {
    text-align: left; /* Align text to the left */
    font-family: 'Georgia', serif; /* Change font style */
    font-size: 3rem; /* Adjust font size */
    font-weight: bold; /* Adjust weight */
    margin-left: 10%; /* Add space from the left */
    color: #ffffff; /* Optional: Adjust text color */
  }
  
  /* Style the description text */
  .hero-section p {
    text-align: left; /* Align to the left */
    font-family: 'Arial', sans-serif; /* Optional: Change font */
    margin-left: 10%; /* Match margin with heading */
    color: #ffffff; /* Ensure good contrast with background */
  }
```

## OUTPUT:
![alt text](<1 (4).png>)
![alt text](<2 (4).png>)
![alt text](<3 (4).png>)


## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
