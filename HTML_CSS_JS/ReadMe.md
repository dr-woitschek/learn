**HTML/CSS/JS mit Leaflet**

---

1. wir erstelle einen Work-Ordner, zum Beispiel in über die `cmd.exe` mit `mkdir C:\Users\%username%\work`
2. in unserem Work-Ordner erstellen wir eine neue Datei mit dem Namen `spass-mit-leaflet.html`
3. in der neu erstellten HTML-Datei müssen wir ein HTML-Grundgerüst erstellen
   ```
   <!DOCTYPE html>
   <html lang="en">
      <head>
         <meta charset="utf-8">
         <title>Leaflet-Beispiel von Dr. Woitschek</title>
      </head>
      <body>
      <h1>:)</h1>
      </body>
   </html>
   ```
4. um Leaflet in unsere HTML-Datei einbinden zu können, müssen wir nachfolgende Zeilen in den HTML-Header einfügen
   ```
   <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin=""/>
   <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>
   ```
5. per CSS formatieren wir die HTML-Objekte, dieser Code wird in den HTML-Header eingefügt
   ```
   <style>
      html, body {
         height:    100%;
         margin:    0   auto;
         padding:   15px;
      }
      .leaflet-container {
         border:         1px solid black;
         border-radius:  8px;
         height:         100%;
         width:          100%;
         max-width:      100%;
         max-height:     85%;
      }
      .marker-ff0000 { /* Color: Rot     */ width: 2rem; height: 2rem; border-radius: 2rem; background: #ff0000; }
      .marker-000000 { /* Color: Schwarz */ width: 2rem; height: 2rem; border-radius: 2rem; background: #000000; }
   </style>
   ```
6. für die Anzeige der Karte benötigen wir im Body einen `<div>`-Container
   ```
   <div id='map'></div>
   ```
7. um die Karte mit allen funktionen einzubinden benötigen wir folgenden Code. Die Werte [52.52003, 13.40489] geben den Mittelpunkt von Deutschland an.
   ```
   <script>
      const map = L.map('map').setView([52.52003, 13.40489], 5);
      L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
         attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
   	  }).addTo(map);
   </script>
   ```
8. mit nachfolgendem Code können wir einen Marker auf der Karte setzten
   ```
   <script>
      var dieMarkierungsCSSClass = L.divIcon({className: 'marker-ff0000'});
      const einePunkt001 = L.marker([ 48.218775 , 11.624753 ], {icon: dieMarkierungsCSSClass}).bindPopup( 'Allianz Arena des FC Bayern München in München').addTo(map);
   </script>
   ```
9. hier der komplette Code
   ```
   <!DOCTYPE html>
   <html lang="en">
      <head>
         <meta charset="utf-8">
         <title>Leaflet-Beispiel von Dr. Woitschek</title>
   	  <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css" integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY=" crossorigin=""/>
         <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js" integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo=" crossorigin=""></script>
         <style>
            html, body {
               height:    100%;
               margin:    0   auto;
               padding:   15px;
            }
            .leaflet-container {
               border:         1px solid black;
               border-radius:  8px;
               height:         100%;
               width:          100%;
               max-width:      100%;
               max-height:     85%;
            }
            .marker-ff0000 { /* Color: Rot     */ width: 2rem; height: 2rem; border-radius: 2rem; background: #ff0000; }
            .marker-000000 { /* Color: Schwarz */ width: 2rem; height: 2rem; border-radius: 2rem; background: #000000; }
         </style>
      </head>
      <body>
         <div id='map'></div>
         <h1>:)</h1>
         <script>
            const map = L.map('map').setView([52.52003, 13.40489], 5);
            L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
               attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
         	  }).addTo(map);
         </script>
         <script>
            var dieMarkierungsCSSClass = L.divIcon({className: 'marker-ff0000'});
            const einePunkt001 = L.marker([ 48.218775 , 11.624753 ], {icon: dieMarkierungsCSSClass}).bindPopup( 'Allianz Arena des FC Bayern München in München'                ).addTo(map);
            const einePunkt002 = L.marker([ 48.3225   , 10.882222 ], {icon: dieMarkierungsCSSClass}).bindPopup( 'SGL Arena des FC Augsburg in Augsburg'                         ).addTo(map);
            const einePunkt003 = L.marker([ 51.038256 , 7.002206  ], {icon: dieMarkierungsCSSClass}).bindPopup( 'BayArena von Bayer Leverkusen in Leverkusen'                   ).addTo(map);
            const einePunkt004 = L.marker([ 51.492569 , 7.451842  ], {icon: dieMarkierungsCSSClass}).bindPopup( 'Signal Iduna Park von Borussia Dortmund in Dortmund'           ).addTo(map);
            const einePunkt005 = L.marker([ 51.174583 , 6.385464  ], {icon: dieMarkierungsCSSClass}).bindPopup( 'Borussia-Park des Borussia Mönchengladbach in Mönchengladbach' ).addTo(map);
            const einePunkt006 = L.marker([ 50.068572 , 8.645458  ], {icon: dieMarkierungsCSSClass}).bindPopup( 'Commerzbank-Arena von Eintracht Frankfurt in Frankfurt'        ).addTo(map);
            const einePunkt007 = L.marker([ 47.988889 , 7.893056  ], {icon: dieMarkierungsCSSClass}).bindPopup( 'MAGE SOLAR Stadion des SC Freiburg in Freiburg'                ).addTo(map);
            const einePunkt008 = L.marker([ 49.239008 , 8.888281  ], {icon: dieMarkierungsCSSClass}).bindPopup( 'Rhein-Neckar Arena von TSG 1899 Hoffenheim in Sinsheim'        ).addTo(map);
            const einePunkt009 = L.marker([ 49.984167 , 8.224167  ], {icon: dieMarkierungsCSSClass}).bindPopup( 'Coface Arena des 1. FSV Mainz 05 in Mainz'                     ).addTo(map);
            const einePunkt010 = L.marker([ 48.792269 , 9.232031  ], {icon: dieMarkierungsCSSClass}).bindPopup( 'Mercedes-Benz Arena des VfB Stuttgart in Stuttgart'            ).addTo(map);
            const einePunkt011 = L.marker([ 53.066394 , 8.837628  ], {icon: dieMarkierungsCSSClass}).bindPopup( 'Weserstadion von Werder Bremen in Bremen'                      ).addTo(map);
            const einePunkt012 = L.marker([ 52.431944 , 10.803889 ], {icon: dieMarkierungsCSSClass}).bindPopup( 'Volkswagen Arena des VfL Wolfsburg in Wolfsburg'               ).addTo(map);
            const einePunkt013 = L.marker([ 53.554444 , 9.967778  ], {icon: dieMarkierungsCSSClass}).bindPopup( 'Millerntor-Stadion des FC St. Pauli in Hamburg'                ).addTo(map);
         </script>
      </body>
   </html>
   ```

---

_Weitere Informationen_
- [https://wiki.selfhtml.org/wiki/SELFHTML](https://wiki.selfhtml.org/wiki/SELFHTML)
- [https://leafletjs.com/](https://leafletjs.com/)
