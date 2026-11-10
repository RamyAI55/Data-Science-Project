# NYC Rental Listings Analysis

Group project for the Data Science module at The British University in Egypt. The analysis explores how listing prices, room types and availability vary across New York City, then compares short-term Airbnb listings with Craigslist rental listings.

## Project workflow

| Notebook | What it covers |
| --- | --- |
| [Phase 1 · Airbnb data cleaning and exploration](01-airbnb-cleaning-and-eda.ipynb) | Standardizes prices and borough labels, handles missing values, and visualizes price, availability and reviews. |
| [Phase 2 · Rental listing integration](02-rental-listing-integration.ipynb) | Cleans Craigslist listing fields, joins Airbnb summary statistics at neighborhood and borough level, and explores relationships in the combined data. |

The second phase uses borough averages where neighborhood matches are unavailable. Borough-level correlations are exploratory given the five boroughs and the different coverage of the two platforms.

## Run locally

Install dependencies with `python -m pip install -r requirements.txt`. Open the notebooks in Jupyter and run them in order with permitted copies of the input files in the same directory.

- Phase 1 reads `Airbnb_Open_Data.csv` and writes `airbnb_cleaned.csv`.
- Phase 2 reads `nyc_apartments.csv` and the Phase 1 output. It writes `Craigslist_Cleaned.csv` and `airbnb_with_rental_data1.csv`.

This portfolio copy contains the analysis notebooks and excludes listing-level datasets and cached outputs.
