This module implements interactive maps to visualize the geographical distribution and strategic positioning of SpaceX launch sites. By using Folium, we transform coordinate data into a dynamic visual environment to analyze proximity to infrastructure and regional launch success rates.

Interactive Mapping: Initialized a world map centered on the NASA Johnson Space Center using folium.Map to serve as the analytical canvas.

Site Localization: Added highlighted circles and markers to identify the four primary SpaceX launch sites: CCAFS LC-40, CCAFS SLC-40, KSC LC-39A, and VAFB SLC-4E.

Performance Visualization: Developed a color-coding system for launch outcomes—green for successful landings and red for failures—applied via custom marker icons.

Marker Clustering: Implemented MarkerCluster to efficiently manage high-density launch data, grouping multiple missions at the same site into manageable, interactive clusters.

Proximity Analysis: Integrated a Mouse Position plugin to capture real-time coordinates and utilized the Haversine formula to calculate the physical distance (in km) between launch sites and nearby geographical features.

Strategic Mapping: Visualized proximity to critical infrastructure, such as coastlines, railways, and highways, to understand the safety and logistical requirements of aerospace operations.

Output
An interactive geographical dashboard that reveals the spatial logic behind SpaceX operations. This analysis confirms that launch sites are strategically located near coastlines (for safety) and major transport infrastructure, while providing a visual baseline of site-specific success rates.
