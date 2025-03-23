# Projects
Html
<!DOCTYPE html>
<html>
<head>
    <title>Portfolio</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #84a6e9;
        }

        header {
            background-color: #941919;
            color: #fff;
            text-align: center;
            padding: 3rem 0;
            position: relative;
        }

        .header-content {
            position: relative;
        }

        .header-content h1 {
            font-size: 2.5rem;
            margin-top: 100px;
        }

        /* Profile Picture */
        .profile-picture {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            object-fit: cover;
            position: absolute;
            top: -75px;
            left: 100px;
            transform: translateX(-50%);
            border: 5px solid white;
        }

        nav {
            background-color: #333;
            color: #fff;
            text-align: center;
        }

        nav ul {
            list-style-type: none;
            padding: 0;
        }

        nav ul li {
            display: inline;
            margin: 0 20px;
        }

        nav ul li a {
            text-decoration: none;
            color: #fff;
        }

        .section-content {
            background-color: #fff;
            padding: 2rem;
            margin: 1rem;
            border-radius: 20px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            text-align: justify;
        }

        .download-button {
            background-color: #333;
            color: #fff;
            padding: 0.5rem 1rem;
            text-decoration: none;
            border-radius: 20px;
            display: inline-block;
            margin-top: 10px;
        }

        .download-button:hover {
            background-color: #555;
        }

        footer {
            text-align: center;
            padding: 1rem 0;
            background-color: #333;
            color: #fff;
        }

        ul {
            list-style-type: disc;
            padding-left: 20px;
        }
    </style>
</head>
<body>
    <header>
        <div class="header-content">
            <img src="paste your photo link" alt="Profile Picture" class="profile-picture">
            <h1>YOUR NAME</h1>
            <p>Computer Science Student</p>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="#about">About</a></li>
            <li><a href="#education">Education</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#resume">Resume</a></li>
        </ul>
    </nav>

    <section id="about">
        <div class="section-content">
            <h2>About Me</h2>
            <p>I am a Computer Science student at Bharathidasan University, passionate about programming, web development, and cybersecurity.</p>
        </div>
    </section>

    <section id="education">
        <div class="section-content">
            <h2>Education</h2>
            <p>Bachelor of Science (Computer Science) at Bharathidasan University (2023-2025)</p>
        </div>
    </section>

    <section id="skills">
        <div class="section-content">
            <h2>Skills</h2>
            <ul>
                <li>CyberSecurity</li>
                <li>Python</li>
                <li>Java</li>
                <li>PHP</li>
                <li>C++</li>
                <li>AI</li>
                <li>JavaScript</li>
            </ul>
        </div>
    </section>

    <section id="projects">
        <div class="section-content">
            <h2>Projects</h2>
            <ul>
                <li><a href="#">Digital Portfolio (HTML, CSS)</a></li>
                <li><a href="#">Tribute Page (HTML, CSS)</a></li>
            </ul>
        </div>
    </section>

    <section id="resume">
        <div class="section-content">
            <center>
                <h2>Resume</h2>
                <a href="paste your resume link" target="_blank" class="download-button">Download CV</a>
            </center>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 </p>
    </footer>

    <script>
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();

                const targetId = this.getAttribute('href').substring(1);
                const targetElement = document.getElementById(targetId);

                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop,
                        behavior: 'smooth'
                    });
                }
            });
        });
    </script>
</body>
</html>