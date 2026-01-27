---
layout: default
title: Home
permalink: /
---

<style>
  .about-container {
    display: flex;
    align-items: flex-start;
    gap: 30px;
    margin-bottom: 30px;
    flex-wrap: nowrap;
  }
  .about-text {
    flex: 1;
    min-width: 0;
  }
  .about-image {
    flex: 0 0 400px;
    text-align: center;
    order: 2;
  }
  .about-image img {
    width: 100%;
    max-width: 400px;
    border-radius: 10px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  }
  .explore-section {
    margin-top: 40px;
    margin-bottom: 50px;
  }
  .welcome-title {
    text-align: center;
    font-size: 2em;
    font-weight: 700;
    margin-bottom: 30px;
    color: #333;
  }
  .cursor {
    animation: blink 1s infinite;
  }
  .explore-links {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    list-style: none;
    padding: 0;
    margin: 0;
  }
  .explore-links li {
    position: relative;
    height: 100%;
  }
  .explore-links a {
    display: flex;
    flex-direction: column;
    height: 100%;
    min-height: 140px;
    background: white;
    border-radius: 12px;
    padding: 25px;
    transition: all 0.3s ease;
    border: 2px solid rgba(102, 126, 234, 0.3);
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
    text-decoration: none;
    color: #000c3f;
    font-size: 1.4em;
    font-weight: bold;
  }
  .explore-links a:hover {
    background: linear-gradient(135deg, rgb(255, 255, 255), rgba(153, 37, 230, 0.25));
    transform: translateY(-20px);
    box-shadow: 0 8px 25px rgba(7, 4, 189, 0.46);
    border-color: rgba(102, 126, 234, 0.5);
  }
  .explore-links .link-title {
    display: block;
    margin-bottom: 10px;
  }
  .explore-links .link-description {
    display: block;
    color: #003972;
    font-size: 0.7em;
    font-weight: normal;
    margin-top: 8px;
  }
  @keyframes blink {
    0%, 50% { opacity: 1; }
    51%, 100% { opacity: 0; }
  }
  @media (max-width: 768px) {
    .about-container {
      flex-direction: column;
    }
    .about-image {
      flex: 0 0 auto;
      width: 100%;
      order: 1;
    }
    .explore-section h2 {
      font-size: 2em;
    }
    .explore-links {
      grid-template-columns: 1fr;
    }
  }
</style>

<div class="about-container">
  <div class="about-text">
    
    <h1 class="welcome-title">Welcome to a work in progress!</h1>
    
    <div class="explore-section">
      <ul class="explore-links">
        <li><a href="/projects"><span class="link-title">🚀 Projects</span><span class="link-description">Shelf of technical things</span></a></li>
        <li><a href="/research"><span class="link-title">🔬 Research</span><span class="link-description">Publications, working papers, and research interests</span></a></li>
        <li><a href="/work-experience"><span class="link-title">💼 Work Experience</span><span class="link-description">Places which paid for my work</span></a></li>
        <li><a href="/education"><span class="link-title">📚 Education</span><span class="link-description">Academic background and coursework</span></a></li>
      </ul>
    </div>

    <h2>About Me</h2>
    <p>
    I am pursuing a Master’s degree in Mech Engg at Georgia Tech, where I also earned my bachelors degree. During my undergraduate years, I explored a broad range of mechanical engineering disciplines through coursework, research, and student organizations. I've enjoyed my time dealing with the nuts and bolts of the mechanical world, but I've since pivoted to praying for covergence in the world of robotics. My research interests lies towards control systems, locomotion, manipulation, state estimation, optimization, and robot-focused mechanical design.
    </p>

    <p>
    I was born in Orlando, Florida, grew up in Tampa, and later lived in Hyderabad, India for 12 years where I did my schooling. I returned to the U.S. for college and now consider Georgia home.
    </p>

    <h2>Hobbies</h2>
    <p>
    My hobbies include swimming, basketball, squash, table tennis, rock climbing, chess, hiking, pool, movies, lifting ...pretty much anything physical.
    </p>



  </div>
  
  <div class="about-image">
    <img src="/assets/figures/facePic.png" alt="Profile Picture">
    
    <div style="margin-top: 20px; text-align: left; padding: 15px; background: #f8f9fa; border-radius: 10px;">
      <h3 style="margin-top: 0; font-size: 1.2em;">Contact</h3>
      <p style="margin: 10px 0;"><strong>Email:</strong><br>
      <a href="mailto:saaketh09@gmail.com">saaketh09@gmail.com</a> (personal)<br>
      <a href="mailto:saaketh@gatech.edu">saaketh@gatech.edu </a>(school)</p>
      
      <p style="margin: 10px 0;"><strong>Phone:</strong><br>
      <a href="tel:+17138858582">+1 (713) 885-8582</a></p>
      
      <p style="margin: 10px 0;"><strong>Connect:</strong><br>
      <a href="https://github.com/saakeechan" target="_blank">GitHub</a><br>
      <a href="https://www.linkedin.com/in/saakethcreddy/" target="_blank">LinkedIn</a></p>
      
      <p style="margin: 15px 0;"><a href="/cv" style="display: inline-block; padding: 10px 15px; background-color: #6967f7; color: white; text-decoration: none; border-radius: 5px; font-weight: bold; text-align: center;">📄 View C.V.</a></p>
    </div>
  </div>
</div>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const title = document.querySelector('.welcome-title');
  const lines = ["Hello! Welcome to", "a work in progress."];
  let lineIndex = 0;
  let charIndex = 0;
  let typedText = '';
  title.innerHTML = '<span class="cursor">|</span>';

  function typeWriter() {
    if (lineIndex < lines.length) {
      if (charIndex < lines[lineIndex].length) {
        typedText += lines[lineIndex].charAt(charIndex);
        title.innerHTML = typedText + '<span class="cursor">|</span>';
        charIndex++;
        setTimeout(typeWriter, 100);
      } else {
        if (lineIndex < lines.length - 1) {
          typedText += '<br>';
          title.innerHTML = typedText + '<span class="cursor">|</span>';
        }
        lineIndex++;
        charIndex = 0;
        setTimeout(typeWriter, 500);
      }
    } else {
      // Remove cursor after typing is done
      setTimeout(() => {
        title.innerHTML = typedText;
      }, 1000);
    }
  }

  typeWriter();

  // Optional: Click to restart
  title.addEventListener('click', function() {
    lineIndex = 0;
    charIndex = 0;
    typedText = '';
    title.innerHTML = '<span class="cursor">|</span>';
    typeWriter();
  });
});
</script>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const title = document.querySelector('.welcome-title');
  title.addEventListener('click', function() {
    this.style.animation = 'none';
    setTimeout(() => {
      this.style.animation = 'typing 3.5s steps(25, end), blink-caret 0.75s step-end infinite';
    }, 10);
  });
});
</script>
