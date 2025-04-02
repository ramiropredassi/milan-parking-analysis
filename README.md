# Analysis of High-Density Parking Areas in Milan  
*Urban mobility analysis project using GPS Tracks*

## Introduction

In modern cities, managing and optimizing parking is essential for improving mobility and overall quality of life. This project focuses on Milan, Italy, where simulated GPS trajectory data from private vehicles is analyzed to detect areas with high stop density—potential parking zones. The goal is to identify neighborhoods with a high demand for parking, providing insights for urban planning and infrastructure improvements.

## Motivation

My primary motivation for this project was to understand and learn how to use the libraries involved, such as **scikit-mobility**, **GeoPandas**, and **Folium**. I wanted to introduce myself to the field of geospatial data analysis and urban mobility studies while gaining hands-on experience with these powerful tools. This exploration has enabled me to see firsthand how various Python libraries can be integrated to analyze and visualize complex mobility data.

## Methodology

The analysis was conducted through several key steps:

1. **Loading and Visualizing Geospatial Data**  
   - Imported a geographic tessellation of Milan's neighborhoods.
   - Customized the map style to highlight polygon borders and background.
   - **Visual Suggestion:** Include a static or interactive map of the tessellation to provide a visual context of Milan’s neighborhoods.

2. **Processing Mobility Data**  
   - Loaded the GPS data (latitude, longitude, date, and time) of private vehicles.
   - Filtered trajectories to remove points with speeds greater than 150 km/h, ensuring data quality.
   - Applied spatial compression to reduce noise and focus on the core mobility patterns.
   - **Visual Suggestion:** Add a chart (e.g., histogram) showing the distribution of vehicle speeds before and after filtering to highlight data cleaning.

3. **Stop Detection and Clustering**  
   - Detected stops for each user using criteria such as a minimum stop duration of 30 minutes and a spatial radius of 0.3 km.
   - Applied clustering to group nearby stops, identifying high-density parking zones.
   - **Visual Suggestion:** Display an interactive map overlaying detected stops and clusters to visually represent where stops are concentrated.

4. **Mapping and Visualization**  
   - Mapped each stop to the neighborhood tessellation, visualizing stop locations within the city.
   - Created interactive maps using [Folium](https://python-visualization.github.io/folium/), showing individual stops and clusters.
   - Developed a choropleth map to illustrate the number of GPS points per neighborhood, providing a clear view of parking demand across Milan.
   - **Visual Suggestion:** Include a choropleth map alongside detailed charts (such as bar charts or heatmaps) to compare neighborhood-wise GPS point counts.

## Results and Discussion

- **Understanding the Tools:**  
  This project allowed me to delve into the functionalities of various Python libraries, understand how they interact, and see their application in real-world data analysis scenarios.

- **Identification of Critical Areas:**  
  Interactive maps reveal zones with a high density of stops, indicating potential areas where additional parking infrastructure could be beneficial.

- **Temporal and Spatial Analysis:**  
  By grouping stops and analyzing the average duration, the study not only identifies the locations but also the significance of each area based on usage. This analysis suggests that some neighborhoods might benefit from either temporary or long-term parking solutions.

- **Intuitive Visualizations:**  
  The integration of geospatial visualization techniques ensures that the information is accessible and easy to understand, aiding urban planners and municipal authorities in decision-making.  
  **Visual Suggestion:** Supplement the discussion with time-series charts showing stop duration distributions per cluster to further illustrate temporal patterns.

## Conclusions

This study not only demonstrates the potential of mobility data to address critical urban challenges but also serves as a learning journey into geospatial data analysis. By identifying high-density parking areas in Milan, the project guides infrastructure planning towards neighborhoods that need it most while providing practical insights into using powerful Python libraries. The experience gained here lays a strong foundation for future explorations in urban mobility studies.

---

**Where to Add Graphics:**

1. **Geospatial Tessellation Map:**  
   - After the "Loading and Visualizing Geospatial Data" section, include an interactive or static map that shows Milan's neighborhoods with the customized style. This sets the geographic context.

2. **Data Filtering Visuals:**  
   - Insert a histogram or line chart in the "Processing Mobility Data" section to display the distribution of vehicle speeds before and after filtering. This helps illustrate the data cleaning process.

3. **Stop Detection and Clustering Map:**  
   - In the "Stop Detection and Clustering" section, add an interactive map overlay that highlights the detected stops and clusters. This visual can dynamically show the concentration of stops across different neighborhoods.

4. **Choropleth Map and Comparative Charts:**  
   - In the "Mapping and Visualization" section, incorporate the choropleth map along with additional charts (e.g., bar charts or heatmaps) that compare the number of GPS points across neighborhoods, offering a clear visual summary of parking demand.

5. **Temporal Analysis Charts:**  
   - Consider adding time-series charts or scatter plots in the "Results and Discussion" section to depict the duration of stops per cluster, highlighting temporal trends.
