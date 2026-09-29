#ips- collage -demo 
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Kartik Bandhoriya | Portfolio</title>

<style>
*{
  box-sizing:border-box;
  margin:0;
  padding:0;
}

body{
  font-family:Arial;
  background:#080b10;
  color:white;
  line-height:1.6;
}

nav{
  padding:18px 8%;
  display:flex;
  justify-content:space-between;
  background:#05070a;
  position:sticky;
  top:0;
  z-index:10;
}

nav a{
  color:white;
  text-decoration:none;
  margin-left:18px;
}

nav a:hover{
  color:#00e5ff;
}

section{
  padding:80px 8%;
  min-height:70vh;
}

.hero{
  min-height:90vh;
  display:flex;
  align-items:center;
  justify-content:space-between;
  gap:40px;
  background:linear-gradient(135deg,#080b10,#09232a);
}

h1{
  font-size:65px;
  line-height:1;
}

h1 span,h2 span{
  color:#00e5ff;
}

p{
  color:#aaa;
  margin:20px 0;
  max-width:600px;
}

.photo{
  width:300px;
  height:400px;
  border-radius:20px;
  overflow:hidden;
  border:2px solid #00e5ff;
}

.photo img{
  width:100%;
  height:100%;
  object-fit:cover;
}

.btn{
  display:inline-block;
  background:#00e5ff;
  color:#000;
  padding:12px 22px;
  border-radius:25px;
  text-decoration:none;
  font-weight:bold;
}

.card{
  background:#111820;
  border:1px solid #26313a;
  padding:25px;
  border-radius:15px;
  margin:15px 0;
}

.grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
  gap:20px;
}

.contact a{
  color:#00e5ff;
}

footer{
  text-align:center;
  padding:25px;
  background:#05070a;
  color:#777;
}

@media(max-width:700px){
  .hero{
    flex-direction:column-reverse;
    text-align:center;
  }

  h1{
    font-size:48px;
  }

  .photo{
    width:240px;
    height:320px;
  }

  nav{
    flex-direction:column;
    gap:10px;
  }

  nav a{
    font-size:13px;
  }
}
</style>
</head>

<body>

<nav>
<b>Kartik.</b>

<div>
<a href="#about">About</a>
<a href="#skills">Skills</a>
<a href="#projects">Projects</a>
<a href="#contact">Contact</a>
</div>
</nav>


<section class="hero">

<div>
<small>HELLO, I'M</small>

<h1>
Kartik<br>
<span>Bandhoriya</span>
</h1>

<p>
B.Tech CSIT student at IPS Academy, currently in second year,
interested in web development and technology.
</p>

<a class="btn" href="#contact">Contact Me</a>
</div>


<div class="photo">
<img src="profile.jpg" alt="Kartik Bandhoriya">
</div>

</section>


<section id="about">

<h2>About <span>Me</span></h2>

<div class="card">

<p>
I am Kartik Bandhoriya, a second-year B.Tech CSIT student
at IPS Academy. I am currently learning web development
and building my technical skills through practical projects.
</p>

<p>
My goal is to become a skilled developer and work on
real-world technology projects.
</p>

</div>

</section>


<section id="skills">

<h2>My <span>Skills</span></h2>

<div class="grid">

<div class="card">
<h3>HTML</h3>
<p>Creating structured and responsive web pages.</p>
</div>

<div class="card">
<h3>Learning</h3>
<p>Currently improving my web development skills.</p>
</div>

</div>

</section>


<section>

<h2>My <span>Education</span></h2>

<div class="card">

<h3>B.Tech CSIT</h3>

<p>IPS Academy, Indore</p>

<p>2025 - Present | Second Year</p>

</div>

</section>


<section id="projects">

<h2>My <span>Projects</span></h2>

<div class="card">

<h3>Personal Portfolio Website</h3>

<p>
A responsive portfolio website created using HTML
and CSS to showcase my skills and education.
</p>

</div>

</section>


<section id="contact" class="contact">

<h2>Let's <span>Connect</span></h2>

<div class="card">

<p>
📱 <a href="tel:6264750934">6264750934</a>
</p>

<p>
📧 <a href="mailto:kartikbandhoriya@gmail.com">
kartikbandhoriya@gmail.com
</a>
</p>

</div>

</section>


<footer>
© 2026 Kartik Bandhoriya
</footer>

</body>
</html>
