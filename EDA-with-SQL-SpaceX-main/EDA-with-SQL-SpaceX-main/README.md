This module focuses on Exploratory Data Analysis (EDA) using SQL to interact with the SpaceX dataset. By loading the processed data into a relational database, we perform structured queries to quantify performance metrics, mission success rates, and operational trends.

Database Integration: Established a connection to a SQLite database and loaded the cleaned SpaceX CSV data into a structured table named SPACEXTABLE.

Operational Identification: Queried unique launch site names and filtered records based on specific string patterns to isolate regional performance.

Quantitative Aggregation: Calculated total and average payload masses for specific customers and booster versions, such as NASA (CRS) and the F9 v1.1.

Milestone Tracking: Identified historical firsts, such as the initial successful ground pad landing, using temporal aggregate functions.

Complex Filtering: Executed multi-condition queries to isolate boosters that achieved success under specific constraints, including drone ship landings with payloads between 4,000 and 6,000 kg.

Success Rate Profiling: Categorized and ranked the total count of mission outcomes and landing results to provide a statistical baseline for success.

Advanced Subqueries: Utilized nested SQL queries to extract booster versions associated with the maximum payload mass recorded in the dataset.

Temporal Analysis: Performed string manipulation on date fields to analyze monthly failure patterns and rank landing outcomes within specific historical windows.

Output
A series of structured insights that quantify the historical performance of Falcon 9. These SQL-driven results serve as the analytical foundation for the project, validating the dataset's integrity and highlighting the most significant variables for subsequent machine learning stages.
