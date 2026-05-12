# Data-Collection-SpaceX-Web-Scraping
Web scraping module that extracts Falcon 9 launch records from a static Wikipedia snapshot, parses the launch table with BeautifulSoup, cleans the data, and builds a structured DataFrame to complement the SpaceX REST API dataset

Web Scraping: Falcon 9 Launch Data
This module collects Falcon 9 launch records by scraping a static snapshot of the “List of Falcon 9 and Falcon Heavy launches” Wikipedia page. The goal is to extract structured launch information that complements the SpaceX REST API dataset.

Process Summary
Performed an HTTP GET request to a fixed Wikipedia revision for reproducibility.

Parsed the HTML using BeautifulSoup.

Identified the correct launch table among multiple tables on the page.

Extracted and cleaned column names (removing links, superscripts, and annotations).

Parsed each launch row to retrieve:

- Flight number

- Date and time

- Launch site

- Payload and payload mass

- Orbit

- Customer

- Launch outcome

- Booster version and landing result

Cleaned inconsistent formatting and normalized values.

Built a structured Pandas DataFrame ready for merging with the API dataset.

Output
A clean, structured dataset containing Falcon 9 launch records scraped from Wikipedia, used to validate and enrich the API‑collected data.
