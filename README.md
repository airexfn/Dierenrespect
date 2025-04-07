<!DOCTYPE html>
<html lang="nl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Dierenliefde & Respect</title>
  <style>
    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f5f5f5;
      color: #333;
    }
    header {
      background-color: #4CAF50;
      color: white;
      padding: 40px 20px;
      text-align: center;
    }
    nav {
      background-color: #388e3c;
      padding: 10px;
      text-align: center;
    }
    nav a {
      color: white;
      text-decoration: none;
      margin: 0 15px;
      font-weight: bold;
    }
    main {
      max-width: 900px;
      margin: 40px auto;
      padding: 0 20px;
    }
    section {
      margin-bottom: 40px;
    }
    h2 {
      color: #388e3c;
    }
    a.button {
      display: inline-block;
      background-color: #4CAF50;
      color: white;
      padding: 10px 20px;
      margin-top: 10px;
      text-decoration: none;
      border-radius: 5px;
    }
    footer {
      text-align: center;
      padding: 20px;
      background-color: #e0e0e0;
      margin-top: 60px;
      color: #666;
    }
    .animal-images {
      display: flex;
      justify-content: space-between;
      margin: 20px 0;
    }
    .animal-images img {
      width: 30%;
      height: auto;
      border-radius: 10px;
      box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.1);
    }
    .tip-button {
      display: inline-block;
      background-color: #388e3c;
      color: white;
      padding: 12px 20px;
      margin-top: 20px;
      text-decoration: none;
      border-radius: 5px;
      font-weight: bold;
    }
    .popup-fact {
      display: none;
      background-color: #fff;
      border: 1px solid #388e3c;
      padding: 20px;
      border-radius: 10px;
      max-width: 500px;
      margin: 30px auto;
      text-align: center;
    }
  </style>
  <script>
    function showFact() {
      const facts = [
        "Wist je dat honden ongeveer 100 verschillende geluiden kunnen maken?",
        "Wist je dat olifanten zich kunnen herinneren waar waterbronnen zijn, zelfs na jaren?",
        "Wist je dat katten kunnen springen tot 6 keer hun lengte?",
        "Wist je dat dolfijnen elkaar een naam geven?",
        "Wist je dat konijnen snel kunnen rennen, tot 56 km/u?"
      ];
      const randomFact = facts[Math.floor(Math.random() * facts.length)];
      document.getElementById("fact-text").innerText = randomFact;
      document.getElementById("fact-popup").style.display = "block";
    }

    function closePopup() {
      document.getElementById("fact-popup").style.display = "none";
    }
  </script>
</head>
<body>

  <header>
    <h1>Dierenliefde & Respect</h1>
    <p>Voor een wereld waarin dieren met zorg en respect worden behandeld</p>
  </header>

  <nav>
    <a href="#welkom">Welkom</a>
    <a href="#watjijkuntdoen">Wat jij kunt doen</a>
    <a href="#overons">Over ons</a>
    <a href="https://www.instagram.com/goed_omgaan_met_dieren_25" target="_blank">Instagram</a>
  </nav>

  <main>
    <section id="welkom">
      <h2>Welkom</h2>
      <p>De volgende stelling staat centraal: alle diersoorten hebben recht op een zodanig niveau van welzijn dat mishandeling en lijden geen rol meer mogen spelen...</p>

      <p>We nodigen je graag uit om ons te volgen op Instagram:  
        <a href="https://www.instagram.com/goed_omgaan_met_dieren_25" target="_blank">@goed_omgaan_met_dieren_25</a>
      </p>

      <div class="animal-images">
        <img src="animal1.jpg" alt="Dier 1">
        <img src="animal2.jpg" alt="Dier 2">
        <img src="animal3.jpg" alt="Dier 3">
      </div>
    </section>

    <section id="watjijkuntdoen">
      <h2>Wat jij kunt doen</h2>
      <ul>
        <li>Overweeg adoptie in plaats van aankoop.</li>
        <li>Meld vermoedens van mishandeling bij de bevoegde instanties.</li>
        <li>Steun organisaties en individuen die zich inzetten voor dierenwelzijn.</li>
        <li>Informeer anderen over het belang van respect voor dieren.</li>
        <li>Geef huisdieren rust, ruimte en aandacht.</li>
      </ul>
      <a class="button" href="https://www.dierenbescherming.nl" target="_blank">Steun de Dierenbescherming</a>
      <a class="button" href="https://www.worldanimalprotection.nl/" target="_blank">World Animal Protection</a>
    </section>

    <section id="overons">
      <h2>Over ons</h2>
      <p>Wij zijn een groep scholieren die zich inzet voor het welzijn van dieren...</p>
      <p>Door samen te werken geloven we dat we daadwerkelijk verandering kunnen realiseren.</p>
    </section>

    <button class="tip-button" onclick="showFact()">Ontvang een Dierenfeit!</button>

    <div class="popup-fact" id="fact-popup">
      <p id="fact-text"></p>
      <button onclick="closePopup()">Sluit</button>
    </div>
  </main>

  <footer>
    © 2025 Dierenliefde & Respect | Gemaakt door scholieren voor een betere wereld
  </footer>

</body>
</html>





