# IPS-collage---demo
Kartik-Portfolio
│
├── index.html
│
└── profile.jpg
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <meta name="description"
        content="Kartik Bandhoriya - B.Tech CSIT student at IPS Academy and aspiring web developer.">

    <title>Kartik Bandhoriya | Portfolio</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        :root {
            --bg: #050505;
            --bg2: #0b0f10;
            --card: rgba(255, 255, 255, 0.04);
            --border: rgba(255, 255, 255, 0.10);
            --text: #ffffff;
            --muted: #a5a5a5;
            --accent: #00e5ff;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            background: var(--bg);
            color: var(--text);
            overflow-x: hidden;
        }

        /* Animated background */
        body::before {
            content: "";
            position: fixed;
            width: 500px;
            height: 500px;
            background: rgba(0, 229, 255, 0.08);
            filter: blur(100px);
            border-radius: 50%;
            top: 10%;
            right: -150px;
            z-index: -1;
            animation: glow 7s infinite alternate;
        }

        body::after {
            content: "";
            position: fixed;
            width: 400px;
            height: 400px;
            background: rgba(0, 100, 255, 0.06);
            filter: blur(100px);
            border-radius: 50%;
            bottom: 0;
            left: -150px;
            z-index: -1;
        }

        @keyframes glow {
            from {
                transform: translateY(0);
            }

            to {
                transform: translateY(80px);
            }
        }

        /* NAVBAR */

        nav {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            padding: 18px 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;

            background: rgba(5, 5, 5, 0.75);
            backdrop-filter: blur(15px);

            border-bottom: 1px solid var(--border);
            z-index: 1000;
        }

        .logo {
            font-size: 23px;
            font-weight: 800;
            letter-spacing: 1px;
        }

        .logo span {
            color: var(--accent);
        }

        nav ul {
            display: flex;
            gap: 25px;
            list-style: none;
        }

        nav ul li a {
            color: #ddd;
            text-decoration: none;
            font-size: 14px;
            transition: 0.3s;
        }

        nav ul li a:hover {
            color: var(--accent);
        }

        /* GENERAL */

        section {
            min-height: 100vh;
            padding: 110px 8%;
        }

        .section-title {
            font-size: clamp(35px, 5vw, 55px);
            margin-bottom: 45px;
        }

        .section-title span {
            color: var(--accent);
        }

        /* HERO */

        .hero {
            min-height: 100vh;

            display: flex;
            justify-content: space-between;
            align-items: center;

            gap: 70px;

            background:
                radial-gradient(circle at 80% 40%,
                    rgba(0, 229, 255, 0.10),
                    transparent 30%);

            padding-top: 130px;
        }

        .hero-content {
            max-width: 650px;
        }

        .hero small {
            color: var(--accent);
            font-size: 15px;
            letter-spacing: 4px;
            font-weight: bold;
        }

        .hero h1 {
            font-size: clamp(50px, 8vw, 90px);
            line-height: 0.95;
            margin: 18px 0 25px;
            letter-spacing: -3px;
        }

        .hero h1 span {
            color: var(--accent);
        }

        .hero p {
            color: var(--muted);
            font-size: 18px;
            line-height: 1.8;
            max-width: 600px;
            margin-bottom: 30px;
        }

        /* PROFILE IMAGE */

        .profile-image {
            width: 350px;
            height: 470px;

            border-radius: 25px;
            overflow: hidden;

            border: 1px solid rgba(255, 255, 255, 0.15);

            box-shadow:
                0 0 70px rgba(0, 229, 255, 0.10);

            transform: rotate(2deg);

            transition: 0.5s;
        }

        .profile-image:hover {
            transform: rotate(0deg) scale(1.02);
            box-shadow:
                0 0 90px rgba(0, 229, 255, 0.18);
        }

        .profile-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        /* BUTTONS */

        .hero-buttons {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-block;
            padding: 14px 25px;

            background: var(--accent);
            color: #000;

            text-decoration: none;
            border-radius: 30px;

            font-weight: bold;
            font-size: 14px;

            transition: 0.3s;
        }

        .btn:hover {
            transform: translateY(-4px);
            box-shadow: 0 10px 30px rgba(0, 229, 255, 0.25);
        }

        .btn.outline {
            background: transparent;
            color: var(--accent);
            border: 1px solid var(--accent);
        }

        .btn.outline:hover {
            background: var(--accent);
            color: #000;
        }

        /* ABOUT */

        .about {
            background: rgba(255, 255, 255, 0.015);
        }

        .about-box {
            max-width: 900px;

            padding: 40px;

            background: var(--card);
            border: 1px solid var(--border);

            border-radius: 25px;

            backdrop-filter: blur(10px);
        }

        .about-box p {
            color: #bdbdbd;
            font-size: 17px;
            line-height: 1.9;
        }

        /* INFO CARDS */

        .info {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
            margin-top: 30px;
        }

        .info-card {
            padding: 25px;

            background: rgba(255, 255, 255, 0.04);

            border: 1px solid var(--border);
            border-radius: 18px;

            transition: 0.3s;
        }

        .info-card:hover {
            transform: translateY(-5px);
            border-color: var(--accent);
        }

        .info-card h3 {
            color: var(--accent);
            margin-bottom: 8px;
            font-size: 15px;
        }

        .info-card p {
            color: white;
            font-size: 15px;
        }

        /* SKILLS */

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 20px;
        }

        .skill-card {
            padding: 30px;

            background: var(--card);
            border: 1px solid var(--border);

            border-radius: 20px;

            transition: 0.3s;
        }

        .skill-card:hover {
            transform: translateY(-8px);
            border-color: var(--accent);
        }

        .skill-icon {
            width: 55px;
            height: 55px;

            display: flex;
            justify-content: center;
            align-items: center;

            background: rgba(0, 229, 255, 0.10);

            border-radius: 15px;

            color: var(--accent);

            font-size: 25px;
            font-weight: bold;

            margin-bottom: 20px;
        }

        .skill-card h3 {
            margin-bottom: 8px;
        }

        .skill-card p {
            color: var(--muted);
            font-size: 14px;
            line-height: 1.7;
        }

        /* EDUCATION */

        .education {
            background: rgba(255, 255, 255, 0.015);
        }

        .education-card {
            max-width: 800px;

            padding: 35px;

            background: var(--card);

            border: 1px solid var(--border);
            border-left: 4px solid var(--accent);

            border-radius: 20px;
        }

        .education-card h3 {
            font-size: 26px;
            margin-bottom: 8px;
        }

        .education-card .college {
            color: var(--accent);
            font-size: 18px;
            margin-bottom: 10px;
        }

        .education-card p {
            color: var(--muted);
            margin-top: 5px;
        }

        /* PROJECTS */

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
        }

        .project-card {
            padding: 30px;

            background: var(--card);

            border: 1px solid var(--border);
            border-radius: 20px;

            transition: 0.3s;
        }

        .project-card:hover {
            transform: translateY(-8px);
            border-color: var(--accent);
        }

        .project-card h3 {
            font-size: 22px;
            margin-bottom: 12px;
        }

        .project-card p {
            color: var(--muted);
            line-height: 1.7;
            margin-bottom: 20px;
        }

        .project-tag {
            display: inline-block;

            padding: 6px 12px;

            background: rgba(0, 229, 255, 0.10);

            color: var(--accent);

            border-radius: 20px;

            font-size: 12px;
        }

        /* CONTACT */

        .contact {
            text-align: center;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
        }

        .contact p {
            color: var(--muted);
            max-width: 600px;
            line-height: 1.8;
            margin-bottom: 30px;
        }

        .contact-info {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
            margin-bottom: 30px;
        }

        .contact-item {
            padding: 15px 20px;

            background: var(--card);
            border: 1px solid var(--border);

            border-radius: 12px;

            color: #ddd;
            text-decoration: none;

            transition: 0.3s;
        }

        .contact-item:hover {
            border-color: var(--accent);
            color: var(--accent);
            transform: translateY(-3px);
        }

        /* FOOTER */

        footer {
            padding: 30px 8%;

            text-align: center;

            background: #020202;

            border-top: 1px solid var(--border);

            color: #777;

            font-size: 14px;
        }

        footer span {
            color: var(--accent);
        }

        /* MOBILE */

        @media (max-width: 850px) {

            nav {
                padding: 16px 5%;
            }

            nav ul {
                gap: 12px;
            }

            nav ul li a {
                font-size: 12px;
            }

            section {
                padding: 90px 6%;
            }

            .hero {
                flex-direction: column-reverse;
                text-align: center;
                justify-content: center;
                padding-top: 120px;
            }

            .hero-content {
                display: flex;
                flex-direction: column;
                align-items: center;
            }

            .hero h1 {
                letter-spacing: -2px;
            }

            .profile-image {
                width: 280px;
                height: 370px;
            }

            .info {
                grid-template-columns: 1fr;
            }

            .hero-buttons {
                justify-content: center;
            }
        }

        @media (max-width: 500px) {

            nav {
                flex-direction: column;
                gap: 10px;
            }

            nav ul {
                gap: 10px;
            }

            .hero h1 {
                font-size: 50px;
            }

            .hero p {
                font-size: 15px;
            }

            .profile-image {
                width: 240px;
                height: 320px;
            }

            .about-box {
                padding: 25px;
            }

            .section-title {
                font-size: 36px;
            }
        }

    </style>
