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

## Results

### Accessibility to Healthcare and Supermarkets

Using road-network distances calculated from sample locations across Christchurch, the analysis produced the following accessibility metrics:

| Metric | Healthcare | Supermarket |
|------|------|------|
| Mean distance | **4.46 km** | **3.40 km** |
| Median distance | **4.13 km** | **2.86 km** |
| Maximum distance | **14.20 km** | **12.78 km** |

---

## Key Findings

### Central Christchurch shows the highest service accessibility

Healthcare and supermarket locations are concentrated in the central urban area.  
As a result, grid points near the city centre have the shortest travel distances to essential services.

---

### Peripheral areas show significantly longer travel distances

Outer suburban and fringe areas experience much longer network travel distances, in some cases exceeding **12–14 km** to the nearest healthcare facility.

---

### Supermarket accessibility is generally higher than healthcare accessibility

Across the sampled locations:

- Average distance to supermarkets: **3.4 km**
- Average distance to healthcare services: **4.5 km**

This reflects a broader spatial distribution of supermarkets compared with healthcare facilities.

---

## Visualisation

### Healthcare Accessibility

![Healthcare Accessibility Map](<img width="2819" height="2970" alt="healthcare_accessibility_map" src="https://github.com/user-attachments/assets/9d46184f-8f83-4756-a396-17d897af60a3" />
)

This map illustrates road-network distance to the nearest healthcare service across Christchurch.

- Dark colours indicate better accessibility  
- Lighter colours represent longer travel distances  

---

### Supermarket Accessibility

![Supermarket Accessibility Map](<img width="2819" height="2970" alt="supermarket_accessibility_map" src="https://github.com/user-attachments/assets/71c452ef-4c44-435f-ad34-a5c8dde272a0" />
)

This map shows accessibility to supermarkets using the same network-distance approach.

---

## Interpretation

The results highlight a clear spatial accessibility gradient across Christchurch:

- **Central Christchurch → higher service accessibility**
- **Peripheral areas → reduced accessibility**

This pattern reflects the concentration of services in the central urban area and the lower service density in outer suburbs.
