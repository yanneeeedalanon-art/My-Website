
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Yane | Personal Portfolio</title>

    <!-- Google Font: Poppins -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: #F3E8DC;
            color: #33271F;
            line-height: 1.7;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        .container {
            width: 90%;
            max-width: 1100px;
            margin: auto;
        }

        /* NAVIGATION */
        header {
            background: #FFFAF5;
            padding: 20px 0;
            border-bottom: 1px solid #E5D4C5;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            color: #765846;
            font-size: 25px;
            font-weight: 800;
        }

        .nav-links {
            display: flex;
            gap: 25px;
            list-style: none;
        }

        .nav-links a {
            color: #806F63;
            font-size: 14px;
            transition: 0.3s;
        }

        .nav-links a:hover {
            color: #765846;
        }

        /* HOME SECTION */
        .hero {
            min-height: 620px;
            display: grid;
            grid-template-columns: 1.2fr 0.8fr;
            align-items: center;
            gap: 50px;
            padding: 80px 0;
        }

        .eyebrow {
            color: #765846;
            font-weight: 700;
            letter-spacing: 3px;
            font-size: 13px;
            margin-bottom: 15px;
        }

        h1 {
            font-size: 65px;
            line-height: 1.2;
            margin-bottom: 15px;
        }

        h1 span {
            color: #765846;
        }

        .hero h2 {
            color: #765846;
            font-size: 22px;
            font-weight: 500;
            margin-bottom: 15px;
        }

        .hero p {
            color: #806F63;
            margin-bottom: 25px;
        }

        .btn {
            display: inline-block;
            padding: 12px 24px;
            border-radius: 6px;
            font-size: 14px;
            font-weight: 600;
            transition: 0.3s;
            margin-right: 10px;
        }

        .btn-primary {
            background: #765846;
            color: white;
        }

        .btn-primary:hover {
            background: #33271F;
        }

        .btn-outline {
            border: 1px solid #765846;
            color: #765846;
        }

        .btn-outline:hover {
            background: #765846;
            color: white;
        }

        /* PROFILE DESIGN */
        .hero-card {
            background: #FFFAF5;
            padding: 18px;
            border-radius: 18px;
            box-shadow: 0 15px 40px rgba(75, 52, 37, 0.10);
        }

        .portrait {
            min-height: 360px;
            background: linear-gradient(145deg, #DFC8B5, #B9957C);
            display: flex;
            justify-content: center;
            align-items: center;
            border-radius: 12px;
            color: white;
            text-align: center;
        }

        .portrait-mark {
            width: 110px;
            height: 110px;
            border: 2px solid white;
            border-radius: 50%;
            display: grid;
            place-items: center;
            font-size: 40px;
            margin: auto auto 15px;
        }

        /* GENERAL SECTIONS */
        section {
            padding: 85px 0;
        }

        .section-heading {
            text-align: center;
            margin-bottom: 45px;
        }

        .section-heading h2 {
            font-size: 38px;
            margin-bottom: 10px;
        }

        .section-heading p {
            color: #806F63;
        }

        /* ABOUT */
        .about {
            background: #FFFAF5;
        }

        .about-content {
            max-width: 790px;
            margin: auto;
            text-align: center;
            color: #806F63;
        }

        /* SKILLS */
        .skill-list {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 18px;
            max-width: 850px;
            margin: auto;
        }

        .skill {
            background: #FFFAF5;
            padding: 18px;
            border-radius: 8px;
            color: #765846;
            font-weight: 600;
            border-left: 4px solid #B18D75;
        }

        /* ACHIEVEMENTS */
        .cards {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 22px;
        }

        .card {
            background: #FFFAF5;
            padding: 28px;
            border-radius: 12px;
            transition: 0.3s;
        }

        .card:hover {
            transform: translateY(-6px);
            box-shadow: 0 10px 25px rgba(75, 52, 37, 0.10);
        }

        .card-number {
            color: #B18D75;
            font-size: 13px;
            font-weight: 700;
            margin-bottom: 12px;
        }

        .card h3 {
            color: #765846;
            margin-bottom: 10px;
        }

        .card p {
            color: #806F63;
            font-size: 14px;
        }

        /* CONTACT */
        .contact {
            background: #FFFAF5;
        }

        .contact-panel {
            max-width: 760px;
            margin: auto;
            text-align: center;
            padding: 40px;
            border-radius: 14px;
        }

        .contact-panel p {
            color: #806F63;
            margin: 15px 0 25px;
        }

        .contact-details {
            margin-top: 25px;
            color: #765846;
            font-size: 14px;
        }

        /* FOOTER */
        footer {
            background: #3D3028;
            color: #F3E8DC;
            text-align: center;
            padding: 22px;
            font-size: 13px;
        }

        /* RESPONSIVE DESIGN */
        @media (max-width: 760px) {
            nav {
                flex-direction: column;
                gap: 15px;
            }

            .nav-links {
                gap: 12px;
                flex-wrap: wrap;
                justify-content: center;
            }

            .hero {
                grid-template-columns: 1fr;
                text-align: center;
            }

            h1 {
                font-size: 45px;
            }

            .cards {
                grid-template-columns: 1fr;
            }

            .skill-list {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>

<body>

    <!-- NAVIGATION -->
    <header>
        <div class="container">
            <nav>
                <a href="#home" class="logo">YANE.</a>

                <ul class="nav-links">
                    <li><a href="#home">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#skills">Skills</a></li>
                    <li><a href="#achievements">Achievements</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- HOME -->
    <div class="container">
        <section class="hero" id="home">

            <div>
                <p class="eyebrow">PERSONAL PORTFOLIO</p>

                <h1>Hello, I'm <span>Yane.</span></h1>

                <h2>Aspiring Web Developer</h2>

                <p>
                    I am a passionate student who enjoys learning about
                    technology and creating clean, user-friendly websites.
                    I am committed to improving my skills and turning
                    creative ideas into meaningful digital experiences.
                </p>

                <a href="#contact" class="btn btn-primary">
                    Contact Me
                </a>

                <a href="#about" class="btn btn-outline">
                    Learn More
                </a>
            </div>

            <div class="hero-card">
                <div class="portrait">
                    <div>
                        <div class="portrait-mark">Y</div>
                        <h3>Aspiring Web Developer</h3>
                        <p style="color:white;">
                            Creative | Dedicated | Curious
                        </p>
                    </div>
                </div>
            </div>

        </section>
    </div>

    <!-- ABOUT -->
    <section class="about" id="about">
        <div class="container">

            <div class="section-heading">
                <p class="eyebrow">GET TO KNOW ME</p>
                <h2>About Me</h2>
            </div>

            <div class="about-content">
                <p>
                    I am an aspiring web developer with an interest in
                    designing and building websites. I enjoy exploring
                    new technologies, solving problems, and learning
                    through hands-on projects.

                    My goal is to become a skilled IT professional who
                    creates useful, accessible, and visually appealing
                    digital solutions. I believe that every project is
                    an opportunity to learn, grow, and improve.
                </p>
            </div>

        </div>
    </section>

    <!-- SKILLS -->
    <section id="skills">
        <div class="container">

            <div class="section-heading">
                <p class="eyebrow">WHAT I CAN DO</p>
                <h2>My Skills</h2>
                <p>Skills I am developing through my studies and practice.</p>
            </div>

            <div class="skill-list">
                <div class="skill">HTML - Webpage Structure</div>
                <div class="skill">CSS - Styling and Layout</div>
                <div class="skill">Basic Programming</div>
                <div class="skill">Problem-Solving</div>
                <div class="skill">Communication and Teamwork</div>
                <div class="skill">Time Management</div>
            </div>

        </div>
    </section>

    <!-- ACHIEVEMENTS -->
    <section id="achievements">
        <div class="container">

            <div class="section-heading">
                <p class="eyebrow">MY PROGRESS</p>
                <h2>Achievements & Projects</h2>
                <p>Experiences that reflect my learning and development.</p>
            </div>

            <div class="cards">

                <div class="card">
                    <p class="card-number">01 / LEARNING</p>
                    <h3>Web Development Studies</h3>
                    <p>
                        Learning the fundamentals of HTML and CSS
                        to create structured and attractive webpages.
                    </p>
                </div>

                <div class="card">
                    <p class="card-number">02 / PROJECT</p>
                    <h3>Personal Portfolio</h3>
                    <p>
                        Designed a personal website to present my
                        background, skills, goals, and achievements.
                    </p>
                </div>

                <div class="card">
                    <p class="card-number">03 / GROWTH</p>
                    <h3>Continuous Improvement</h3>
                    <p>
                        Building confidence through school activities,
                        practical tasks, and independent learning.
                    </p>
                </div>

            </div>
        </div>
    </section>

    <!-- CONTACT -->
    <section class="contact" id="contact">
        <div class="container">

            <div class="section-heading">
                <p class="eyebrow">LET'S CONNECT</p>
                <h2>Contact Me</h2>
            </div>

            <div class="contact-panel">
                <h3>Have a project or opportunity?</h3>

                <p>
                    I would be happy to connect, learn, and collaborate.
                    Feel free to reach out using my contact details below.
                </p>

                <a href="mailto:your.email@example.com"
                   class="btn btn-primary">
                    Send an Email
                </a>

                <div class="contact-details">
                    <p>Email: your.email@example.com</p>
                    <p>Location: Philippines</p>
                </div>
            </div>

        </div>
    </section>

    <!-- FOOTER -->
    <footer>
        <p>
            © 2026 Yane. All Rights Reserved.
            | Designed with HTML & CSS
        </p>
    </footer>

</body>
</html>

