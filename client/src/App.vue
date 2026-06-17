<script setup>
import hero from './assets/hero.png'
</script>
<template>
  <div class="container">

    <nav>
      <h2 class="logo">Khushi Portfolio</h2>

      <ul>
        <li><a href="#home">Home</a></li>
<li><a href="#about">About</a></li>
<li><a href="#projects">Projects</a></li>
<li><a href="#contact">Contact</a></li>
      </ul>
    </nav>

    <section id="home" class="hero">
    <img :src="hero" alt="hero image" class="hero-img">
  <h1>Creative Web Developer</h1>
  <p>I build modern, responsive and user-friendly websites.</p>
  <p>Passionate CSE Student | Learning Web Development</p>
  <button>Hire Me</button>
  <button>Download Resume</button>
 <div class="social-links">
    <button>GitHub</button>
  <button>LinkedIn</button>
</div>
</section>

    <section id="about">
      <h2>About Me</h2>
      <p>
        I am learning Web Development and building modern websites.
      </p>
    </section>
<section id="skills">
  <h2>My Skills</h2>

  <div class="skills">
    <span>HTML</span>
    <span>CSS</span>
    <span>JavaScript</span>
    <span>Vue.js</span>
    <span>C Programming</span>
    <span>Git & GitHub</span>
  </div>
</section>
    <section id="projects">
      <h2>Projects</h2>

      <div class="card">
      <img :src="hero" class="project-img">
        <h3>Student Management System</h3>
<p>Manage student records efficiently.</p>
<p>Built with HTML, CSS and JavaScript</p>
<button>View Project</button>
      </div>

      <div class="card">
      <img :src="hero" class="project-img">
       <h3>Restaurant Website</h3>
<p>Modern restaurant landing page.</p>
<p>Built with Vue.js and CSS</p>
<button>View Project</button>
      </div>
    </section>

   <section id="contact">
      <h2>Contact</h2>
<p>Email: khushimangal@gmail.com</p>
      <input placeholder="Your Name" />
      <br><br>

      <input placeholder="Your Email" />
      <br><br>

      <textarea placeholder="Message"></textarea>
      <br><br>

      <button>Send message</button>
    </section>

 <footer>
  <p>© 2026 Khushi Portfolio | All Rights Reserved</p>
</footer>
 </div>
</template>

<style>
body{
  margin:0;
  font-family:Arial;
  background:black;
  color:white;
}

.container{
  padding:20px;
   max-width:1000px;
  margin:auto;
}

nav{
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:15px;
border-bottom:1px solid skyblue;
position: sticky;
top: 0;
background: black;
}

ul{
  display:flex;
  gap:20px;
  list-style:none;
}
li:hover{
  color:skyblue;
  cursor:pointer;
}
.hero{
   text-align:center;
  margin-top:60px;
  padding:30px;
  border:1px solid skyblue;
  border-radius:15px;
}
.hero h1{
  font-size:50px;
  color:skyblue;
  text-shadow: 0 0 15px skyblue;
}

button{
  background:skyblue;
  border:none;
  padding:12px 25px;
  cursor:pointer;
  border-radius:8px;
  font-size:16px;
}
  button:hover{
  transform: scale(1.1);
}

.card{
  border:1px solid skyblue;
  padding:20px;
  margin:15px 0;
  border-radius:12px;
  box-shadow: 0 0 10px skyblue;
}
.card:hover{
  transform: scale(1.03);
}
input,textarea{
  width:300px;
  padding:10px;
}
section{
  margin-top:50px;
}

h2{
  color:skyblue;
}
.hero-img{
  width:350px;
  margin-bottom:20px;
  animation: float 3s ease-in-out infinite;
}
  @keyframes float{
  0%{
    transform: translateY(0px);
  }

  50%{
    transform: translateY(-15px);
  }

  100%{
    transform: translateY(0px);
  }
}
footer{
  text-align:center;
  margin-top:50px;
  padding:20px;
  border-top:1px solid skyblue;
}
.logo{
  color:skyblue;
  text-shadow:0 0 10px skyblue;
}
html{
  scroll-behavior:smooth;
}

*{
  transition:0.3s;
}
a{
  text-decoration:none;
  color:white;
}

html{
  scroll-behavior:smooth;
}
.card{
  transition:0.3s;
}

.card:hover{
  transform:translateY(-10px);
}
button{
  margin:10px;
}
.skills{
  display:flex;
  flex-wrap:wrap;
  gap:15px;
  margin-top:20px;
}

.skills span{
  border:1px solid skyblue;
  padding:10px 20px;
  border-radius:20px;
  box-shadow:0 0 10px skyblue;
  transition:0.3s;
}

.skills span:hover{
  transform:scale(1.1);
}
input,
textarea{
  background:#111;
  color:white;
  border:1px solid skyblue;
  border-radius:10px;
  box-shadow:0 0 10px skyblue;
}

input:focus,
textarea:focus{
  outline:none;
  box-shadow:0 0 20px skyblue;
}
.project-img{
  width:100%;
  max-width:400px;
  border-radius:15px;
  margin-bottom:15px;
  box-shadow:0 0 15px skyblue;
}
@media (max-width:768px){

  nav{
    flex-direction:column;
    gap:15px;
  }

  ul{
    flex-direction:column;
    align-items:center;
    padding:0;
  }

  .hero h1{
    font-size:32px;
  }

  .hero-img{
    width:220px;
  }

  input,
  textarea{
    width:90%;
  }

  .container{
    padding:10px;
  }
}
.social-links{
  margin-top:20px;
}

.social-links button{
  margin:10px;
}
button{
  background:linear-gradient(45deg, #00c6ff, #0072ff);
  color:white;
  font-weight:bold;
}

button:hover{
  box-shadow:0 0 20px skyblue;
}
</style>