</head>


<body>

    <!-- ================= NAVBAR ================= -->

    <nav>

        <div class="logo">
            Kartik<span>.</span>
        </div>

        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#education">Education</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>

    </nav>


    <!-- ================= HERO ================= -->

    <section class="hero" id="home">

        <div class="hero-content">

            <small>HELLO, I'M</small>

            <h1>
                Kartik<br>
                <span>Bandhoriya</span>
            </h1>

            <p>
                B.Tech CSIT student at IPS Academy, currently in my
                second year and interested in web development,
                technology and continuous learning.
            </p>

            <div class="hero-buttons">

                <a href="#about" class="btn">
                    Explore My Portfolio
                </a>

                <a href="#contact" class="btn outline">
                    Contact Me
                </a>

            </div>

        </div>


        <!-- YOUR PHOTO -->

        <div class="profile-image">

            <img
                src="profile.jpg"
                alt="Kartik Bandhoriya">

        </div>

    </section>


    <!-- ================= ABOUT ================= -->

    <section class="about" id="about">

        <h2 class="section-title">
            About <span>Me</span>
        </h2>

        <div class="about-box">

            <p>
                I am Kartik Bandhoriya, a second-year B.Tech CSIT
                student at IPS Academy. I am interested in technology
                and web development and currently building my
                foundation in HTML.
                <br><br>
                I enjoy learning through practical projects and
                improving my technical skills step by step.
                My goal is to build strong development skills,
                work on real-world projects and grow as a developer.
            </p>


            <div class="info">

                <div class="info-card">

                    <h3>COURSE</h3>

                    <p>
                        B.Tech CSIT
                    </p>

                </div>


                <div class="info-card">

                    <h3>YEAR</h3>

                    <p>
                        Second Year
                    </p>

                </div>


                <div class="info-card">

                    <h3>COLLEGE</h3>

                    <p>
                        IPS Academy
                    </p>

                </div>

            </div>

        </div>

    </section>


    <!-- ================= SKILLS ================= -->

    <section id="skills">

        <h2 class="section-title">
            My <span>Skills</span>
        </h2>


        <div class="skills-grid">

            <div class="skill-card">

                <div class="skill-icon">
                    HTML
                </div>

                <h3>HTML</h3>

                <p>
                    Creating structured web pages and
                    building the foundation of websites
                    using HTML.
                </p>

            </div>


            <!-- Future skill -->

            <div class="skill-card">

                <div class="skill-icon">
                    +
                </div>

                <h3>Currently Learning</h3>

                <p>
                    Continuously learning new technologies
                    and improving my web development skills.
                </p>

            </div>

        </div>

    </section>


    <!-- ================= EDUCATION ================= -->

    <section class="education" id="education">

        <h2 class="section-title">
            My <span>Education</span>
        </h2>


        <div class="education-card">

            <h3>
                Bachelor of Technology
            </h3>

            <div class="college">
                Computer Science & Information Technology
            </div>

            <p>
                <strong>IPS Academy, Indore</strong>
            </p>

            <p>
                2025 - Present
            </p>

            <p>
                Currently studying in Second Year
            </p>

        </div>

    </section>


    <!-- ================= PROJECTS ================= -->

    <section id="projects">

        <h2 class="section-title">
            My <span>Projects</span>
        </h2>


        <div class="projects-grid">


            <!-- PROJECT 1 -->

            <div class="project-card">

                <h3>
                    Personal Portfolio Website
                </h3>

                <p>
                    A responsive personal portfolio website
                    created to showcase my education, skills,
                    projects and contact information.
                </p>

                <span class="project-tag">
                    HTML
                </span>

            </div>


            <!-- PROJECT 2 -->

            <div class="project-card">

                <h3>
                    More Projects Coming
                </h3>

                <p>
                    I am currently learning and working on
                    new projects. More practical projects
                    will be added here as I build them.
                </p>

                <span class="project-tag">
                    Learning
                </span>

            </div>


        </div>

    </section>


    <!-- ================= CONTACT ================= -->

    <section class="contact" id="contact">

        <h2 class="section-title">
            Let's <span>Connect</span>
        </h2>

        <p>
            Interested in technology, web development and
            learning new skills? Feel free to connect with me.
        </p>


        <div class="contact-info">


            <!-- PHONE -->

            <a
                class="contact-item"
                href="tel:6264750934">

                📱 6264750934

            </a>


            <!-- EMAIL -->

            <a
                class="contact-item"
                href="mailto:kartikbandhoriya@gmail.com">

                📧 kartikbandhoriya@gmail.com

            </a>


        </div>


        <!-- EMAIL BUTTON -->

        <a
            href="mailto:kartikbandhoriya@gmail.com"
            class="btn">

            Send Me an Email

        </a>

    </section>


    <!-- ================= FOOTER ================= -->

    <footer>

        © 2026
        <span>Kartik Bandhoriya</span>.
        All Rights Reserved.

    </footer>


</body>

</html>
