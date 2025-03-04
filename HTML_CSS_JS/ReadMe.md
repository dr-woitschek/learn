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









---

_Weitere Informationen_
- [https://wiki.selfhtml.org/wiki/SELFHTML](https://wiki.selfhtml.org/wiki/SELFHTML)
- [https://leafletjs.com/](https://leafletjs.com/)
