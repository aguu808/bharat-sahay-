<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Bharat Sahay 🇮🇳</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, sans-serif;
      background: #ffffff;
      color: #172033;
      line-height: 1.6;
    }

    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 18px 7%;
      background: white;
      border-bottom: 1px solid #eeeeee;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .logo {
      font-size: 22px;
      font-weight: 800;
      color: #172033;
    }

    .logo span {
      color: #138808;
    }

    nav a {
      text-decoration: none;
      color: #172033;
      margin-left: 22px;
      font-weight: 600;
      font-size: 14px;
    }

    nav a:hover {
      color: #138808;
    }

    .tricolour {
      height: 4px;
      background: linear-gradient(
        to right,
        #ff9933 33.3%,
        white 33.3%,
        white 66.6%,
        #138808 66.6%
      );
    }

    .hero {
      text-align: center;
      padding: 80px 20px 70px;
      background: linear-gradient(180deg, #fffaf5, #ffffff);
    }

    .flag {
      font-size: 55px;
      margin-bottom: 15px;
    }

    .hero h1 {
      font-size: clamp(38px, 7vw, 70px);
      margin-bottom: 15px;
      color: #172033;
    }

    .hero h1 span {
      color: #138808;
    }

    .hero p {
      max-width: 650px;
      margin: auto;
      color: #596273;
      font-size: 18px;
    }

    .search-box {
      max-width: 650px;
      margin: 35px auto 0;
      display: flex;
      background: white;
      border: 1px solid #dddddd;
      border-radius: 14px;
      padding: 7px;
      box-shadow: 0 8px 30px rgba(0,0,0,0.07);
    }

    .search-box input {
      flex: 1;
      border: none;
      outline: none;
      padding: 14px;
      font-size: 16px;
    }

    .search-box button {
      border: none;
      background: #138808;
      color: white;
      padding: 0 24px;
      border-radius: 10px;
      font-weight: bold;
      cursor: pointer;
    }

    .search-box button:hover {
      background: #0d6f06;
    }

    .section {
      max-width: 1100px;
      margin: auto;
      padding: 65px 20px;
    }

    .section-title {
      text-align: center;
      margin-bottom: 35px;
    }

    .section-title h2 {
      font-size: 32px;
      margin-bottom: 8px;
    }

    .section-title p {
      color: #697386;
    }

    .cards {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 20px;
    }

    .card {
      padding: 30px;
      border: 1px solid #eeeeee;
      border-radius: 18px;
      background: white;
      transition: 0.2s;
      cursor: pointer;
    }

    .card:hover {
      transform: translateY(-4px);
      box-shadow: 0 12px 30px rgba(0,0,0,0.08);
    }

    .icon {
      font-size: 38px;
      margin-bottom: 12px;
    }

    .card h3 {
      margin-bottom: 8px;
      font-size: 22px;
    }

    .card p {
      color: #697386;
    }

    .card a {
      display: inline-block;
      margin-top: 15px;
      color: #138808;
      font-weight: bold;
      text-decoration: none;
    }

    .card a:hover {
      text-decoration: underline;
    }

    /* EDUCATION RESOURCES */

    .education-box {
      background: #f7faf7;
      border-radius: 24px;
      padding: 35px;
      margin-top: 30px;
    }

    .education-box h3 {
      margin-bottom: 20px;
      font-size: 25px;
    }

    .education-list {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 18px;
    }

    .education-item {
      background: white;
      padding: 22px;
      border-radius: 16px;
      border: 1px solid #eeeeee;
      transition: 0.2s;
    }

    .education-item:hover {
      transform: translateY(-3px);
      box-shadow: 0 8px 20px rgba(0,0,0,0.06);
    }

    .education-item .resource-icon {
      font-size: 32px;
      margin-bottom: 8px;
    }

    .education-item strong {
      display: block;
      font-size: 19px;
      margin-bottom: 7px;
    }

    .education-item p {
      color: #697386;
      margin-bottom: 12px;
    }

    .resource-button {
      display: inline-block;
      background: #138808;
      color: white;
      padding: 9px 15px;
      border-radius: 9px;
      text-decoration: none;
      font-weight: bold;
      font-size: 14px;
    }

    .resource-button:hover {
      background: #0d6f06;
    }

    .official-note {
      text-align: center;
      margin-top: 22px;
      color: #697386;
      font-size: 13px;
    }

    .feature {
      background: #f7faf7;
      border-radius: 24px;
      padding: 45px;
      text-align: center;
    }

    .feature h2 {
      margin-bottom: 12px;
      font-size: 30px;
    }

    .feature p {
      max-width: 650px;
      margin: auto;
      color: #596273;
    }

    footer {
      margin-top: 30px;
      background: #172033;
      color: white;
      text-align: center;
      padding: 35px 20px;
    }

    footer p {
      color: #c9ced8;
      margin-top: 8px;
      font-size: 14px;
    }

    @media (max-width: 700px) {

      nav {
        padding: 15px 20px;
      }

      nav div:last-child {
        display: none;
      }

      .hero {
        padding: 60px 20px;
      }

      .hero p {
        font-size: 16px;
      }

      .search-box {
        flex-direction: column;
        gap: 7px;
      }

      .search-box button {
        padding: 13px;
      }

      .cards {
        grid-template-columns: 1fr;
      }

      .education-list {
        grid-template-columns: 1fr;
      }

      .education-box {
        padding: 25px 18px;
      }

      .feature {
        padding: 30px 20px;
      }
    }
  </style>
</head>

<body>

  <!-- NAVIGATION -->

  <nav>

    <div class="logo">
      🇮🇳 Bharat <span>Sahay</span>
    </div>

    <div>
      <a href="#home">Home</a>
      <a href="#resources">Resources</a>
      <a href="#education">Education</a>
      <a href="#about">About</a>
    </div>

  </nav>

  <div class="tricolour"></div>


  <!-- HERO -->

  <section class="hero" id="home">

    <div class="flag">🇮🇳</div>

    <h1>
      Bharat <span>Sahay</span>
    </h1>

    <p>
      Useful information, opportunities and resources —
      organized simply for people across India.
    </p>


    <!-- SEARCH -->

    <div class="search-box">

      <input
        type="text"
        id="searchInput"
        placeholder="What are you looking for?"
      >

      <button onclick="searchResources()">
        Search
      </button>

    </div>

  </section>


  <!-- MAIN RESOURCES -->

  <section class="section" id="resources">

    <div class="section-title">

      <h2>
        Explore Resources
      </h2>

      <p>
        Start with what you need.
      </p>

    </div>


    <div class="cards">


      <!-- EDUCATION -->

      <div class="card">

        <div class="icon">
          📚
        </div>

        <h3>
          Education
        </h3>

        <p>
          Study resources, learning materials and
          useful information for students.
        </p>

        <a href="#education">
          Explore →
        </a>

      </div>


      <!-- OPPORTUNITIES -->

      <div class="card">

        <div class="icon">
          🎓
        </div>

        <h3>
          Opportunities
        </h3>

        <p>
          Discover scholarships, competitions,
          programs and other opportunities.
        </p>

        <a href="#education">
          Explore →
        </a>

      </div>


      <!-- HELP -->

      <div class="card">

        <div class="icon">
          🆘
        </div>

        <h3>
          Help & Services
        </h3>

        <p>
          Find important services, support information
          and official resources.
        </p>

        <a href="#">
          Coming Soon →
        </a>

      </div>


      <!-- ENVIRONMENT -->

      <div class="card">

        <div class="icon">
          🌱
        </div>

        <h3>
          Environment
        </h3>

        <p>
          Learn simple ways to reduce waste,
          save resources and protect nature.
        </p>

        <a href="#">
          Coming Soon →
        </a>

      </div>

    </div>

  </section>


  <!-- EDUCATION -->

  <section class="section" id="education">

    <div class="section-title">

      <h2>
        📚 Education Resources
      </h2>

      <p>
        Access useful learning resources from official platforms.
      </p>

    </div>


    <div class="
