---
title: Welcome to my game
---

<html>
  <head>
    <title>Gamefroot Arcade</title>
    <style>
      body, html {
        margin: 0;
        padding: 0;
        background: black;
        overflow:  hidden;
      }

      #game-container {
        margin: auto;
      }
    </style>

    <script src="libs/phaser.js"></script>
    <script src="libs/phaserfroot.js"></script>

    <script>
      var game = Phaserfroot.boot( {
        data: "game.json",
        parent: "game-container",
        width: 768,
        height: 512,
        scale: {
          autoCenter: Phaser.Scale.CENTER_HORIZONTALLY,
          mode: Phaser.Scale.FIT,
        },
        splash: {
          image: "assets/images/gamefrootAtlas.png",
          json: "assets/images/gamefrootAtlas.phaser.json",
        },
      } );
    </script>
  </head>
  <body>
    <div id="game-container"></div>
  </body>
</html>
