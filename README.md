# geodev-lab-project
This is a project about Gas Flaring in Rivers state, Nigeria 
# Gas Flaring & Population Exposure Analysis: Rivers State, Nigeria

## Project Overview
This GIS project maps the spatial distribution of active gas flares across Rivers State, Nigeria, and quantifies human exposure to these environmental hazards. By combining nighttime satellite thermal data with high-resolution population grids, this study identifies vulnerable populations living within critical exposure zones.

## Objectives
- Locate active gas flares using NOAA VIIRS Nightfire satellite data.
- Establish environmental exposure zones using multi-ring buffers (2km, 5km, 10km).
- Estimate the total population impacted within each buffer zone using WorldPop spatial datasets.
- Aggregate exposure metrics by Local Government Area (LGA) to highlight environmental justice priorities.

## Methodology & Workflow
1. Data Ingestion & Clipping: Project all datasets to UTM Zone 32N (EPSG:32632) for accurate distance measurements in meters. Filter Nigeria administrative boundaries to Rivers State.
2. Proximity Analysis: Generate multi-ring vector buffers around flare coordinates.
3. Zonal Statistics: Run raster analytics to sum the population pixels falling within each buffer zone.
4. Data Aggregation: Dissolve and intersect layers to determine the most impacted LGAs.

## Results & Key Findings (to be determined)
  (Update this section once your GIS analysis is complete!)  
  Total Flares Detected: X active flares across the state.
  Population at Risk: Approximately X,XXX people live within 2km of an active flare.
  Most Impacted LGA: [Insert LGA Name] shows the highest density of population exposure.

## Technologies Used
- GIS Software: QGIS 
- Data Analysis: Python (Geopandas, Rasterio)   
- Coordinate System: WGS 84 / UTM Zone 32N

## Data Sources
- Gas Flare Locations: [NOAA Earth Observation Group (EOG) VIIRS Nightfire](https://mines.edu)
- Population Data: [WorldPop Project Nigeria 100m Grid](https://worldpop.org)
- Administrative Boundaries: [OCHA Nigeria via HDX](https://humdata.org)
