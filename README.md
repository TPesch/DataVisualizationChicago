# CSV Data on Map and D3.js Charts

This project visualizes CSV data on a map using Leaflet and D3.js to create comparative charts. The data includes gun violence incidents, bike racks, and car crashes in Chicago wards.

## Features

- **Interactive Map**: Displays data points for bike racks, gun violence incidents, and car crashes on a map of Chicago using Leaflet.
- **Clustered Markers**: Uses marker clustering for better visualization of densely populated data points.
- **Popup Information**: Each data point on the map displays detailed information in a popup when clicked.
- **Comparative Charts**: Creates bar charts comparing the number of incidents, bike racks, and car crashes per ward using D3.js.

## Setup

1. **Include Dependencies**:
   - Leaflet CSS and JS for interactive maps.
   - Leaflet MarkerCluster for clustering markers on the map.
   - PapaParse for parsing CSV data.
   - D3.js for creating charts.

2. **HTML Structure**:
   - A div with id `map` to display the map.
   - A div with id `chart` to display the charts.

3. **JavaScript Functionality**:
   - Initialize the map centered on Chicago with Leaflet.
   - Define custom icons for bike racks, gun violence, and car crashes.
   - Create marker clusters for each data type.
   - Fetch and parse CSV data for bike racks, gun violence incidents, and car crashes using PapaParse.
   - Plot the data on the map and aggregate data for each ward.
   - Create bar charts comparing the number of incidents, bike racks, and car crashes per ward using D3.js.

## Usage

1. **Load CSV Data**:
   - Ensure CSV files (`bike-racks.csv`, `Gun_Violence_Data_with_Wards.csv`, and `filtered_car_crash_data_2019_cleaned_v2.csv`) are placed in the `CSV` directory.

2. **Run the HTML File**:
   - Open the HTML file in a web browser. The map will load with clustered markers, and the charts will be generated below the map.

3. **Interacting with the Map**:
   - Click on any marker to view detailed information about the data point.
   - The clusters will expand to show individual markers on zooming in.

## Example CSV Structure

### Bike Racks

| Latitude | Longitude | Address         |
|----------|-----------|-----------------|
| 41.8781  | -87.6298  | 123 Main St     |
| 41.8827  | -87.6233  | 456 Elm St      |

### Gun Violence

| latitude | longitude | date       | address       | n_killed | n_injured | ward |
|----------|-----------|------------|---------------|----------|-----------|------|
| 41.8781  | -87.6298  | 2022-01-01 | 789 Oak St    | 2        | 3         | 1    |
| 41.8827  | -87.6233  | 2022-01-02 | 101 Pine St   | 1        | 1         | 2    |

### Car Crashes

| latitude | longitude | date       | town        | total_injured | total_killed | contributory_cause | ward |
|----------|-----------|------------|-------------|---------------|--------------|--------------------|------|
| 41.8781  | -87.6298  | 2022-01-01 | Chicago     | 3             | 1            | Speeding           | 1    |
| 41.8827  | -87.6233  | 2022-01-02 | Chicago     | 2             | 0            | DUI                | 2    |

## Accessing the Project

You can access the project hosted on GitHub [here](https://tpesch.github.io/DataVisualizationChicago/index.html).

