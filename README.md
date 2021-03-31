# webgis-web-charlie
Web solution group project.

## 🗺️ Live Web Map Solution
https://jimhwei.github.io/webgis-web-charlie/

## 📍 Documentation on Mapbox GeoJSON Upload
Adding a marker to a web map and combining it with a symbol layer may be much more simple than wrangling with ArcGIS Rest Endpoints. A good developer can do both, so this documentation covers how to upload points into mapbox.

### 🧹 Data Cleaning
It might be beneficial to ensure the GeoJSON file of all your points are prepped and ready to go. Using VSCode, you can add or remove points, fields. 
[How to Edit GeoJSON using VSCode](https://dev.to/deadlybyte/working-with-geojson-and-vs-code-2ken)

### 💡 Creating a Dataset 
1. Log into Mapbox Studio and navigate to the Datasets page.
2. Click the New dataset button.
3. Select the Upload option in the upper right corner of the New Dataset modal.
4. Select the GeoJSON file you want to upload. Create and confirm.
5. Drawing new features, and adding properties are all possible in the mapbox studio

![Points Editing](https://docs.mapbox.com/help/img/studio/point-tutorial-dataset-edit.gif)

### ➡️ Exporting the dataset as tileset
The difference between ArcGIS REST Endpoint and Mapbox is that the REST endpoints does a transformation process to fit into the Mapbox web format. It is not considered native and unexpected issues such as projection differences could toss it into chaos. Exporting the dataset as a tileset in mapbox can make it possible to be added into a Mapbox style.

![Exporting as tileset](https://docs.mapbox.com/help/assets/tutorials--add-points-export-to-tileset-960-cd49ef2de90671c42df9a9dd6574c220.png)

According to Mapbox: *Web maps are comprised of map tiles. A collection of tiles is called a tileset. Mapbox cuts up data into tiles that are then added to a web map and displayed at various zoom levels. To make Mapbox maps more performant, a dataset's features are simplified when it is converted into a tileset.*

![Mapbox Tileview](https://user-images.githubusercontent.com/60511633/113148685-239bcb00-9200-11eb-99f2-1052fce00b55.png)
