This module features a real-time, interactive web application built using Plotly Dash to visualize SpaceX launch records. The dashboard allows for dynamic data exploration, enabling users to analyze mission success factors through customizable filters and synchronized visualizations.  

Interactive Dropdown: Implemented a searchable selection menu to switch between aggregate data for "All Sites" or specific performance metrics for individual launch sites like KSC LC-39A or VAFB SLC-4E.

Dynamic Success Analysis: Developed a reactive pie chart that updates based on the selected site to show either the total success distribution across all locations or the success-to-failure ratio for a specific site.

Payload Range Filtering: Integrated a dual-handle RangeSlider that allows users to filter mission data by payload mass, ranging from 0 to 10,000 kg.

Correlation Visualization: Created a scatter plot to analyze the relationship between payload mass and landing success.

Booster Version Categorization: Enhanced the scatter plot by color-coding data points based on the Booster Version Category, allowing users to observe how different rocket iterations perform under various cargo loads.

Reactive Callbacks: Utilized Dash decorators to link user inputs (dropdown and slider) to the graphs, ensuring that all visualizations update instantly without reloading the page.

Output
A fully functional, interactive dashboard that provides a high-level overview and deep-dive capabilities into SpaceX’s launch history. This tool simplifies the identification of trends—such as the correlation between payload weight and booster reliability—making it an essential asset for final project reporting and data-driven storytelling.
