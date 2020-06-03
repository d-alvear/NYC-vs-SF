# Battle of the Cities: New York City vs. San Francisco

## Overview

This is an _unfinished_ refactoring of the project I completed through the Data Science Specialization Capstone Course through Coursera in June 2019. After completeing Dataquest in October 2019, I had a better grasp of Python and machine learning methods, so I decided to revisit this project and refactor it. See the original project [here](https://nbviewer.jupyter.org/gist/d-alvear/6b023d5d5bf0c458c66f4a26379f99a9).

My goal was to answer, based on neighborhood venue types, whether Manhattan or San Francisco offers more "bang for your buck." I compared rent prices and venues per neighborhood for both cities. I used k-means clustering analysis and leveraged data using the Foursquare API.

I wanted to improve upon the first iteration of this project by incorporating more factors into the analysis, such as quality of schools, percent greenspace, etc.

## Methods
* __Rent Analysis__ ([nbviewer](https://nbviewer.jupyter.org/github/d-alvear/NYC-vs-SF/blob/master/notebooks/rent-analysis.ipynb)): comparing the distributions of rent prices between San Francisco and Manhattan.
* __Choropleth Maps__ ([nbviewer](https://nbviewer.jupyter.org/github/d-alvear/NYC-vs-SF/blob/master/notebooks/data-visualizations.ipynb)): used the Folium library to create heatmaps of each city that indicate neighborhoods of high, moderate, and low rent relative to the median rent price in the city,
* __Foursquare API__ ([nbviewer](https://nbviewer.jupyter.org/github/d-alvear/NYC-vs-SF/blob/master/notebooks/foursquare-api-work.ipynb)): used the API to get all venues in each neighborhood using neighborhood latitude/longitude; used one-hot encoding to calculate the frequency of venue type. This allowed me to see the top 10 most common venues in each neighborhood for both cities.
* __K-Means Clustering__ ([nbviewer](https://nbviewer.jupyter.org/github/d-alvear/NYC-vs-SF/blob/master/notebooks/clustering-nb.ipynb)): clustered the neighborhoods by their top 10 most common venue types to see which neighborhoods are similar to each other. Examined each cluster to see what criteria the neighborhoods were being clustered on ([nbviewer](https://nbviewer.jupyter.org/github/d-alvear/NYC-vs-SF/blob/master/notebooks/examine-clusters.ipynb)).

### To Do/Ideas:

* ~~find neighborhood data to partition each city into its neighborhoods~~
* ~~find median rent prices per neighborhood~~
* transportation counts with average wait times?
* ~~venue data from Foursquare API~~
* percentage greenspace?
* quality of schools?
### Done

* cleaned rent data
* tested geojson files with folium
