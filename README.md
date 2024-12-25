# Project Responsive Web Design using Bootstrap
# Date: 25/11/2024
# AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

## Step 5:
Create a HTML file and include the needed Bootstrap components.

## Step 6:
Publish the website in the LocalHost.

# PROGRAM :
Index.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Dribbble</title>
  
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>

 
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top">
    <div class="container">
      <a class="navbar-brand" href="#">Dribbble Showcase</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item">
            <a class="nav-link" href="sign.html">Sign up</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#shots">Login</a>
          </li>
        </ul>

        
        <form class="d-flex ms-3" action="#" method="GET">
          <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
          <button class="btn btn-outline-secondary" type="submit">Search</button>
        </form>
      </div>
    </div>
  </nav>


  <div class="container-fluid bg-primary text-white py-5" id="home">
    <div class="container text-center">
      <h1 class="display-4">Discover the Best Creative Works</h1>
      <p class="lead">Showcase your designs, get inspired, and connect with other creatives.</p>
      <a href="#shots" class="btn btn-dark mt-3">Explore Shots</a>
    </div>
  </div>

  
  <div id="shots" class="container my-5">
    <h2 class="text-center mb-4">Featured Design Shots</h2>
    <div class="row row-cols-1 row-cols-md-3 g-4">
      
      <div class="col">
        <div class="card shadow-sm border-0">
          <img src="6.jpeg" class="card-img-top" alt="Shot 1">
          <div class="card-body">
            <h5 class="card-title">Modern Logo Design</h5>
            <p class="card-text">A sleek and minimalistic logo design for a modern tech company.</p>
            <a href="#" class="btn btn-outline-secondary">View More</a>
          </div>
        </div>
      </div>
      
      <div class="col">
        <div class="card shadow-sm border-0">
          <img src="5.jpeg" class="card-img-top" alt="Shot 2">
          <div class="card-body">
            <h5 class="card-title">Creative Branding</h5>
            <p class="card-text">An innovative branding project to elevate a startup's image.</p>
            <a href="#" class="btn btn-outline-secondary">View More</a>
          </div>
        </div>
      </div>
     
      <div class="col">
        <div class="card shadow-sm border-0">
          <img src="4.jpeg" class="card-img-top" alt="Shot 3">
          <div class="card-body">
            <h5 class="card-title">Web Design Interface</h5>
            <p class="card-text">A modern and user-friendly interface for a new website.</p>
            <a href="#" class="btn btn-outline-secondary">View More</a>
          </div>
        </div>
      </div>
      
      <div class="col">
        <div class="card shadow-sm border-0">
          <img src="2.jpeg" class="card-img-top" alt="Shot 4">
          <div class="card-body">
            <h5 class="card-title">App UI Design</h5>
            <p class="card-text">A seamless and intuitive user interface for a mobile application.</p>
            <a href="#" class="btn btn-outline-secondary">View More</a>
          </div>
        </div>
      </div>
      
      <div class="col">
        <div class="card shadow-sm border-0">
          <img src="1.jpeg" class="card-img-top" alt="Shot 5">
          <div class="card-body">
            <h5 class="card-title">Minimalistic Poster</h5>
            <p class="card-text">A modern and clean poster design perfect for advertising.</p>
            <a href="#" class="btn btn-outline-secondary">View More</a>
          </div>
        </div>
      </div>
      
      <div class="col">
        <div class="card shadow-sm border-0">
          <img src="bg3.png" class="card-img-top" alt="Shot 6">
          <div class="card-body">
            <h5 class="card-title">Packaging Design</h5>
            <p class="card-text">A creative and innovative design for product packaging.</p>
            <a href="#" class="btn btn-outline-secondary">View More</a>
          </div>
        </div>
      </div>
    </div>
  </div>

  
  <footer class="bg-dark text-white text-center py-3">
    <p>&copy; 2024 Creative Showcase. Designed by dhashvanth b.</p>
  </footer>

  
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js"></script>

</body>
</html>
~~~
Signup.html
~~~
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sign Up Page</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            background: linear-gradient(45deg, #302f30, #020202);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            color: #fff;
        }
        .card {
            border-radius: 15px;
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.2);
            background: #fff;
            color: #000;
            width: 100%;
            max-width: 400px;
        }
        .card-header {
            text-align: center;
            font-size: 1.8rem;
            font-weight: bold;
            color: #fff;
            background-color: #2575fc;
            border-top-left-radius: 15px;
            border-top-right-radius: 15px;
            padding: 20px;
        }
        .form-control {
            border-radius: 8px;
            box-shadow: none;
        }
        .form-control:focus {
            border-color: #2575fc;
            box-shadow: 0 0 0 0.2rem rgba(37, 117, 252, 0.25);
        }
        .btn-primary {
            background-color: #2575fc;
            border: none;
            color: #fff;
            border-radius: 8px;
        }
        .btn-primary:hover {
            background-color: #1a5db4;
        }
        .text-center a {
            color: #2575fc;
            text-decoration: none;
        }
        .text-center a:hover {
            text-decoration: underline;
        }
        .card-body {
            padding: 30px;
        }
    </style>
</head>
<body>
    <div class="card">
        <div class="card-header">
            Sign Up
        </div>
        <div class="card-body">
            <form>
                <div class="mb-3">
                    <label for="fullName" class="form-label">Full Name</label>
                    <input type="text" class="form-control" id="fullName" placeholder="Enter your full name" required>
                </div>
                <div class="mb-3">
                    <label for="email" class="form-label">Email address</label>
                    <input type="email" class="form-control" id="email" placeholder="Enter your email" required>
                </div>
                <div class="mb-3">
                    <label for="password" class="form-label">Password</label>
                    <input type="password" class="form-control" id="password" placeholder="Enter your password" required>
                </div>
                <div class="mb-3">
                    <label for="confirmPassword" class="form-label">Confirm Password</label>
                    <input type="password" class="form-control" id="confirmPassword" placeholder="Confirm your password" required>
                </div>
                <button type="submit" class="btn btn-primary w-100 mt-3">Sign Up</button>
            </form>
        </div>
        <div class="text-center mt-3">
            <span>Already have an account? <a href="login.html" class="link">Login</a></span>
        </div>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

~~~
# OUTPUT:
![image](https://github.com/user-attachments/assets/f68f6396-c529-4447-9472-c9ce3720dcee)
![image](https://github.com/user-attachments/assets/c6dc4124-d740-4fef-b72f-91b4e266c3d5)

# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
