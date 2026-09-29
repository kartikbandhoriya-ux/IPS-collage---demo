# IPS-collage---demo
This is my first get repository.
<br>
author - kartik bandhoriya 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Kartik Bandhoriya | Portfolio</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, sans-serif;
            background: #0a0a0a;
            color: #ffffff;
            line-height: 1.6;
        }

        nav {
            position: fixed;
            top: 0;
            width: 100%;
            padding: 18px 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: rgba(10,10,10,0.85);
            backdrop-filter: blur(10px);
            z-index: 1000;
            border-bottom: 1px solid #222;
        }

        .logo {
            font-size: 22px;
            font-weight: bold;
        }

        .logo span {
            color: #00e5ff;
        }

        nav ul {
            display: flex;
            gap: 25px;
            list-style: none;
        }

        nav a {
            color: #fff;
            text-decoration: none;
            transition: 0.3s;
        }

        nav a:hover {
            color: #00e5ff;
        }

        section {
            padding: 100px 8%;
            min-height: 100vh;
        }

        .hero {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: flex-start;
            background:
                radial-gradient(circle at 80% 30%, #003b45 0%, transparent 30%),
                #0a0a0a;
        }

        .hero small {
            color: #00e5ff;
            font-size: 16px;
            margin-bottom: 10px;
        }

        .hero h1 {
            font-size: clamp(45px, 8vw, 85px);
            line-height: 1;
            margin-bottom: 20px;
        }

        .hero h1 span {
            color: #00e5ff;
        }

        .hero p {
            max-width: 600px;
            color: #aaa;
            font-size: 19px;
            margin-bottom: 30px;
        }

        .btn {
            display: inline-block;
            padding: 13px 25px;
            background: #00e5ff;
            color: #000;
            text-decoration: none;
            border-radius: 30px;
            font-weight: bold;
            transition: 0.3s;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(0,229,255,0.25);
        }

        .section-title {
            font-size: 42px;
            margin-bottom: 40px;
        }

        .section-title span {
            color: #00e5ff;
        }

        .about {
            background: #0e0e0e;
        }

        .about-box {
            max-width: 800px;
            padding: 35px;
            border: 1px solid #252525;
            border-radius: 20px;
            background: #111;
        }

        .about-box p {
            color: #bbb;
            font-size: 18px;
        }

        .info {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }

        .info-card {
            padding: 25px;
            background: #151515;
            border: 1px solid #252525;
            border-radius: 15px;
        }

        .info-card h3 {
            color: #00e5ff;
            margin-bottom: 8px;
        }

        .skills {
            background: #0a0a0a;
        }

        .skill-card {
            width: 250px;
            padding: 30px;
            border-radius: 18px;
            background: #111;
            border: 1px solid #252525;
            transition: 0.3s;
        }

        .skill-card:hover {
            transform: translateY(-8px);
            border-color: #00e5ff;
        }

        .skill-card h3 {
            margin-bottom: 10px;
        }

        .skill-card p {
            color: #999;
        }

        .education {
            background: #0e0e0e;
        }

        .education-card {
            max-width: 700px;
            padding: 30px;
            background: #111;
            border-left: 4px solid #00e5ff;
            border-radius: 12px;
        }

        .education-card h3 {
            font-size: 24px;
            margin-bottom: 5px;
        }

        .education-card p {
            color: #aaa;
        }

        .contact {
            text-align: center;
        }

        .contact p {
            color: #aaa;
            margin-bottom: 25px;
        }

        footer {
            text-align: center;
            padding: 25px;
            background: #050505;
            color: #777;
            border-top: 1px solid #222;
        }

        @media (max-width: 700px) {
            nav {
                padding: 15px 5%;
            }

            nav ul {
                gap: 12px;
                font-size: 13px;
            }

            section {
                padding: 90px 6%;
            }

            .hero h1 {
                font-size: 52px;
            }

            .section-title {
                font-size: 34px;
            }

            .skill-card {
                width: 100%;
            }
        }
    </style>
</head>

<body>

    <!-- NAVBAR -->
    <nav>
        <div class="logo">Kartik<span>.</span></div>

        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#education">Education</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>


    <!-- HERO -->
    <section class="hero" id="home">

        <small>HELLO, I'M</small>

        <h1>
            Kartik<br>
            <span>Bandhoriya</span>
        </h1>

        <p>
            B.Tech CSIT student at IPS Academy,
            currently in my second year and interested
            in learning web development and technology.
        </p>

        <a href="#about" class="btn">Explore My Portfolio</a>

    </section>


    <!-- ABOUT -->
    <section class="about" id="about">

        <h2 class="section-title">
            About <span>Me</span>
        </h2>

        <div class="about-box">

            <p>
                I am Kartik Bandhoriya, a second-year
                B.Tech CSIT student at IPS Academy.
                I am currently developing my technical
                skills and exploring web development.
                My current skill is HTML, and I am
                continuously learning new technologies
                to improve my development abilities.
            </p>

            <div class="info">

                <div class="info-card">
                    <h3>Course</h3>
                    <p>B.Tech CSIT</p>
                </div>

                <div class="info-card">
                    <h3>Year</h3>
                    <p>Second Year</p>
                </div>

                <div class="info-card">
                    <h3>College</h3>
                    <p>IPS Academy</p>
                </div>

            </div>

        </div>

    </section>


    <!-- SKILLS -->
    <section class="skills" id="skills">

        <h2 class="section-title">
            My <span>Skills</span>
        </h2>

        <div class="skill-card">

            <h3>HTML</h3>

            <p>
                Creating structured and responsive
                web pages using HTML.
            </p>

        </div>

    </section>


    <!-- EDUCATION -->
    <section class="education" id="education">

        <h2 class="section-title">
            <span>Education</span>
        </h2>

        <div class="education-card">

            <h3>B.Tech CSIT</h3>

            <p>IPS Academy</p>

            <p>Currently studying in Second Year</p>

        </div>

    </section>


    <!--<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Kartik Bandhoriya | Portfolio</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, sans-serif;
            background: #0a0a0a;
            color: #ffffff;
            line-height: 1.6;
        }

        nav {
            position: fixed;
            top: 0;
            width: 100%;
            padding: 18px 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: rgba(10,10,10,0.85);
            backdrop-filter: blur(10px);
            z-index: 1000;
            border-bottom: 1px solid #222;
        }

        .logo {
            font-size: 22px;
            font-weight: bold;
        }

        .logo span {
            color: #00e5ff;
        }

        nav ul {
            display: flex;
            gap: 25px;
            list-style: none;
        }

        nav a {
            color: #fff;
            text-decoration: none;
            transition: 0.3s;
        }

        nav a:hover {
            color: #00e5ff;
        }

        section {
            padding: 100px 8%;
            min-height: 100vh;
        }

        .hero {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: flex-start;
            background:
                radial-gradient(circle at 80% 30%, #003b45 0%, transparent 30%),
                #0a0a0a;
        }

        .hero small {
            color: #00e5ff;
            font-size: 16px;
            margin-bottom: 10px;
        }

        .hero h1 {
            font-size: clamp(45px, 8vw, 85px);
            line-height: 1;
            margin-bottom: 20px;
        }

        .hero h1 span {
            color: #00e5ff;
        }

        .hero p {
            max-width: 600px;
            color: #aaa;
            font-size: 19px;
            margin-bottom: 30px;
        }

        .btn {
            display: inline-block;
            padding: 13px 25px;
            background: #00e5ff;
            color: #000;
            text-decoration: none;
            border-radius: 30px;
            font-weight: bold;
            transition: 0.3s;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(0,229,255,0.25);
        }

        .section-title {
            font-size: 42px;
            margin-bottom: 40px;
        }

        .section-title span {
            color: #00e5ff;
        }

        .about {
            background: #0e0e0e;
        }

        .about-box {
            max-width: 800px;
            padding: 35px;
            border: 1px solid #252525;
            border-radius: 20px;
            background: #111;
        }

        .about-box p {
            color: #bbb;
            font-size: 18px;
        }

        .info {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }

        .info-card {
            padding: 25px;
            background: #151515;
            border: 1px solid #252525;
            border-radius: 15px;
        }

        .info-card h3 {
            color: #00e5ff;
            margin-bottom: 8px;
        }

        .skills {
            background: #0a0a0a;
        }

        .skill-card {
            width: 250px;
            padding: 30px;
            border-radius: 18px;
            background: #111;
            border: 1px solid #252525;
            transition: 0.3s;
        }

        .skill-card:hover {
            transform: translateY(-8px);
            border-color: #00e5ff;
        }

        .skill-card h3 {
            margin-bottom: 10px;
        }

        .skill-card p {
            color: #999;
        }

        .education {
            background: #0e0e0e;
        }

        .education-card {
            max-width: 700px;
            padding: 30px;
            background: #111;
            border-left: 4px solid #00e5ff;
            border-radius: 12px;
        }

        .education-card h3 {
            font-size: 24px;
            margin-bottom: 5px;
        }

        .education-card p {
            color: #aaa;
        }

        .contact {
            text-align: center;
        }

        .contact p {
            color: #aaa;
            margin-bottom: 25px;
        }

        footer {
            text-align: center;
            padding: 25px;
            background: #050505;
            color: #777;
            border-top: 1px solid #222;
        }

        @media (max-width: 700px) {
            nav {
                padding: 15px 5%;
            }

            nav ul {
                gap: 12px;
                font-size: 13px;
            }

            section {
                padding: 90px 6%;
            }

            .hero h1 {
                font-size: 52px;
            }

            .section-title {
                font-size: 34px;
            }

            .skill-card {
                width: 100%;
            }
        }
    </style>
</head>

<body>

    <!-- NAVBAR -->
    <nav>
        <div class="logo">Kartik<span>.</span></div>

        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#education">Education</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>


    <!-- HERO -->
    <section class="hero" id="home">

        <small>HELLO, I'M</small>

        <h1>
            Kartik<br>
            <span>Bandhoriya</span>
        </h1>

        <p>
            B.Tech CSIT student at IPS Academy,
            currently in my second year and interested
            in learning web development and technology.
        </p>

        <a href="#about" class="btn">Explore My Portfolio</a>

    </section>


    <!-- ABOUT -->
    <section class="about" id="about">

        <h2 class="section-title">
            About <span>Me</span>
        </h2>

        <div class="about-box">

            <p>
                I am Kartik Bandhoriya, a second-year
                B.Tech CSIT student at IPS Academy.
                I am currently developing my technical
                skills and exploring web development.
                My current skill is HTML, and I am
                continuously learning new technologies
                to improve my development abilities.
            </p>

            <div class="info">

                <div class="info-card">
                    <h3>Course</h3>
                    <p>B.Tech CSIT</p>
                </div>

                <div class="info-card">
                    <h3>Year</h3>
                    <p>Second Year</p>
                </div>

                <div class="info-card">
                    <h3>College</h3>
                    <p>IPS Academy</p>
                </div>

            </div>

        </div>

    </section>


    <!-- SKILLS -->
    <section class="skills" id="skills">

        <h2 class="section-title">
            My <span>Skills</span>
        </h2>

        <div class="skill-card">

            <h3>HTML</h3>

            <p>
                Creating structured and responsive
                web pages using HTML.
            </p>

        </div>

    </section>


    <!-- EDUCATION -->
    <section class="education" id="education">

        <h2 class="section-title">
            <span>Education</span>
        </h2>

        <div class="education-card">

            <h3>B.Tech CSIT</h3>

            <p>IPS Academy</p>

            <p>Currently studying in Second Year</p>

        </div>

    </section>


    <!-- CONTACT -->
    <section class="contact" id="contact">

        <h2 class="section-title">
            Let's <span>Connect</span>
        </h2>

        <p>
            Interested in technology, web development
            and learning new skills.
        </p>

        <a href="mailto:your@email.com" class="btn">
            Contact Me
        </a>

    </section>


    <!-- FOOTER -->
    <footer>
        © 2026 Kartik Bandhoriya. All Rights Reserved.
    </footer>


</body>
</html><!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Kartik Bandhoriya | Portfolio</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, sans-serif;
            background: #0a0a0a;
            color: #ffffff;
            line-height: 1.6;
        }

        nav {
            position: fixed;
            top: 0;
            width: 100%;
            padding: 18px 8%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: rgba(10,10,10,0.85);
            backdrop-filter: blur(10px);
            z-index: 1000;
            border-bottom: 1px solid #222;
        }

        .logo {
            font-size: 22px;
            font-weight: bold;
        }

        .logo span {
            color: #00e5ff;
        }

        nav ul {
            display: flex;
            gap: 25px;
            list-style: none;
        }

        nav a {
            color: #fff;
            text-decoration: none;
            transition: 0.3s;
        }

        nav a:hover {
            color: #00e5ff;
        }

        section {
            padding: 100px 8%;
            min-height: 100vh;
        }

        .hero {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: flex-start;
            background:
                radial-gradient(circle at 80% 30%, #003b45 0%, transparent 30%),
                #0a0a0a;
        }

        .hero small {
            color: #00e5ff;
            font-size: 16px;
            margin-bottom: 10px;
        }

        .hero h1 {
            font-size: clamp(45px, 8vw, 85px);
            line-height: 1;
            margin-bottom: 20px;
        }

        .hero h1 span {
            color: #00e5ff;
        }

        .hero p {
            max-width: 600px;
            color: #aaa;
            font-size: 19px;
            margin-bottom: 30px;
        }

        .btn {
            display: inline-block;
            padding: 13px 25px;
            background: #00e5ff;
            color: #000;
            text-decoration: none;
            border-radius: 30px;
            font-weight: bold;
            transition: 0.3s;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(0,229,255,0.25);
        }

        .section-title {
            font-size: 42px;
            margin-bottom: 40px;
        }

        .section-title span {
            color: #00e5ff;
        }

        .about {
            background: #0e0e0e;
        }

        .about-box {
            max-width: 800px;
            padding: 35px;
            border: 1px solid #252525;
            border-radius: 20px;
            background: #111;
        }

        .about-box p {
            color: #bbb;
            font-size: 18px;
        }

        .info {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }

        .info-card {
            padding: 25px;
            background: #151515;
            border: 1px solid #252525;
            border-radius: 15px;
        }

        .info-card h3 {
            color: #00e5ff;
            margin-bottom: 8px;
        }

        .skills {
            background: #0a0a0a;
        }

        .skill-card {
            width: 250px;
            padding: 30px;
            border-radius: 18px;
            background: #111;
            border: 1px solid #252525;
            transition: 0.3s;
        }

        .skill-card:hover {
            transform: translateY(-8px);
            border-color: #00e5ff;
        }

        .skill-card h3 {
            margin-bottom: 10px;
        }

        .skill-card p {
            color: #999;
        }

        .education {
            background: #0e0e0e;
        }

        .education-card {
            max-width: 700px;
            padding: 30px;
            background: #111;
            border-left: 4px solid #00e5ff;
            border-radius: 12px;
        }

        .education-card h3 {
            font-size: 24px;
            margin-bottom: 5px;
        }

        .education-card p {
            color: #aaa;
        }

        .contact {
            text-align: center;
        }

        .contact p {
            color: #aaa;
            margin-bottom: 25px;
        }

        footer {
            text-align: center;
            padding: 25px;
            background: #050505;
            color: #777;
            border-top: 1px solid #222;
        }

        @media (max-width: 700px) {
            nav {
                padding: 15px 5%;
            }

            nav ul {
                gap: 12px;
                font-size: 13px;
            }

            section {
                padding: 90px 6%;
            }

            .hero h1 {
                font-size: 52px;
            }

            .section-title {
                font-size: 34px;
            }

            .skill-card {
                width: 100%;
            }
        }
    </style>
</head>

<body>

    <!-- NAVBAR -->
    <nav>
        <div class="logo">Kartik<span>.</span></div>

        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#education">Education</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>


    <!-- HERO -->
    <section class="hero" id="home">

        <small>HELLO, I'M</small>

        <h1>
            Kartik<br>
            <span>Bandhoriya</span>
        </h1>

        <p>
            B.Tech CSIT student at IPS Academy,
            currently in my second year and interested
            in learning web development and technology.
        </p>

        <a href="#about" class="btn">Explore My Portfolio</a>

    </section>


    <!-- ABOUT -->
    <section class="about" id="about">

        <h2 class="section-title">
            About <span>Me</span>
        </h2>

        <div class="about-box">

            <p>
                I am Kartik Bandhoriya, a second-year
                B.Tech CSIT student at IPS Academy.
                I am currently developing my technical
                skills and exploring web development.
                My current skill is HTML, and I am
                continuously learning new technologies
                to improve my development abilities.
            </p>

            <div class="info">

                <div class="info-card">
                    <h3>Course</h3>
                    <p>B.Tech CSIT</p>
                </div>

                <div class="info-card">
                    <h3>Year</h3>
                    <p>Second Year</p>
                </div>

                <div class="info-card">
                    <h3>College</h3>
                    <p>IPS Academy</p>
                </div>

            </div>

        </div>

    </section>


    <!-- SKILLS -->
    <section class="skills" id="skills">

        <h2 class="section-title">
            My <span>Skills</span>
        </h2>

        <div class="skill-card">

            <h3>HTML</h3>

            <p>
                Creating structured and responsive
                web pages using HTML.
            </p>

        </div>

    </section>


    <!-- EDUCATION -->
    <section class="education" id="education">

        <h2 class="section-title">
            <span>Education</span>
        </h2>

        <div class="education-card">

            <h3>B.Tech CSIT</h3>

            <p>IPS Academy</p>

            <p>Currently studying in Second Year</p>

        </div>

    </section>


    <!-- CONTACT -->
    <section class="contact" id="contact">

        <h2 class="section-title">
            Let's <span>Connect</span>
        </h2>

        <p>
            Interested in technology, web development
            and learning new skills.
        </p>

        <a href="mailto:your@email.com" class="btn">
            Contact Me
        </a>

    </section>


    <!-- FOOTER -->
    <footer>
        © 2026 Kartik Bandhoriya. All Rights Reserved.
    </footer>


</body>
</html> CONTACT -->
    <section class="contact" id="contact">

        <h2 class="section-title">
            Let's <span>Connect</span>
        </h2>

        <p>
            Interested in technology, web development
            and learning new skills.
        </p>

        <a href="mailto:your@email.com" class="btn">
            Contact Me
        </a>

    </section>


    <!-- FOOTER -->
    <footer>
        © 2026 Kartik Bandhoriya. All Rights Reserved.
    </footer>


</body>
</html>
