# Spatial-ML: A Python Exploration of Spatial Machine Learning

This repository is a collection of Python notebooks demonstrating a wide range of spatial analysis and machine learning techniques. It serves as a practical guide for moving from fundamental geospatial operations to advanced modelling, using a combination of synthetic and real-world data.

## Goals

- **Provide Clear Examples**  
  To offer runnable, well-commented examples of common spatial analysis and machine learning tasks.

- **Demonstrate a Logical Workflow**  
  To guide users through a logical progression, from setup and data manipulation to advanced statistical modelling and optimisation.

- **Explore Key Libraries**  
  To showcase the power of the modern Python geospatial stack, including `GeoPandas`, `OSMnx`, `PuLP`, and the `PySAL` ecosystem.

- **Bridge Theory and Practice**  
  To connect theoretical concepts like spatial autocorrelation and accessibility to practical applications like site selection and hotspot analysis.

## Notebooks Overview

The notebooks are designed to be followed sequentially, with each one building on concepts from the last:

- **00_Setup_Demo.ipynb**  
  Verifies the Conda environment and demonstrates basic `geopandas` and `shapely` operations to confirm the core libraries are installed and working.

- **01_Site_Optimization_Synthetic.ipynb**  
  Implements heuristic-based approaches for facility location using synthetic demand points, introducing concepts like K-Means clustering and greedy coverage models.

- **02_Spatial_Clustering_Demo.ipynb**  
  Explores unsupervised machine learning for spatial data, using K-Means and DBSCAN to identify spatial clusters and noise.

- **03_Spatial_Interpolation_Basic.ipynb**  
  Introduces methods for predicting values at unsampled locations (e.g., temperature maps) using IDW and machine learning regressors.

- **04_Service_Area_Analysis_Buffers_and_Isochrones.ipynb**  
  Compares simple distance buffers with realistic network-based service areas (isochrones) to model accurate catchment zones based on travel time.

- **05_Health_Facility_Hierarchy_and_Capability_Modelling.ipynb**  
  Models a real-world scenario by assigning different service levels to facilities to find the nearest appropriate location for a given demand.

- **06_Integrating_Census_Geographies_OA_LSOA_MSOA.ipynb**  
  Performs spatial joins to enrich point data with demographic context using official census geographies.

- **07_Interactive_Facility_Scenario_Explorer.ipynb**  
  Creates an interactive tool using `ipywidgets` and `ipyleaflet` to explore "what-if" scenarios by adding facilities and visualising service impact in real time.

- **08_Network_Based_Accessibility_Analysis_with_OSMNx.ipynb**  
  Performs network analysis using `OSMnx` to calculate travel times from residential areas to services, highlighting access disparities.

- **09_Capacitated_Facility_Location_Optimization_with_PuLP.ipynb**  
  Uses the `PuLP` library to solve the capacitated facility location problem, optimising cost under facility capacity constraints.

- **10_Spatial_Statistical_Hotspot_Detection_and_Cluster_Analysis.ipynb**  
  Applies spatial statistics (`Moran's I` and `LISA`) to identify statistically significant hotspots, cold spots, and spatial outliers.

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/RossTylr/Spatial-ML.git
cd Spatial-ML
