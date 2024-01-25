<html>
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="initial-scale=1, maximum-scale=1, user-scalable=no" />
    <title>ArcGIS Maps SDK for JavaScript Tutorials: Display a map</title>

    <style>
      html,
      body,
      #viewDiv {
        padding: 0;
        margin: 0;
        height: 100%;
        width: 100%;
      }
    </style>

    <link rel="stylesheet" href="https://js.arcgis.com/4.28/esri/themes/light/main.css">
    <script src="https://js.arcgis.com/4.28/"></script>

   <script>
      require(["esri/config", "esri/Map", "esri/views/MapView"], function(esriConfig, Map, MapView) {


        esriConfig.apiKey = "AAPK51e574e8cc2f4290996b983abcbdea5cJ2WK7X63hl7OAfynAq71bsWM4QH7Pd9-RoF-qLrFGZNpfYFwoFVxhj4X4q6P1Wym";

        const map = new Map({
          basemap: "arcgis/topographic" // basemap styles service
        });

        const view = new MapView({
          map: map,
          center: [-118.805, 34.027], // Longitude, latitude
          zoom: 13, // Zoom level
          container: "viewDiv" // Div element
        });

      });
    </script>

  </head>
  <body>
    <div id="viewDiv"></div>
  </body>
</html>  
