# Data-Wrangling-SpaceX-

This module processes and prepares the combined SpaceX datasets—collected from the REST API and web scraping—into a clean, consistent, and analysis‑ready format. The goal is to standardize all variables, resolve inconsistencies, handle missing values, and merge enriched information into a unified dataset suitable for exploratory analysis and machine‑learning modeling.

Filtered out inconsistent launch records, such as entries with multiple cores or multiple payloads.

Extracted single‑value fields from nested JSON structures and list‑based attributes.

Converted date strings into standardized year‑based fields for temporal analysis.

Identified and handled missing values, including imputing payload mass using the mean.

Cleaned categorical fields (orbit, landing outcome, booster version, launch site).

Normalized formatting across numeric and text variables to ensure consistency.

Merged the enriched API dataset with the cleaned web‑scraped dataset.

Prepared the final feature table by selecting relevant variables for prediction tasks.

Applied one‑hot encoding to categorical variables and cast all features to float64.

Output

A fully cleaned, standardized, and feature‑engineered dataset combining API and web‑scraped information. This dataset is ready for modeling tasks such as predicting Falcon 9 landing success and supports all subsequent analysis in the project.
