# Covid-19 Worldwide Map

+ Final assignments of Application Development course (2019-2020) of University of Salzburg.
+ Click [here](https://maps.solidjerryc.com/index.html) to visit the website.
+ The front page consists of 2 parts: Covid-19 Map (all the group members) and location-sharing (Jerry Cai).
+ Javascript/Python/OpenLayers/echarts
+ My teammates: Jerry Cai, Bismark Ade, Leo Eger, Yumeng Zhou & Ziyan Ding.

## Basic Structure
This project has two parts in total. The Covid-19 map is an interactive web-map that lets the user explore the development of covid-19 cases for most countries in different kinds of charts, covering each day in the course of the pandemic. The location sharing part allows users to share their geolocation on the webpage. Users can switch the different tabs by clicking the buttons in the navigation bar.

## Data
+ Covid-19 cases by country are taken from: https://github.com/pomber/covid19 (should be updated three times a day, but in reality the data is usually one to two days late)
+ Country polygons are taken from: https://openlayers.org/en/latest/examples/data/geojson/countries.geojson (Partly different country names than the covid data. E.g. “United states of america” versus “Us”

## Api-used
+ OpenLayers for the web-map: https://openlayers.org/en/v5.3.0/build/ol.js
+ JQuery: https://code.jquery.com/jquery-1.11.0.min.js
+ Bootstrap: (For styling buttons, only barely used) https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/js/bootstrap.min.js 
+ Chart.js for the creation of the line chart of every country/region: https://cdn.jsdelivr.net/npm/chart.js@2.9.3/dist/Chart.min.js
+ Echarts.js which is anopen-sourced tool for the creation and visualization of charts on the upper-right corner: https://echarts.apache.org/en/index.html  

## Covid-19 map 
An interactive web-map to explore covid-19 cases (confirmed, active, recovered, dead) for almost all countries in the world. When clicking on a country/region a line-chart will appear and display information on the different cases per day for the selected country/region. By using the ‘logarithmic/linear’ button on the bottom left the y-Scale can be toggled between a linear or logarithmic scale which is useful for countries with low amounts of cases or the beginning stages for other countries. 

On the upper right side of the page, there are three charts and one statistic graph. They are showing the global situation by default. When users click on a specific country/region, the charts would change and show the numbers and distributions of this selected country/region. Users can also switch charts by clicking on the buttons.
Also on the map is the circle bubbles that represent the cluster  of cases per country. This is proportional to the number of cases being confirmed by the various countries. The classes were created proportionally and will vary (increase) if the number of cases increase. 

The histogram shows the comparison of the number of recovered people, deaths, active people  and confirmed people more intuitively. The horizontal axis shows several statistical data types, including recovered, deaths,active and confirmed data. The vertical axis shows the specific value of different data types. 

Recovery rate is recovery cases over confirmed cases and mortality rate is deaths cases over confirmed cases. The numbers after these percentages are the recovery cases and mortality cases. EChart's biaxial bar chart is modified into this figure.

## Location-sharing
Location sharing is a map that allows the users to share their geolocations to friends and see each other on the map. This part is fully done by Jerry Cai. 

## Possible Improvements and Additions
+ Responsive design
+ Addition of a button to remove the days without any incidents in the beginning
+ Resizable chart (by dragging or with two buttons)
+ Option to show the development of the pandemic globally for each day in the chart
+ Inclusion of more specific data for selected countries (states, cities)
+ the website often need about 10 seconds to load.


