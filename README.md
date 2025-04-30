<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Medicine Career Overview</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #f9fafc;
      scroll-behavior: smooth;
    }

    header {
      background-color: #005f73;
      color: white;
      padding: 20px;
      text-align: center;
    }

    nav {
      background-color: #0a9396;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 10px;
      padding: 10px;
    }

    nav a {
      color: white;
      text-decoration: none;
      padding: 10px 15px;
      border-radius: 5px;
      background-color: #94d2bd;
      transition: background 0.3s;
    }

    nav a:hover {
      background-color: #ee9b00;
    }

    .container {
      max-width: 1000px;
      margin: auto;
      padding: 20px;
    }

    .section {
      margin-bottom: 40px;
      background: white;
      padding: 20px;
      border-radius: 12px;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
      opacity: 0;
      transform: translateY(30px);
      transition: opacity 0.6s ease-out, transform 0.6s ease-out;
    }

    .section.visible {
      opacity: 1;
      transform: translateY(0);
    }

    h2 {
      color: #005f73;
    }

    .section img {
      width: 100%;
      height: auto;
      border-radius: 8px;
      margin-top: 15px;
    }

    @media (max-width: 768px) {
      nav {
        flex-direction: column;
      }
    }
  </style>
</head>
<body>

<header>
  <h1>Medicine Career Overview</h1>
  <p>Explore the most important aspects of studying medicine</p>
</header>

<nav>
  <a href="#section1">Origin</a>
  <a href="#section2">Importance</a>
  <a href="#section3">Technology</a>
  <a href="#section4">Contributions</a>
  <a href="#section5">University Plans</a>
  <a href="#section6">Motivations</a>
  <a href="#section7">Skills</a>
  <a href="#section8">Top Universities</a>
  <a href="#section9">Postgraduate Programs</a>
</nav>

<div class="container">
  <div id="section1" class="section">
    <h2>1. Origin of the Career</h2>
    <p>Medicine originated in ancient civilizations like Egypt and Greece, with foundational figures such as Hippocrates and Galen setting early principles.</p>
    <img src="https://via.placeholder.com/800x400?text=Ancient+Medicine" alt="Ancient Medicine">
  </div>

  <div id="section2" class="section">
    <h2>2. Current Importance</h2>
    <p>Essential to public health, medicine saves lives, combats disease, and improves overall quality of life globally.</p>
    <img src="https://via.placeholder.com/800x400?text=Modern+Medicine" alt="Modern Medicine">
  </div>

  <div id="section3" class="section">
    <h2>3. Technological Development</h2>
    <p>Modern medicine uses AI, robotic surgery, genetic engineering, and advanced imaging to enhance diagnosis and treatment.</p>
    <img src="https://via.placeholder.com/800x400?text=Robotic+Surgery" alt="Robotic Surgery">
  </div>

  <div id="section4" class="section">
    <h2>4. Contributions to Humanity</h2>
    <p>From vaccines to organ transplants, medicine has vastly extended human lifespan and wellbeing.</p>
    <img src="https://via.placeholder.com/800x400?text=Medical+Contributions" alt="Medical Contributions">
  </div>

  <div id="section5" class="section">
    <h2>5. University Plans</h2>
    <p>Programs in medicine span undergraduate to postgraduate, with strong global partnerships and practical training.</p>
    <img src="https://via.placeholder.com/800x400?text=University+Programs" alt="University Programs">
  </div>

  <div id="section6" class="section">
    <h2>6. Reasons to Study</h2>
    <p>Desire to help others, interest in science, and making a real-world impact motivate many to pursue medicine.</p>
    <img src="https://via.placeholder.com/800x400?text=Reasons+to+Study" alt="Reasons to Study">
  </div>

  <div id="section7" class="section">
    <h2>7. Labor Market Skills</h2>
    <p>Professionals need critical thinking, empathy, communication skills, adaptability, and scientific knowledge.</p>
    <img src="https://via.placeholder.com/800x400?text=Medical+Skills" alt="Medical Skills">
  </div>

  <div id="section8" class="section">
    <h2>8. Best Universities</h2>
    <p>Top schools include Harvard, Oxford, and UNAM. Costs range from free (public) to over $60,000/year abroad.</p>
    <img src="https://via.placeholder.com/800x400?text=Top+Universities" alt="Top Universities">
  </div>

  <div id="section9" class="section">
    <h2>9. Postgraduate Programs</h2>
    <p>Available at Johns Hopkins, UBA, and other institutions offering master's, specialties, and doctoral research tracks.</p>
    <img src="https://via.placeholder.com/800x400?text=Postgraduate+Programs" alt="Postgraduate Programs">
  </div>
</div>

<script>
  const sections = document.querySelectorAll('.section');
  const observer = new IntersectionObserver(entries => {
    entries.forEach(entry => {
      if (entry.isIntersecting) {
        entry.target.classList.add('visible');
      }
    });
  }, {
    threshold: 0.2
  });

  sections.forEach(section => {
    observer.observe(section);
  });
</script>

</body>
</html>
