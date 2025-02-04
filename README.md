<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Portfolio</title>
    <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f5f5f5;
        }
        .left-panel {
            background-color: #2c3e50;
            color: white;
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 40px 0;
        }
        .left-panel img {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            margin-bottom: 20px;
        }
        .nav-links {
            display: flex;
            flex-direction: column;
            width: 100%;
            text-align: center;
        }
        .nav-links a {
            text-decoration: none;
            color: white;
            padding: 15px;
            display: block;
            transition: 0.3s;
        }
        .nav-links a:hover {
            background-color: #34495e;
        }
        .right-panel {
            padding: 40px;
        }
        .section-header i {
            margin-right: 10px;
        }
        .card {
            background: white;
            padding: 20px;
            margin-top: 20px;
            border-radius: 8px;
            box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
        }
        .skills-bar {
            display: none;
            width: 100%;
        }
        .bar {
            width: 100%;
            background-color: #ddd;
            border-radius: 5px;
            overflow: hidden;
        }
        .bar div {
            height: 20px;
            text-align: right;
            padding-right: 5px;
            line-height: 20px;
            color: white;
            background-color: #3498db;
        }
        .project-card {
            min-height: 250px;
            text-align: center;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            padding: 20px;
            background: white;
        }
        .skills-bar {
            display: none;
            width: 100%;
        }
        /* Colorful background for each project card */
        .project-card:nth-child(1) {
            background-color: #f39c12; /* Yellow */
            color: #fff;
        }
        .project-card:nth-child(2) {
            background-color: #1abc9c; /* Teal */
            color: #fff;
        }
        .project-card:nth-child(3) {
            background-color: #9b59b6; /* Purple */
            color: #fff;
        }
        .project-card:nth-child(4) {
            background-color: #e67e22; /* Orange */
            color: #fff;
        }
    </style>
