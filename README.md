<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title> Gaming Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&display=swap" rel="stylesheet">

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

body{
    font-family:'Orbitron',sans-serif;
    background:#050510;
    color:white;
    overflow-x:hidden;
}

body::before{
    content:"";
    position:fixed;
    width:100%;
    height:100%;
    background:
    radial-gradient(circle at 20% 20%, rgba(0,255,255,.12), transparent 30%),
    radial-gradient(circle at 80% 80%, rgba(255,0,255,.12), transparent 30%);
    z-index:-1;
}

nav{
    position:fixed;
    top:0;
    width:100%;
    padding:20px;
    display:flex;
    justify-content:center;
    gap:30px;
    background:rgba(0,0,0,.6);
    backdrop-filter:blur(10px);
}

nav a{
    color:#00ffff;
    text-decoration:none;
}

.hero{
    min-height:100vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
    padding:20px;
}

.hero h1{
    font-size:4rem;
    text-shadow:0 0 20px cyan;
}

.hero p{
    margin:20px 0;
    max-width:700px;
}

.btn{
    display:inline-block;
    padding:14px 30px;
    background:transparent;
    border:2px solid cyan;
    color:cyan;
    text-decoration:none;
    border-radius:40px;
    box-shadow:0 0 20px cyan;
}

section{
    padding:100px 10%;
}

.section-title{
    text-align:center;
    font-size:2.5rem;
    color:cyan;
    margin-bottom:40px;
}

.grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
    gap:25px;
}

.card{
    background:rgba(255,255,255,.05);
    border:1px solid rgba(0,255,255,.3);
    padding:25px;
    border-radius:15px;
    transition:.4s;
}

.card:hover{
    transform:translateY(-10px);
    box-shadow:0 0 25px cyan;
}

.skills{
    display:flex;
    flex-wrap:wrap;
    justify-content:center;
    gap:15px;
}

.skill{
    padding:12px 20px;
    border:1px solid cyan;
    border-radius:30px;
}

.contact{
    text-align:center;
}

footer{
    text-align:center;
    padding:25px;
    border-top:1px solid rgba(255,255,255,.1);
}
</style>
</head>

<body>

<nav>
    <a href="#about">About</a>
    <a href="#projects">Projects</a>
    <a href="#skills">Skills</a>
    <a href="#contact">Contact</a>
</nav>

<section class="hero">
    <h1>YOUR NAME</h1>
    <p>Game Developer • YouTuber • Creative Designer</p>
    <a href="#projects" class="btn">Explore Projects</a>
</section>

<section id="about">
    <h2 class="section-title">About Me</h2>
    <div class="card">
        <p>
            I create games, gaming content, and digital experiences.
            Passionate about Unity, Unreal Engine, storytelling,
            and immersive gameplay.
        </p>
    </div>
</section>

<section id="projects">
    <h2 class="section-title">Projects</h2>

    <div class="grid">
        <div class="card">
            <h3>Zombie Apocalypse</h3>
            <p>Open-world survival game with advanced AI enemies.</p>
        </div>

        <div class="card">
            <h3>Cyber Racer</h3>
            <p>Fast-paced futuristic racing game.</p>
        </div>

        <div class="card">
            <h3>Fantasy Kingdom</h3>
            <p>Action RPG with quests and exploration.</p>
        </div>
    </div>
</section>

<section id="skills">
    <h2 class="section-title">Skills</h2>

    <div class="skills">
        <div class="skill">Unity</div>
        <div class="skill">Unreal Engine</div>
        <div class="skill">C#</div>
        <div class="skill">C++</div>
        <div class="skill">Blender</div>
        <div class="skill">Photoshop</div>
        <div class="skill">Video Editing</div>
        <div class="skill">Game Design</div>
    </div>
</section>

<section id="contact">
    <h2 class="section-title">Contact</h2>

    <div class="contact">
        <p>Email: your@email.com</p>
        <p>YouTube: Your Channel</p>
        <p>Instagram: @yourname</p>
    </div>
</section>

<footer>
    © 2026 Your Name | Gaming Portfolio
</footer>

</body>
</html>
