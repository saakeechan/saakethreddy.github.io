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
    font-size: 2.5em;
    font-weight: 700;
    margin-bottom: 30px;
    color: #333;
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
    
    <h1 class="welcome-title">Hello! Welcome to my page</h1>
    
    <div class="explore-section">
      <ul class="explore-links">
        <li><a href="/education"><span class="link-title">📚 Education</span><span class="link-description">My academic background and coursework</span></a></li>
        <li><a href="/work-experience"><span class="link-title">💼 Work Experience</span><span class="link-description">Places I got paid for my work</span></a></li>
        <li><a href="/research"><span class="link-title">🔬 Research</span><span class="link-description">Publications, working papers, and research interests</span></a></li>
        <li><a href="/projects"><span class="link-title">🚀 Projects</span><span class="link-description">A showcase of projects I worked on</span></a></li>
      </ul>
    </div>

    <h2>About Me</h2>
    <p>
    I am currently pursuing a Master’s degree in Mechanical Engineering at the Georgia Institute of Technology, where my research interests center on control systems, autonomous robotics, state estimation, optimization, and robot-focused mechanical design. I also earned my bachelor’s degree in Mechanical Engineering from Georgia Tech.
    </p>

    <p>
    During my undergraduate years, I explored a broad range of mechanical engineering disciplines through coursework, research, and student organizations. Over time, this exploration converged into a strong interest in robotics and autonomous systems, which became clear during the summer of 2025. Since then, I have focused my work on the mathematical and control-theoretic foundations of robotic systems, guided by a strong preference for first-principles thinking.
    </p>

    <p>
    I was born in Orlando, Florida, grew up in Tampa, and later lived in Hyderabad, India until the age of 19. I returned to the U.S. for college and now consider Georgia home.
    </p>

    <h2>Hobbies</h2>
    <p>
    My hobbies include swimming, basketball, squash, table tennis, rock climbing, chess, hiking, pool, movies, lifting,.....(pretty much anything physical)
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
    </div>
  </div>
</div>
