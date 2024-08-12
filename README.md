# Old-growth projects
 This repository contains the data and code to building an exploration map for old-growth forests and logging projects in the United States:
 https://lauramiina.github.io/oldgrowth-project-search/

 The map was done as part of a Data Journalism Master's Project in Columbia Journalism School.

# Methodology
## Building interactive maps of old forests and logging projects
For this project, we built interactive maps to visualize the amount and location of old-growth forests in the U.S. and show where controversial logging projects are located. You can find the complete datasets, data analysis and code for building the maps on GitHub: https://github.com/LauraMiina/oldgrowth-project-search. The scrolly-telling map was made separately with a Mapbox template, and you can see that code in a separate GitHub repository: https://github.com/LauraMiina/oldgrowth. 
## Data Inquiry
The U.S. Forest Service (USFS) conducted a vast inventory and risk assessment of the old-growth and mature forests in the country. We used a Python tool, esri2gpd, to scrape the USFS data from their ArcGIS environment: https://apps.fs.usda.gov/fsgisx02/rest/services/wo_nfs_gstc/WO_OSC_GapAnalysis_OldGrowthAndMatureForests/MapServer/29.
The Python tool and instructions can be found here: https://github.com/PhilaController/esri2gpd.
The inventory doesn’t provide the exact locations of the old trees, but it shows the number of old-growth forest acres inside 250,000-acre areas called firesheds. These units, related to the USFS’s role as the nation’s largest fire-prevention agency, are used only as mapping units in this context.
The logging project data is from the Climate Forests, which provided us with a Google Doc with the data. We created a spreadsheet of the document so that it would be workable with code and could be uploaded to Mapbox. The project locations are approximations based on the USFS’s descriptions of the project areas.
Most of the data analysis was done visually using QGIS and Mapbox to show the locations and amounts of old-growth forest and also the acres threatened by the logging projects.
## Building the maps
We created a scrolly-telling map using Mapbox’s template and instructions. You can find the template here: https://labs.mapbox.com/education/impact-tools/interactive-storytelling/. Basically, you can upload your own location data to Mapbox and create visualizations, and just call the map layers with code.
In addition, we built a map with a search bar for exploring both datasets in their entirety using HTML, JavaScript, and CSS. This map uses the same Mapbox map as the scrolly.

