---
layout: home
title: "CortexEdu"
---

<style>
  body {
    font-family: 'Arial', sans-serif;
    background-color: #f0f4f8;
    margin: 0;
    padding: 0;
    color: #333;
  }
  h1, h2 {
    color: #007acc;
  }
  header {
    text-align: center;
    padding: 50px 20px;
    background-color: #fff;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
  }
  .container {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
  }
  .button {
    background-color: #007acc;
    color: white;
    padding: 15px 30px;
    text-align: center;
    display: inline-block;
    border-radius: 5px;
    text-decoration: none;
    transition: background-color 0.3s;
  }
  .button:hover {
    background-color: #005fa3;
  }
  footer {
    text-align: center;
    padding: 20px 0;
    background-color: #fff;
    box-shadow: 0 -2px 10px rgba(0, 0, 0, 0.1);
    margin-top: 50px;
  }
</style>

<header>
  <h1>Welcome to CortexEdu</h1>
  <p>Your gateway to knowledge and learning.</p>
  <a class="button" href="#sections">Explore Now</a>
</header>

<div class="container">
  <h2 id="sections">Explore Our Topics</h2>
  <ul>
    <li><a href="section1.md">🛠 Section 1: Basics of Coding</a></li>
    <li><a href="section2.md">📚 Section 2: Advanced Programming</a></li>
    <li><a href="section3.md">💡 Section 3: Resources and Tools</a></li>
    <li><a href="section4.md">🌐 Section 4: Web Development</a></li>
    <li><a href="section5.md">🚀 Section 5: Data Science</a></li>
  </ul>

  <h2>About CortexEdu</h2>
  <p>CortexEdu is dedicated to providing high-quality educational resources to help you succeed in your learning journey. This site is continuously being improved, with new content and resources added regularly.</p>
</div>

<footer>
  <p>&copy; 2024 CortexEdu. All rights reserved.</p>
  <p id="dateTime"></p>
</footer>

<script>
  function updateDateTime() {
    const now = new Date();
    const options = { 
      year: 'numeric', 
      month: 'long', 
      day: 'numeric', 
      hour: '2-digit', 
      minute: '2-digit', 
      second: '2-digit', 
      hour12: false 
    };
    const dateTimeString = now.toLocaleString(undefined, options);
    document.getElementById('dateTime').textContent = dateTimeString;
  }
  updateDateTime();
  setInterval(updateDateTime, 1000); // Update every second
</script>
