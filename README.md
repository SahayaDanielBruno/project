# Project Responsive Web Design using Bootstrap
# Date:23/12/2025
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
```
# Project.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smart up</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Raleway:wght@400;700&family=Roboto+Slab:wght@700&display=swap" rel="stylesheet">
    <style>
        .f1{
            font-family: 'Roboto Slab', serif;
            padding-left: 10px;
            margin-top: 27px;
        }
        
        body {
            background-color:beige;
        }

        .card {
            border: none;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
        }
        .card img {
    max-height: 180px;
    object-fit: cover;
    cursor: pointer;
    display: block;  
    width: 100%;    
    z-index: 1;  
}

        .card:hover {
            transform: scale(1.05);
            box-shadow: 0 4px 10px rgba(0,0,0,0.2);
        }
        .fade-in {
            opacity: 0;
            transform: translateY(20px);
            animation: fadeInUp 1s ease-out forwards;
        }
        @keyframes fadeInUp {
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        .gallery-title {
            text-align: center;
            margin: 50px;
            font-weight: bold;
        }
        .pagination .page-link {
            color: #343a40;
        }
        .pagination .page-item.active .page-link {
            background-color: #343a40;
            border-color: #343a40;
            color: #fff;
        }
        .i1{
            height: 70px;
            width: 100%;
            background-size: cover;
            
        }
        .about-us {
            background-color: #fff;
            padding: 2rem;
            margin-top: 2rem;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }
        .about-us h2 {
            text-align: center;
            margin-bottom: 1rem;
        }
        .about-us p {
            text-align: justify;
        }
    </style>
</head>
<body>
    <nav class="navbar navbar-dark bg-dark">
        <div class="container d-flex justify-content-between align-items-center">
            <div class="d-flex">
                <a class="navbar-brand me-3" href="#">
                    <img src="https://smartupindia.co/wp-content/uploads/2024/08/WHITE-Logo-scaled.webp" class="i1" />
                </a>
                <a class="nav-link text-light me-3 f1" href="#gallery">Gallery</a>
                <a class="nav-link text-light me-3 f1" href="#aboutUs">About Us</a>
            </div>
            <div>
                <a href="login.html" target="_blank"><button class="btn btn-outline-light" type="button">Login</button></a>
                <a href="signup.html" target="_blank"><button class="btn btn-outline-light" type="button">Sign Up</button></a>
            </div>
        </div>
    </nav>
    
    
     <header class="bg-dark text-light shadow pt-1 pb-1">
        <div class="gallery-title">
            <h2>Popular Now</h2>
        </div>
    </header>

    <div class="container">
        <div id="gallery"  class="row g-4">
            <div class="col-md-4 col-sm-6 col-lg-3 fade-in">
                <div class="card">
                    <img src="https://media.wired.com/photos/5fb70f2ce7b75db783b7012c/master/pass/Gear-Photos-597589287.jpg" class="i1">
                    <div class="card-body text-center">
                        <h5 class="card-title">Project 1</h5>
                        <p class="card-text text-muted">
                            <small>by Designer 1</small>
                        </p>
                    </div>
                </div>
            </div>
            
            <div class="col-md-4 col-sm-6 col-lg-3 fade-in" style="animation-delay: 0.4s;">
                <div class="card">
                    <img src="https://via.placeholder.com/300x180" class="card-img-top" alt="Placeholder">
                    <div class="card-body text-center">
                        <h5 class="card-title">Project 3</h5>
                        <p class="card-text text-muted">
                            <small>by Designer 3</small>
                        </p>
                    </div>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 col-lg-3 fade-in" style="animation-delay: 0.4s;">
                <div class="card">
                    <img src="https://via.placeholder.com/300x180" class="card-img-top" alt="Placeholder">
                    <div class="card-body text-center">
                        <h5 class="card-title">Project 4</h5>
                        <p class="card-text text-muted">
                            <small>by Designer 4</small>
                        </p>
                    </div>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 col-lg-3 fade-in" style="animation-delay: 0.4s;">
                <div class="card">
                    <img src="https://via.placeholder.com/300x180" class="card-img-top" alt="Placeholder">
                    <div class="card-body text-center">
                        <h5 class="card-title">Project 5</h5>
                        <p class="card-text text-muted">
                            <small>by Designer 5</small>
                        </p>
                    </div>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 col-lg-3 fade-in" style="animation-delay: 0.4s;">
                <div class="card">
                    <img src="https://via.placeholder.com/300x180" class="card-img-top" alt="Placeholder">
                    <div class="card-body text-center">
                        <h5 class="card-title">Project 6</h5>
                        <p class="card-text text-muted">
                            <small>by Designer 6</small>
                        </p>
                    </div>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 col-lg-3 fade-in" style="animation-delay: 0.4s;">
                <div class="card">
                    <img src="https://via.placeholder.com/300x180" class="card-img-top" alt="Placeholder">
                    <div class="card-body text-center">
                        <h5 class="card-title">Project 6</h5>
                        <p class="card-text text-muted">
                            <small>by Designer 7</small>
                        </p>
                    </div>
                </div>
            </div>
            <div class="col-md-4 col-sm-6 col-lg-3 fade-in" style="animation-delay: 0.4s;">
                <div class="card">
                    <img src="https://via.placeholder.com/300x180" class="card-img-top" alt="Placeholder">
                    <div class="card-body text-center">
                        <h5 class="card-title">Project 6</h5>
                        <p class="card-text text-muted">
                            <small>by Designer 8</small>
                        </p>
                    </div>
                </div>
            </div>

        </div>  
    </div>



    <nav aria-label="Page navigation" class="mt-4">
        <ul class="pagination justify-content-center">
            <li class="page-item">
                <button id="prevButton"  disabled></button>
            </li>
            <li class="page-item">
                <button id="nextButton" disabled></button>
            </li>
        </ul>
    </nav>    

    <div class="modal fade" id="lightboxModal" tabindex="-1" aria-labelledby="lightboxModalLabel" aria-hidden="true">
        <div class="modal-dialog modal-dialog-centered modal-lg">
            <div class="modal-content">
                <div class="modal-header">
                    <h5 class="modal-title" id="lightboxModalLabel">Image Preview</h5>
                    <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                </div>
                <div class="modal-body">
                    <img id="lightboxImage" src="" class="img-fluid w-100" alt="Enlarged Image">
                </div>
                <div class="modal-footer justify-content-between">
                    <button class="btn btn-secondary" onclick="navigateLightbox(-1)">Previous</button>
                    <button class="btn btn-secondary" onclick="navigateLightbox(1)">Next</button>
                </div>
            </div>
        </div>
    </div>
            <div class="about-us" id="aboutUs">
                <style>
                    .about-us {
                        font-family: 'Raleway', sans-serif;
                        padding: 50px 20px;
                        background-color:black ;
                        color: #f8f6f6;
                        text-align: center;
                    }
                    .about-us h2 {
                        font-family: 'Roboto Slab', serif;
                        font-size: 2.5rem;
                        margin-bottom: 20px;
                        color: #f5f5f5;
                    }
                    .about-us p {
                        font-size: 1.2rem;
                        line-height: 1.8;
                        margin-bottom: 20px;
                    }
                    .about-us img {
                        max-width: 100%;
                        height: auto;
                        border-radius: 10px;
                        margin-top: 30px;
                    }
                </style>
            
                <h2>About Us</h2>
                <p>
                    Smartup Visuals is a London-based visual communication and illustration studio specializing in animation, infographics, and live event scribing. Established in 2013, their team of experts assists companies in engaging target audiences by transforming complex information into memorable visuals.
                </p>
            </div>
            
    <footer class="bg-dark text-white text-center py-3 mt-4">
        <p>&copy; 2024 220056474 </p>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>

    <script>
        const cardsData = {
            1: [
                { title: "Project 1", designer: "Bivrin", likes: 1500, views: 300, imgSrc: "https://cdn.pixabay.com/photo/2017/02/08/17/24/fantasy-2049567_640.jpg" },
                { title: "Project 2", designer: "Winegar", likes: 1700, views: 450, imgSrc: "https://cdn.pixabay.com/photo/2021/08/25/20/42/field-6574455_640.jpg" },
                { title: "Project 3", designer: "Mihailova", likes: 2000, views: 500, imgSrc: "https://cdn.pixabay.com/photo/2018/01/12/14/24/night-3078326_640.jpg" },
                { title: "Project 4", designer: "Makris", likes: 900, views: 250, imgSrc: "https://cdn.pixabay.com/photo/2023/06/27/10/51/pier-8091934_640.jpg" },
                { title: "Project 5", designer: "Franklin", likes: 1200, views: 320, imgSrc: "https://cdn.pixabay.com/photo/2021/09/13/08/16/purple-flower-6620617_640.jpg" },
                { title: "Project 6", designer: "Zuidema", likes: 2500, views: 600, imgSrc: "https://cdn.pixabay.com/photo/2018/04/16/16/16/sunset-3325080_640.jpg" },
                { title: "Project 7", designer: "Asplund", likes: 2800, views: 690, imgSrc: "https://cdn.pixabay.com/photo/2018/08/14/13/23/ocean-3605547_640.jpg" },
                { title: "Project 8", designer: "Besliu", likes: 2750, views: 650, imgSrc: "https://cdn.pixabay.com/photo/2018/08/23/07/35/thunderstorm-3625405_640.jpg" },
            ],
        };
    
        let currentImageIndex = 0;
        const lightboxImages = [];
        let currentPage = 1;
        const totalPages = Object.keys(cardsData).length;
    
        function loadCards(page) {
            const gallery = document.getElementById('gallery');
            gallery.innerHTML = '';
    
            lightboxImages.length = 0;
    
            cardsData[page].forEach((card, index) => {
                lightboxImages.push(card.imgSrc);
                const cardHTML = `
                    <div class="col-md-4 col-sm-6 col-lg-3 fade-in">
                        <div class="card">
                            <img src="${card.imgSrc}" class="card-img-top" alt="${card.title}" onclick="openLightbox(${index})">
                            <div class="card-body text-center">
                                <h5 class="card-title">${card.title}</h5>
                                <p class="text-muted">by ${card.designer}</p>
                                <p>💖 ${card.likes} 👀 ${card.views}</p>
                            </div>
                        </div>
                    </div>
                `;
                gallery.insertAdjacentHTML('beforeend', cardHTML);
            });
        }
    
        function openLightbox(index) {
            currentImageIndex = index;
            document.getElementById('lightboxImage').src = lightboxImages[currentImageIndex];
            const lightboxModal = new bootstrap.Modal(document.getElementById('lightboxModal'));
            lightboxModal.show();
        }
    
        function navigateLightbox(step) {
            currentImageIndex = (currentImageIndex + step + lightboxImages.length) % lightboxImages.length;
            document.getElementById('lightboxImage').src = lightboxImages[currentImageIndex];
        }
    
        function changePage(direction) {
            currentPage += direction;
    
            document.getElementById('prevButton').disabled = currentPage === 1;
            document.getElementById('nextButton').disabled = currentPage === totalPages;
    
            loadCards(currentPage);
        }
    
        document.getElementById('prevButton').disabled = currentPage === 1;
        document.getElementById('nextButton').disabled = currentPage === totalPages;
    
        loadCards(currentPage);
    </script>
    
</body>
</html>
```
```
# login.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Login Page</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            background:bisque;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            color: #fff;
        }
        .card {
            border-radius: 20px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
            background: #fff;
            color: #000;
        }
        .card-header {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 10px;
            text-align: center;
            font-size: 1.5rem;
            font-weight: bold;
            color:cornflowerblue;
            background: #f8f9fa;
            border-top-left-radius: 20px;
            border-top-right-radius: 20px;
        }
        .card-header img {
            width: 30px;
            height: 30px;
        }
        .btn-primary {
            background-color: #000;
            border: none;
            color: #fff;
        }
        .btn-primary:hover {
            background-color: #333;
        }
        .form-control:focus {
            box-shadow: none;
            border-color: #000;
        }
        .link:hover {
            text-decoration: underline;
            color: #000;
        }
        .text-center a {
            color: #000;
        }
        .text-center a:hover {
            text-decoration: underline;
            color: #000;
        }
    </style>
</head>
<body>
    <div class="card p-4" style="width: 22rem;">
        <div class="card-header">
            Login
        </div>
        <div class="card-body">
            <form>
                <div class="mb-3">
                    <label for="email" class="form-label">Email address</label>
                    <input type="email" class="form-control" id="email" placeholder="Enter your email" required>
                </div>
                <div class="mb-3">
                    <label for="password" class="form-label">Password</label>
                    <input type="password" class="form-control" id="password" placeholder="Enter your password" required>
                </div>
                <div class="d-flex justify-content-between align-items-center">
                    <div>
                        <input type="checkbox" id="rememberMe">
                        <label for="rememberMe" class="form-label">Remember me</label>
                    </div>
                    <a href="#" class="text-decoration-none link">Forgot Password?</a>
                </div>
                <button type="submit" class="btn btn-primary w-100 mt-3">Login</button>
            </form>
        </div>
        <div class="text-center mt-3">
            <span>Don't have an account? <a href="signup.html" target="_blank" class="text-decoration-none link">Sign Up</a></span>
        </div>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```
