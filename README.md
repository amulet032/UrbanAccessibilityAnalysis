# Urban Accessibility Analysis – Christchurch

Spatial and network-based analysis of accessibility to essential services across Christchurch, New Zealand.

This project explores how easily residents can access key services such as healthcare facilities and supermarkets using road network analysis and geospatial data.

---

## Project Motivation

Accessibility to essential services is an important factor in urban planning and public wellbeing.  
Understanding spatial differences in service access can help identify areas where residents may face longer travel distances or limited service coverage.

This project analyses accessibility patterns across Christchurch using open geospatial datasets and network analysis methods.

---

## Key Questions

- How accessible are essential services across different areas of Christchurch?
- Which suburbs have relatively limited access to services such as healthcare or supermarkets?
- What spatial patterns can be observed in service coverage?

---

## Data Sources

The project uses publicly available geospatial datasets:

- **Road network data** from OpenStreetMap
- **Service locations** (e.g., hospitals, medical centres, supermarkets) from OpenStreetMap
- **Suburb or administrative boundaries** from Stats NZ or Christchurch open data portals

These datasets are combined to perform spatial and network-based accessibility analysis.

---

## Methodology

The analysis workflow includes the following steps:

1. **Data acquisition**
   - Download road network and service locations from OpenStreetMap.

2. **Data preparation**
   - Clean and structure spatial datasets using GeoPandas.
   - Extract relevant service categories.

3. **Network construction**
   - Build a road network graph using OSMNX.
   - Calculate travel distances along the network.

4. **Accessibility analysis**
   - Measure distance or travel time to the nearest essential services.
   - Compare accessibility across suburbs.

5. **Visualisation**
   - Produce maps and charts to illustrate spatial accessibility patterns.

---

## Technologies Used

- Python  
- Pandas  
- GeoPandas  
- OSMNX  
- NetworkX  
- Matplotlib / Folium

---
