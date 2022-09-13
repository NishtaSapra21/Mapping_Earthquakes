# Mapping Earthquakes

## Overview

  The purpose of this analysis is to add tectonic plate data, major earthquake data and additional map “dark” layer on visually shown magnitudes of earthquakes all       over   the world for the last seven days using __JavaScript__ , __D3.js__ library to retrieve the coordinates and magnitudes of the earthquakes from the __GeoJSON__   data. __Leaflet__ library is used to plot the data on a __Mapbox__ map through an API request and create interactivity for the earthquake data.

## Results

  * Tectonic Plate Data

      d3.json("https://raw.githubusercontent.com/fraxen/tectonicplates/master/GeoJSON/PB2002_boundaries.json") makes a call to get tectonic plate data. GeoJSON objects       are added to the map through a GeoJSON layer, L.geoJSON() which parses our data. In geoJSON() layer , lines are styled with color “orange” and weight “2.5” to         show tectonic plates of earth. 
      
      After adding tectonic plate layer to map, map looks like below in satellite view with orange plate lines having weight 2.5. 
      
      ![tectonic_plates_satellite](https://user-images.githubusercontent.com/107717882/190008694-2cc06236-ceb5-405c-906b-4ab83e353aa3.png)

  * Major Earthquake Data
  
      d3.json("https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/4.5_week.geojson") makes a call to get major earthquake data and passes it to GeoJSON layer to       add circlemaker , add style to circlemaker with colors  and size , creates a popup for the circle to display magnitude and location of the earthquake.
      
      After adding major earthquake layer to map, map looks like below with major earthquakes displaying.
            
      ![major_earthquakes](https://user-images.githubusercontent.com/107717882/190008728-eb0bdf10-b747-47bf-9413-e9e3bc671b92.png)

      Folowing image shows earthquake data with major earthquakes and tectonic plates with popup marker in "dark" theme.
      
      ![all_data_dark](https://user-images.githubusercontent.com/107717882/190008753-294e09ba-b2d6-4233-973a-b1bc7a7eef80.png)
      
## Summary

   Plotting your data analysis is very important aspect. In this analysis,  Leaflet helps to display interactive earthquake maps  using Mapbox API with the help of        JAvaScrip , GeoJSON ang D3.js library.  Also, we can view map with major earthquakes, tectonic plates by selecting street, satellite or dark views. This analysis      gives us insight that which part of earth has more earthquakes, with more magnitudes. Largest earthquake belt you can see near Pacific Ocean.  
   
   Have a look at complete page of __“Mapping Earthquakes”__ .
   
   ![mapping_earthquakes](https://user-images.githubusercontent.com/107717882/190010640-476ee3c2-741f-4ed2-b732-80cc07fc584a.png)

   
   
   

