# Ex01 Portfolio
## Date: 14-05-2026

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ganesh Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
    scroll-behavior:smooth;
}

body{
    background:#0f172a;
    color:white;
}

/* NAVBAR */

nav{
    width:100%;
    padding:20px 10%;
    display:flex;
    justify-content:space-between;
    align-items:center;
    background:rgba(255,255,255,0.05);
    backdrop-filter:blur(10px);
    position:sticky;
    top:0;
    z-index:1000;
}

nav h1{
    color:#38bdf8;
}

nav ul{
    display:flex;
    list-style:none;
}

nav ul li{
    margin-left:25px;
}

nav ul li a{
    text-decoration:none;
    color:white;
    transition:0.3s;
}

nav ul li a:hover{
    color:#38bdf8;
}

/* HERO SECTION */

.hero{
    min-height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:40px;
    background:linear-gradient(135deg,#1e293b,#0f172a);
}

.hero-content img{
    width:180px;
    height:180px;
    border-radius:50%;
    border:5px solid #38bdf8;
    margin-bottom:20px;
    box-shadow:0 0 25px #38bdf8;
}

.hero-content h2{
    font-size:50px;
}

.hero-content h3{
    color:#38bdf8;
    margin:10px 0;
}

.hero-content p{
    max-width:700px;
    margin:auto;
    margin-top:15px;
    line-height:1.7;
}

.btn{
    display:inline-block;
    margin-top:20px;
    padding:12px 30px;
    background:#38bdf8;
    color:black;
    text-decoration:none;
    border-radius:30px;
    font-weight:bold;
    transition:0.4s;
}

.btn:hover{
    background:white;
    transform:scale(1.05);
}

/* SECTION */

section{
    padding:80px 10%;
}

.title{
    text-align:center;
    margin-bottom:50px;
    font-size:40px;
    color:#38bdf8;
}

/* ABOUT */

.about-container{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
    gap:30px;
}

.card{
    background:rgba(255,255,255,0.05);
    padding:30px;
    border-radius:20px;
    backdrop-filter:blur(10px);
    transition:0.4s;
    box-shadow:0 0 10px rgba(255,255,255,0.1);
}

.card:hover{
    transform:translateY(-10px);
    box-shadow:0 0 20px #38bdf8;
}

/* CERTIFICATES */

.certificates{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:30px;
}

.certificates a{
    text-decoration:none;
    color:white;
}

.certificates img{
    width:100%;
    border-radius:15px;
    transition:0.4s;
}

.certificates img:hover{
    transform:scale(1.05);
}

/* ACHIEVEMENTS */

.timeline{
    border-left:3px solid #38bdf8;
    padding-left:20px;
}

.timeline div{
    margin-bottom:30px;
}

/* CONTACT */

.contact-container{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
    gap:30px;
}

.contact-form input,
.contact-form textarea{
    width:100%;
    padding:15px;
    margin-bottom:15px;
    border:none;
    border-radius:10px;
    background:#1e293b;
    color:white;
}

.contact-form button{
    border:none;
    cursor:pointer;
}

.contact-links a{
    color:#38bdf8;
    text-decoration:none;
}

.contact-links a:hover{
    text-decoration:underline;
}

/* FOOTER */

footer{
    text-align:center;
    padding:20px;
    background:#020617;
    margin-top:50px;
}

</style>
</head>

<body>

<!-- NAVBAR -->

<nav>
    <h1>Portfolio</h1>

    <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#certificates">Certificates</a></li>
        <li><a href="#achievements">Achievements</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>

<!-- HERO -->

<section class="hero" id="home">

<div class="hero-content">

<img src="c:\Users\acer\OneDrive\Pictures\Screenshots\WhatsApp Image 2026-05-02 at 10.09.50 AM.jpeg" alt="Profile">

<h2>Ganesh Kanna</h2>

<h3>Data Scientist | Data Analyst</h3>

<p>
I am a first-year Artificial Intelligence and Data Science student with a strong interest in Data Science, AI, and modern technologies. I am continuously learning new skills and exploring innovative technologies to build my future career in the tech field.
</p>

<a href="#" class="btn">Download Resume</a>

</div>

</section>

<!-- ABOUT -->

<section id="about">

<h1 class="title">About Me</h1>

<div class="about-container">

<div class="card">
<h2>Education</h2>
<br>
<p>B.Tech Artificial Intelligence and Data Science</p>
<p>Saveetha Engineering College</p>
</div>

<div class="card">
<h2>Career Goal</h2>
<br>
<p>
To become a successful Data Scientist and develop intelligent AI-driven solutions using data analysis, machine learning, and innovative technologies.
</p>
</div>

<div class="card">
<h2>Personal Details</h2>
<br>
<p>Name : L Ganesh Kanna</p>
<p>Email : kannaganesh2008@gmail.com</p>
<p>Location : Chennai</p>
</div>

</div>

</section>

<!-- CERTIFICATES -->

<section id="certificates">

<h1 class="title">Certificates</h1>

<div class="certificates">

<div class="card">
<a href="c:\Users\acer\OneDrive\Pictures\Screenshots\notes\Screenshot 2026-05-10 213042.png" target="_blank">
<img src="c:\Users\acer\OneDrive\Pictures\Screenshots\notes\Screenshot 2026-05-10 213042.png">
</a>
<br><br>
<h3>Python for Data Science Free Course</h3>
</div>

<div class="card">
<a href="c:\Users\acer\OneDrive\Pictures\Screenshots\notes\Screenshot 2026-05-10 213142.png" target="_blank">
<img src="c:\Users\acer\OneDrive\Pictures\Screenshots\notes\Screenshot 2026-05-10 213142.png">
</a>
<br><br>
<h3>Mastering Arduino based automation system using Tinkercad</h3>
</div>

<div class="card">
<a href="c:\Users\acer\OneDrive\Pictures\Screenshots\notes\Screenshot 2026-05-10 213537.png" target="_blank">
<img src="c:\Users\acer\OneDrive\Pictures\Screenshots\notes\Screenshot 2026-05-10 213537.png">
</a>
<br><br>
<h3>Tamilnadu Robotics League</h3>
</div>

<div class="card">
<a href="c:\Users\acer\OneDrive\Pictures\Screenshots\notes\Screenshot 2026-05-10 213313.png" target="_blank">
<img src="c:\Users\acer\OneDrive\Pictures\Screenshots\notes\Screenshot 2026-05-10 213313.png">
</a>
<br><br>
<h3>Python Programming</h3>
</div>

<div class="card">
<a href="c:\Users\acer\OneDrive\Pictures\Screenshots\notes\Screenshot 2026-05-10 221641.png" target="_blank">
<img src="c:\Users\acer\OneDrive\Pictures\Screenshots\notes\Screenshot 2026-05-10 221641.png">
</a>
<br><br>
<h3>Embedded Treasure Hunt</h3>
</div>

<div class="card">
<a href="c:\Users\acer\OneDrive\Pictures\Screenshots\notes\Screenshot 2026-05-10 221935.png" target="_blank">
<img src="c:\Users\acer\OneDrive\Pictures\Screenshots\notes\Screenshot 2026-05-10 221935.png">
</a>
<br><br>
<h3>Justile League</h3>
</div>

<div class="card">
<a href="c:\Users\acer\OneDrive\Pictures\Screenshots\notes\Screenshot 2026-05-10 222204.png" target="_blank">
<img src="c:\Users\acer\OneDrive\Pictures\Screenshots\notes\Screenshot 2026-05-10 222204.png">
</a>
<br><br>
<h3>RTL RUSH</h3>
</div>

</div>

</section>

<!-- ACHIEVEMENTS -->

<section id="achievements">

<h1 class="title">Achievements</h1>

<div class="card timeline">

<div>
<h3>Tamilnadu Robotics League</h3>
<p>
Participated in the Tamilnadu Robotics League and gained practical exposure to robotics and teamwork.
</p>
</div>

<div>
<h3>EMBEDDED TREASURE HUNT</h3>
<p>
Participated in the Embedded Treasure Hunt and gained practical exposure to embedded systems and problem-solving.
</p>
</div>

<div>
<h3>RTL RUSH</h3>
<p>
Participated in the RTL RUSH and gained practical exposure to digital design and verification. I learned about logic gates and digital circuits.
</p>
</div>

<div>
<h3>Justice League</h3>
<p>
Participated in the Justice League event where I learned about self-confidence, public speaking, communication, and leadership skills.
</p>
</div>

</div>

</section>

<!-- CONTACT -->

<section id="contact">

<h1 class="title">Contact Me</h1>

<div class="contact-container">

<div class="card contact-links">

<h2>Contact Information</h2>

<br>

<p>Email : kannaganesh2008@gmail.com</p>
<p>Phone : +91 9876543210</p>

<p>
LinkedIn :
<a href="https://www.linkedin.com/in/l-ganesh-kanna-77351137a/" target="_blank">
View LinkedIn Profile
</a>
</p>

<p>
GitHub :
<a href="https://github.com/ganesh232008" target="_blank">
View GitHub Profile
</a>
</p>

</div>

<div class="card contact-form">

<input type="text" placeholder="Your Name">

<input type="email" placeholder="Your Email">

<textarea rows="5" placeholder="Your Message"></textarea>

<button class="btn">Send Message</button>

</div>

</div>

</section>

<!-- FOOTER -->

<footer>

<p>© 2026 Ganesh Portfolio | Designed with HTML & CSS</p>

</footer>

</body>
</html>

```

## OUTPUT


## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
