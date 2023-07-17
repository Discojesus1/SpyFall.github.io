<!DOCTYPE html>
<html>
<head>
  <title>Spyfall</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      text-align: center;
      background-color: #111;
      color: #fff;
      margin: 0;
      padding: 0;
    }

    h1 {
      color: #fff;
    }

    .game-container {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      margin: 0 auto;
      width: 800px;
      padding: 20px;
    }

    .game-card {
      flex: 1;
      margin: 0 10px;
      padding: 20px;
      border: 1px solid #fff;
      border-radius: 5px;
      background-color: #333;
    }

    h2, p {
      color: #fff;
      margin: 0;
      padding: 0;
    }

    button {
      margin-top: 20px;
      padding: 10px 20px;
      font-size: 16px;
      background-color: #fff;
      color: #111;
      border: none;
      border-radius: 3px;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <h1>Spyfall</h1>

  <div>
    <label for="theme-select">Choisir un thème :</label>
    <select id="theme-select" onchange="changeTheme()">
      <option value="default">Par défaut</option>
      <option value="countries">Pays</option>
      <option value="culture">Culture</option>
      <option value="scienceFiction">Science Fiction</option>
      <option value="films">Films & Séries</option>
      <option value="voyage">Voyage dans le temps</option>
    </select>
  </div>

  <div class="game-container">
    <div class="game-card" id="card1">
      <h2 class="location" style="display: none;"></h2>
      <p class="role" style="display: none;"></p>
      <button class="reveal-button" onclick="revealRole(1)">Révéler le rôle</button>
      <button class="hide-button" style="display: none;" onclick="hideRole(1)">Cacher le rôle</button>
    </div>
    <div class="game-card" id="card2">
      <h2 class="location" style="display: none;"></h2>
      <p class="role" style="display: none;"></p>
      <button class="reveal-button" onclick="revealRole(2)">Révéler le rôle</button>
      <button class="hide-button" style="display: none;" onclick="hideRole(2)">Cacher le rôle</button>
    </div>
    <div class="game-card" id="card3">
      <h2 class="location" style="display: none;"></h2>
      <p class="role" style="display: none;"></p>
      <button class="reveal-button" onclick="revealRole(3)">Révéler le rôle</button>
      <button class="hide-button" style="display: none;" onclick="hideRole(3)">Cacher le rôle</button>
    </div>
    <div class="game-card" id="card4">
      <h2 class="location" style="display: none;"></h2>
      <p class="role" style="display: none;"></p>
      <button class="reveal-button" onclick="revealRole(4)">Révéler le rôle</button>
      <button class="hide-button" style="display: none;" onclick="hideRole(4)">Cacher le rôle</button>
    </div>
  </div>

  <button onclick="restartGame()">Recommencer la partie</button>

  <script>
    var themes = {
      default: {
        locations: [
          "Plage",
          "Cinéma",
          "Hôtel",
          "Restaurant",
          "Station spatiale",
          "Forêt",
          "Maison",
          "Musée",
          "Maison Hantée",
          "Magasin",
          "Librairie",
          "Pharmacie",
          "Boulangerie"
        ],
        roles: [
          "Serveur",
          "Touriste",
          "Directeur",
          "Cuisinier"
        ]
      },
      countries: {
        locations: [
          "France",
          "Allemagne",
          "Espagne",
          "Italie",
          "États-Unis",
          "Autriche",
          "Pays-Bas",
          "Russie",
          "Ukraine",
          "Suisse",
          "Belgique"
        ],
        roles: [
          "Citoyen",
          "Touriste",
          "Chef",
          "Chauffeur"
        ]
      },
      culture: {
        locations: [
          "Galerie d'art",
          "Musée",
          "Opéra",
          "Bibliothèque",
          "Théâtre",
          "Cinéma",
          "Salle de concert",
          "Festival",
          "Salle de Karaoké"
        ],
        roles: [
          "Artiste",
          "Conservateur",
          "Directeur",
          "Critique"
        ]
      },
      scienceFiction: {
        locations: [
          "Planète Abandonnée",
          "Vaisseau Spatial",
          "Planète Colonisée",
          "La lune",
          "Vaisseau abandonné",
          "Dimension parallèle",
          "Trou noir",
          "Jupiter",
          "A bord du Discovery One",
          "Dans une simulation",
          "Dans un cauchemar"
        ],
        roles: [
          "Explorateur",
          "Pilote",
          "Scientifique",
          "Alien"
        ]
      },
      films: {
        locations: [
          "Star Wars",
          "Vol au-dessus d'un nid de coucou",
          "Amadeus",
          "2001, l'odyssée de l'espace",
          "Barry Lyndon",
          "Black Mirror",
          "Severance",
          "House of Cards",
          "Shining",
          "Blade Runner",
          "Les Rois Maudits",
          "Parasite",
          "Chernobyl",
          "The Last of Us",
          "Focus de Tim Berthaud",
          "Grand Budapest Hotel",
          "Univers de Tim Burton",
          "Univers de Wes Anderson",
          "Univers de Stanley Kubrick",
          "Harry Potter",
          "Jurassic Park"
        ],
        roles: [
          "Acteur",
          "Réalisateur",
          "Producteur",
          "Scénariste"
        ]
      },
      voyage: {
        locations: [
          "Préhistoire",
          "Grèce Antique",
          "Moyen Âge",
          "Révolution Française",
          "Rome Antique",
          "France, deuxième Guerre Mondiale",
          "France, guerre froide",
          "France, époque contemporaine",
          "Guerre en Ukraine",
          "Grenoble, 2100",
          "Fin des temps"
        ],
        roles: [
          "Voyageur temporel",
          "Historien",
          "Chef de guerre",
          "Survivant"
        ]
      },
    };

    var currentTheme = themes.default;
    var spyIndex;
    var sharedLocation;
    var roles = [];

    function getRandomLocation() {
      return currentTheme.locations[Math.floor(Math.random() * currentTheme.locations.length)];
    }

    function revealRole(cardId) {
      var locationElement = document.getElementById("card" + cardId).getElementsByClassName("location")[0];
      var roleElement = document.getElementById("card" + cardId).getElementsByClassName("role")[0];
      var revealButton = document.getElementById("card" + cardId).getElementsByClassName("reveal-button")[0];
      var hideButton = document.getElementById("card" + cardId).getElementsByClassName("hide-button")[0];

      if (revealButton.style.display === "none") {
        return;
      }

      if (cardId === spyIndex) {
        roleElement.textContent = "Vous êtes l'espion !";
        locationElement.textContent = "";
      } else {
        roleElement.textContent = "";
        locationElement.textContent = "Lieu : " + sharedLocation;
      }

      roleElement.style.display = "block";
      locationElement.style.display = "block";
      revealButton.style.display = "none";
      hideButton.style.display = "inline-block";
    }

    function hideRole(cardId) {
      var locationElement = document.getElementById("card" + cardId).getElementsByClassName("location")[0];
      var roleElement = document.getElementById("card" + cardId).getElementsByClassName("role")[0];
      var revealButton = document.getElementById("card" + cardId).getElementsByClassName("reveal-button")[0];
      var hideButton = document.getElementById("card" + cardId).getElementsByClassName("hide-button")[0];

      roleElement.style.display = "none";
      locationElement.style.display = "none";
      revealButton.style.display = "inline-block";
      hideButton.style.display = "none";
    }

    function setupGame() {
      spyIndex = Math.floor(Math.random() * 4) + 1;
      sharedLocation = getRandomLocation();

      for (var i = 1; i <= 4; i++) {
        var locationElement = document.getElementById("card" + i).getElementsByClassName("location")[0];
        var roleElement = document.getElementById("card" + i).getElementsByClassName("role")[0];
        var revealButton = document.getElementById("card" + i).getElementsByClassName("reveal-button")[0];
        var hideButton = document.getElementById("card" + i).getElementsByClassName("hide-button")[0];

        locationElement.style.display = "none";
        roleElement.style.display = "none";
        revealButton.style.display = "inline-block";
        hideButton.style.display = "none";
      }
    }

    function changeTheme() {
      var themeSelect = document.getElementById("theme-select");
      var selectedTheme = themeSelect.value;

      currentTheme = themes[selectedTheme];
      setupGame();
    }

    function restartGame() {
      setupGame();
    }

    setupGame();
  </script>
</body>
</html>