</head>
<body data-spy="scroll" data-target="#navbar" data-offset="50">

    <div class="container-fluid d-flex">
        <!-- Left Panel -->
        <div class="left-panel col-md-3">
            <img src="myp.jpg" alt="Profile Picture">
            <div class="nav-links">
                <a href="#about" class="btn btn-dark">About Me</a>
                <a href="#projects" class="btn btn-dark">Projects</a>
                <a href="#contact" class="btn btn-dark">Contact Me</a>
            </div>
        </div>

        <!-- Right Panel -->
        <div class="right-panel col-md-9">
            <!-- Navbar -->
            <nav id="navbar" class="navbar navbar-expand-lg navbar-light bg-light sticky-top">
                <a class="navbar-brand" href="#">TDP Portfolio</a>
                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                    <span class="navbar-toggler-icon"></span>
                </button>
                <div class="collapse navbar-collapse" id="navbarNav">
                    <ul class="navbar-nav">
                        <li class="nav-item">
                            <a class="nav-link" href="#about">About Me</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#projects">Projects</a>
                        </li>
                        <li class="nav-item">
                            <a class="nav-link" href="#contact">Contact Me</a>
                        </li>
                    </ul>
                </div>
            </nav>

            <!-- About Me Section -->
            <h1 id="about">About Me</h1>
            <p>Hello, I’m Tridib Deb Pabel, a dedicated competitive programmer with a passion for solving complex problems and creating intuitive, high-performance web applications.</p>

            <!-- Education Section with Accordion -->
            <div class="card">
                <h2 class="section-header"><i class="fas fa-graduation-cap"></i> Education</h2>
                <div id="accordion">
                    <div class="card">
                        <div class="card-header" id="headingOne">
                            <h5 class="mb-0">
                                <button class="btn btn-link" data-toggle="collapse" data-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
                                    Bachelor of Science in Computer Science & Engineering
                                </button>
                            </h5>
                        </div>
                        <div id="collapseOne" class="collapse show" aria-labelledby="headingOne" data-parent="#accordion">
                            <div class="card-body">
                                Premier University Chittagong
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Technical Skills Section with Progress Bars -->
            <div class="card">
                <h2 class="section-header"><i class="fas fa-cogs"></i> Technical Skills</h2>
                <div class="card-body">
                    <div class="row">
                        <div class="col-md-4">
                            <h4>DSA</h4>
                            <div class="bar">
                                <div style="width: 70%">70%</div>
                            </div>
                        </div>
                        <div class="col-md-4">
                            <h4>HTML</h4>
                            <div class="bar">
                                <div style="width: 85%">85%</div>
                            </div>
                        </div>
                        <div class="col-md-4">
                            <h4>CSS</h4>
                            <div class="bar">
                                <div style="width: 80%">80%</div>
                            </div>
                        </div>
                        <div class="col-md-4">
                            <h4>JavaScript</h4>
                            <div class="bar">
                                <div style="width: 75%">75%</div>
                            </div>
                        </div>
                        <div class="col-md-4">
                            <h4>Bootstrap</h4>
                            <div class="bar">
                                <div style="width: 70%">70%</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Experience Section -->
            <div class="card">
                <h2 class="section-header"><i class="fas fa-briefcase"></i> Experience</h2>
                <p>Experienced in solving problems for 2 years.</p>
            </div>

            <!-- Achievements Section -->
            <div class="card">
                <h2 class="section-header"><i class="fas fa-trophy"></i> Achievements</h2>
                <h3>Online Judges</h3>
                <h4>Codeforces: <strong>ELSE_IF_TRIDIB21</strong></h4>
                <ul>
                    <li>Solved 700+ Problems</li>
                    <li>Max Rating: 1143</li>
                </ul>
                <h4>Codechef: <strong>tridib21</strong></h4>
                <ul>
                    <li>Solved 250+ Problems</li>
                    <li>Max Rating: 1506</li>
                </ul>
            </div>

            <!-- Projects Section with Carousel -->
            <h1 id="projects">Projects</h1>
            <div id="projectCarousel" class="carousel slide" data-ride="carousel">
                <div class="carousel-inner">
                    <div class="carousel-item active">
                        <div class="project-card">
                            <h3>Competitive Programming Problem Solver</h3>
                            <p>Developed a web app for practicing and solving competitive programming problems.</p>
                            <a href="#" class="btn btn-primary">Learn More</a>
                        </div>
                    </div>
                    <div class="carousel-item">
                        <div class="project-card">
                            <h3>Portfolio Website</h3>
                            <p>Designed and developed a personal portfolio website to showcase my skills and projects.</p>
                            <a href="#" class="btn btn-primary">Learn More</a>
                        </div>
                    </div>
    
                </div>
                <a class="carousel-control-prev" href="#projectCarousel" role="button" data-slide="prev">
                    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                    <span class="sr-only">Previous</span>
                </a>
                <a class="carousel-control-next" href="#projectCarousel" role="button" data-slide="next">
                    <span class="carousel-control-next-icon" aria-hidden="true"></span>
                    <span class="sr-only">Next</span>
                </a>
            </div>

            <!-- Contact Me Section -->
            <h1 id="contact">Contact Me</h1>
            <div class="alert alert-info" role="alert">
                Feel free to reach out to me through the contact form or email!
            </div>
            <form class="contact-form">
                <input type="text" class="form-control" placeholder="Your Name">
                <input type="email" class="form-control" placeholder="Your Email">
                <textarea class="form-control" placeholder="Your Message"></textarea>
                <button type="submit" class="btn btn-dark btn-block">Send Message</button>
            </form>

            <h3>Contact Information</h3>
            <ul class="list-unstyled">
                <li><i class="fas fa-phone"></i> <a href="tel:+1234567890">+880 1886560232</a></li>
                <li><i class="fas fa-envelope"></i> <a href="mailto:email@example.com">tridibdeb21@gmail.com</a></li>
                <li><i class="fas fa-map-marker-alt"></i> Chittagong, Bangladesh</li>
                <li><i class="fab fa-linkedin"></i> <a href="https://www.linkedin.com/in/tridib-deb-407048297" target="_blank">https://www.linkedin.com/in/tridib-deb-407048297</a></li>
            </ul>
        </div>
    </div>

    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.9.1/dist/umd/popper.min.js"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>
</html>
