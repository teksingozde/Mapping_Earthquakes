# Mapping Earthquakes
## Overview of Project

Client requested to create a map with all earthquake information about past 7 days opening the page on the desired website. Circle marker size will be determined on the map according to the magnitude of each earthquake and coloring will be done. The website will be displayed in HTML file, formatted in CSS file, and Leaflet map will be created with Mapbox API key requirement and visualized with different map styles using GeoJSON dataset.

### Resources
#### Software: 
- HTML,
- CSS,
- JavaScript.

#### Other Resources:
- Mapbox – Public API Key required,
- Leaflet (version 1. 9. 3),
- USGS Earthquake Hazards Program Fraxen tectonic plates Github Repository.

## Creating Web Page 
The HTML file is the environment where the codes written in CSS and JavaScript interact with the map. Details of all work and code pieces on the map can be accessed via the Javascript file.
A separate filing technique was created for each map and named the same.
Within each file, there are “index.html”, and static folders. The static folder contains css and .js files.
The file creation format is as follows.
<img width="159" alt="Screen Shot 2022-12-15 at 2 03 12 PM" src="https://user-images.githubusercontent.com/26927158/207965886-df003309-260a-4007-81e2-843384fafa5b.png">

The “index.html” information includes the title of the page created in our web browser and Leaflet CSS, D3 Javascript and Page CSS information. However, we must create the path of the files in the folder on the computer correctly so that when we click on index.html, the website opened by the browser can connect with all the files. If the path containing our CSS, API key and JavaScript file is not formatted correctly, we will not be able to obtain the desired map or image in our web browser.

In the “style.css” file, there is information about the style of the page created with the html link. These style formats are; They are properties such as width, height, padding, margin, color, background-color, float, opacity.

There is a link in the JavaScript file that we call “logic.js” that provides access to the map styles created using the mapbox called tileLayer. Map formatting can be done on this link. Each map style has its own unique link. The styles we use while mapping are; streets, satellite and narrow. If you want to use other styles, map styles such as outdoors, navigation can also be added. Within the JavaScript file, the API_KEY called Access_token must be specified in each link, and in this way the map styles can be accessed. The link containing the GeoJSON dataset is also included in the JavaScript file. However, while the earthquake magnitude scale is being created, the coloring and the scale information showing the severity are also coded in the JavaScript file. Tectonic plate and circle marker information, which shows the severity of the earthquake, are also encoded in the JavaScript file and colored according to the severity. For Tectonic plate, Fraxen tectonic plates Repository information on Github was used.

The "config.py" file contains the API key information and this file will not be shared in Github files. The reason for this is confidentiality. When API key access is provided, our bank account information can be accessed if it is captured by others, and this is a dangerous situation.

## Results
The images obtained from the maps are as follows.

#### Map 1. Simple Map
<img width="1271" alt="Simple_Map" src="https://user-images.githubusercontent.com/26927158/207966114-f7691115-efab-417e-9e70-7d2ff10a2401.png">
The map above is a simple image without earthquake magnitudes, obtained with the help of Leaflet and which we will use as the map style.

#### Map 2. Tectonic Plate – Earthquakes – Major Earthquakes Streets Map
<img width="1275" alt="Streets_Tectonic_Major_Earthquakes" src="https://user-images.githubusercontent.com/26927158/207966361-3646bb6e-b25b-4849-a515-d09c5b5b2c62.png">
The map above shows the tectonic plate, that is, the regions where the fault line passes, and the magnitudes of the earthquakes with the circle maker and their intensity with the colors.

#### Map 3. Tectonic Plate – Earthquakes – Major Earthquakes Satellite Streets Map
<img width="1274" alt="SatelliteStreets_Tectonic_Major_Earthquakes" src="https://user-images.githubusercontent.com/26927158/207966473-e7bdfdac-7e58-481d-9838-4faf3250d113.png">
The map above is a visualized version of the map in Map 2 in Satellite format.

#### Map 4. Tectonic Plate – Earthquakes – Major Earthquakes Dark Map
<img width="1276" alt="Dark_Tectonic_Major_Earthquakes" src="https://user-images.githubusercontent.com/26927158/207966577-c63b7578-4151-4d88-8105-9e164dc37a0a.png">
The map above is a visualized version of the map in Map 2 and Map 3 in dark that is night mode.

#### Map 5. Past 7 Days Street Earthquakes
<img width="1275" alt="Streets_Earthquakes_Past7Days" src="https://user-images.githubusercontent.com/26927158/207966785-2c3cd8a2-91a4-4254-accf-fa9537031c62.png">
Map 5 shows the magnitude and intensity of the earthquakes that have occurred in the last 7 days. There is no tectonic plate visualization on this map.

#### Map 6. Past 7 Days Satellite Street Earthquakes
<img width="1276" alt="SatelliteStreets_Earthquakes_Past7Days" src="https://user-images.githubusercontent.com/26927158/207966980-91298f74-c1aa-49ff-a656-443d70549625.png">
Map 6 shows the magnitude and intensity of the earthquakes that have occurred in the last 7 days. The difference from the Map 5 image is that the map is created in satellite format. There is no tectonic plate visualization on this map.

## Summary
In general, if a result is created in terms of visualizations, earthquakes of 5 and above do not occur much. Generally, it is observed that earthquakes of 4-5 magnitude and 1-2 magnitude occur. Earthquake magnitudes of 4.5 and above are called major earthquakes and are visualized on the map.
