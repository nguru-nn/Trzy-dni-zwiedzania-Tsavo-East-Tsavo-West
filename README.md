# Diani Beach → Tsavo East & Tsavo West: 3-Day Safari Map
 
This is an interactive 3D map of a 3-day road safari from **Diani Beach** on Kenya's south coast. The trip covers both halves of the Tsavo ecosystem, which together form one of the largest protected wildlife areas in Africa. Visitors see the open red-earth plains of **Tsavo East** and the volcanic hills of **Tsavo West**, staying overnight at **Voi Safari Lodge** and **Ngulia Safari Lodge**.
 
🗺️ **See the full itinerary and the live map:**
[Trzy dni zwiedzania – Tsavo Wschód i Tsavo Zachód](https://safarikenia.com.pl/trzy-dni-zwiedzania-tsavo-wschod-tsavo-zachod) on **Safari Kenia**
 
---
 
## The route
 
| Day | Park | Accommodation |
|-----|------|---------------|
| Start | Departure from Diani Beach | — |
| Day 1 | Tsavo East National Park | Voi Safari Lodge |
| Day 2 | Tsavo West National Park | Ngulia Safari Lodge |
| Day 3 | Return to Diani Beach | — |
 
**Day 1:** Diani Beach → Likoni Ferry → Mombasa → Mazeras → Mariakani → Taru → Mackinnon Road → Buchuma Gate → game drive to Voi Safari Lodge
**Day 2:** Voi → Mwatate → into Tsavo West → Ngulia Safari Lodge
**Day 3:** Tsavo West → Voi → Mariakani → Likoni Ferry → Diani Beach
 
The interface labels are in Polish, matching the tour page it's embedded on.
 
## Features
 
- **Two parks in one trip.** The route links Tsavo East and Tsavo West, so the map shows the contrast between the flat eastern plains and the rugged, hilly west.
- **Satellite basemap with 3D terrain.** The map uses the Mapbox Standard Satellite style with DEM terrain at 1.5× exaggeration and a tilted camera. This brings out the Ngulia Hills and the lava landscapes of Tsavo West.
- **Road-accurate route.** Each leg is fetched from the Mapbox Directions API (driving profile) and stitched into one line. If a request fails, that leg falls back to a straight segment.
- **Animated route line.** A golden "marching ants" dashed line runs over a soft glow layer.
- **Interactive itinerary panel.** A glassmorphism sidebar lists each day. Clicking a card flies the camera to that lodge and opens its popup.
- **Optimised for mobile.** On small screens the map gets a compact layout: a shorter container, a tighter bottom-sheet sidebar and smaller controls. Camera fly-to is offset so the selected lodge isn't hidden behind the sheet.
- **Custom markers.** Gold SVG pins mark the overnight stops. Hidden waypoints keep the route on the correct roads.
- **WordPress-ready.** Styles are scoped to a single container, so the code can be pasted into a Custom HTML block.
## Tech stack
 
- [Mapbox GL JS](https://docs.mapbox.com/mapbox-gl-js/) v3.9.0
- [Mapbox Directions API](https://docs.mapbox.com/api/navigation/directions/)
- Vanilla JavaScript, no build step
- Plus Jakarta Sans (Google Fonts)
## Usage
 
1. Copy the HTML into a WordPress **Custom HTML** block or any web page.
2. Replace the Mapbox access token with your own, and restrict it to your domain in your [Mapbox account](https://account.mapbox.com/access-tokens/).
3. Adjust the container height in `.wp-safari-itinerary-container` to fit your layout.
To change the route, edit the `itineraryData` array. Entries with `isWaypoint: true` only shape the route. All other entries get a marker and a sidebar card.
 
## About
 
Built for [Safari Kenia](https://safarikenia.com.pl/), which offers Polish-language safari tours and travel guides for Kenya.
 
➡️ [View this 3-day Tsavo East & Tsavo West itinerary](https://safarikenia.com.pl/trzy-dni-zwiedzania-tsavo-wschod-tsavo-zachod)