```
# signup.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Interactive Sign Up Page</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <style>
        body {
            background:bisque;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            color: #fff;
        }
        .card {
            border-radius: 20px;
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
            background: #fff;
            color: #000;
        }
        .card-header {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 10px;
            text-align: center;
            font-size: 1.5rem;
            font-weight: bold;
            color:cornflowerblue;
            background: #f8f9fa;
            border-top-left-radius: 20px;
            border-top-right-radius: 20px;
        }
        .card-header img {
            width: 30px;
            height: 30px;
        }
        .btn-primary {
            background-color: #000;
            border: none;
            color: #fff;
        }
        .btn-primary:hover {
            background-color: #333;
        }
        .form-control:focus {
            box-shadow: none;
            border-color: #000;
        }
        .link:hover {
            text-decoration: underline;
            color: #000;
        }
        .text-center a {
            color: #000;
        }
        .text-center a:hover {
            text-decoration: underline;
            color: #000;
        }
    </style>
</head>
<body>
    <div class="card p-4" style="width: 22rem;">
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
            <span>Already have an account? <a href="login.html" target="_blank" class="text-decoration-none link">Login</a></span>
        </div>
    </div>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```
# OUTPUT:

![image](https://github.com/user-attachments/assets/44a53f9f-fc07-4143-918f-fcf81a7b1874)

![image](https://github.com/user-attachments/assets/09fd43ce-c5b1-4e24-998a-501098098f07)

![image](https://github.com/user-attachments/assets/8f5e801f-03e8-4710-ac26-907b3f49bacb)

![image](https://github.com/user-attachments/assets/bc8197ba-e135-4fc4-a6ba-981101238258)

# RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
