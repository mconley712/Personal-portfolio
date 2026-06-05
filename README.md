# Personal-portfolio

```html
---
layout: default
title: Madison Conley
---

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Madison Conley | Portfolio</title>

    <style>
        *{
            margin:0;
            padding:0;
            box-sizing:border-box;
            font-family: Arial, sans-serif;
        }

        body{
            background:#f8f9fa;
            color:#333;
            line-height:1.6;
        }

        nav{
            background:#143d59;
            padding:1rem 5%;
            display:flex;
            justify-content:space-between;
            align-items:center;
        }

        nav h2{
            color:white;
        }

        nav ul{
            display:flex;
            list-style:none;
            gap:20px;
        }

        nav a{
            color:white;
            text-decoration:none;
            font-weight:bold;
        }

        .hero{
            display:flex;
            flex-wrap:wrap;
            align-items:center;
            justify-content:center;
            padding:80px 10%;
            gap:50px;
        }

        .hero-text{
            max-width:600px;
        }

        .hero h1{
            font-size:3rem;
            color:#143d59;
        }

        .hero p{
            margin-top:15px;
            font-size:1.1rem;
        }

        .hero-img img{
            width:320px;
            border-radius:15px;
            box-shadow:0 4px 12px rgba(0,0,0,.15);
        }

        .btn{
            display:inline-block;
            margin-top:20px;
            margin-right:10px;
            background:#143d59;
            color:white;
            padding:12px 24px;
            text-decoration:none;
            border-radius:6px;
        }

        section{
            padding:70px 10%;
        }

        h2{
            color:#143d59;
            margin-bottom:20px;
        }

        .card-grid{
            display:grid;
            grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
            gap:20px;
        }

        .card{
            background:white;
            padding:25px;
            border-radius:10px;
            box-shadow:0 2px 10px rgba(0,0,0,.1);
        }

        footer{
            text-align:center;
            padding:30px;
            background:#143d59;
            color:white;
        }
    </style>
</head>

<body>

<nav>
    <h2>Madison Conley</h2>

    <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#leadership">Leadership</a></li>
        <li><a href="#research">Research</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>

<section class="hero">

    <div class="hero-text">
        <h1>Madison Conley</h1>

        <h3>Computer Science Student | Student Leader | Researcher</h3>

        <p>
            Passionate about technology, leadership, and service.
            I enjoy solving problems, exploring cybersecurity,
            and creating meaningful opportunities for others through
            leadership and community involvement.
        </p>

        <a class="btn" href="/assets/files/resume.pdf" download>
            Download Resume
        </a>

        <a class="btn"
           href="https://www.linkedin.com/in/madison-conley-a137293aa"
           target="_blank">
            LinkedIn
        </a>
    </div>

    <div class="hero-img">
        <img src="/assets/images/headshot.jpg"
             alt="Madison Conley">
    </div>

</section>

<section id="about">

<h2>About Me</h2>

<p>
I'm a Computer Science student at Mississippi Valley State University
who believes growth comes from stepping outside your comfort zone,
embracing challenges, and remaining committed to your goals.

My passion for technology has led me to explore programming,
cybersecurity, and research while developing strong leadership
skills through service on campus and in the community.
</p>

</section>

<section id="leadership">

<h2>Leadership & Service</h2>

<div class="card-grid">

<div class="card">
<h3>Student Government Association</h3>
<p>Serving as a representative and advocating for student success.</p>
</div>

<div class="card">
<h3>Campus Activity Board</h3>
<p>Vice President helping plan events and enhance campus life.</p>
</div>

<div class="card">
<h3>Women in Science & Technology</h3>
<p>Secretary supporting women pursuing STEM careers.</p>
</div>

<div class="card">
<h3>NSBE</h3>
<p>Active member of the National Society of Black Engineers.</p>
</div>

</div>

</section>

<section id="research">

<h2>Research & Projects</h2>

<div class="card">
<h3>Cybersecurity & AI Research</h3>

<p>
Conducted undergraduate research examining Internet routing behavior,
route asymmetry, traceroute limitations, MPLS labels, and network
transparency challenges. Analyzed routing data and documented findings
through technical research reports.
</p>

</div>

</section>

<section id="contact">

<h2>Contact</h2>

<p><strong>Email:</strong> madisonconley15@gmail.com</p>

<p>
<strong>LinkedIn:</strong>
<a href="https://www.linkedin.com/in/madison-conley-a137293aa">
linkedin.com/in/madison-conley-a137293aa
</a>
</p>

</section>

<footer>
    <p>© 2026 Madison Conley. All Rights Reserved.</p>
</footer>

</body>
</html>
```
