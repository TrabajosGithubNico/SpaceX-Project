# Data-Collection-SpaceX-API
The SpaceX API provides structured information about all past launches. In this notebook, we retrieve the raw launch records, normalize the JSON response, and enrich the dataset by performing additional API calls to extract detailed information about rockets, payloads, launch sites, and core stages.

Sent an HTTP GET request to the SpaceX /v4/launches/past endpoint to retrieve all historical launch records.

Converted the nested JSON response into a structured DataFrame using JSON normalization.

Filtered out launches with multiple cores or multiple payloads to maintain a consistent dataset.

Extracted key identifiers from each launch record, including:

- Rocket ID

- Payload ID

- Launchpad ID

- Core ID

Performed additional API calls to retrieve detailed metadata:

- Rocket information (booster version, configuration)

- Payload details (mass, orbit, customer)

- Launch site information (site name, coordinates)

- Core attributes (block, reuse count, landing type, landing success, gridfins, legs)

Cleaned and merged all enriched fields into a unified dataset.

Restricted the dataset to Falcon 9 launches to support landing‑success prediction.

Output:

A clean, enriched dataset containing detailed Falcon 9 launch records collected directly from the SpaceX REST API. This dataset serves as the primary structured source for analysis and is later combined with the web‑scraped dataset to validate and enhance data completeness.
