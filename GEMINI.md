# Hawaiian Airlines On-Time Performance Analysis

## Project Setup
- **Main Notebook**: `hawaiian airlines.ipynb`
- **Data Folder**: `bts_data/` (Store BTS CSV files here)
- **Export Folder**: `exports/` (Generated reports and master CSVs)

## Data Extraction (Critical)
The Bureau of Transportation Statistics (BTS) website uses dynamic PostBacks and tokens that make automated scraping difficult.

If the automated extraction script in the notebook fails:
1.  Go to [BTS Departures](https://www.transtats.bts.gov/ONTIME/Departures.aspx).
2.  Select **Airport** (e.g., HNL), **Airline** (Hawaiian Airlines), **Year**, and **Month**.
3.  Click **Download**.
4.  Rename and save the file to `bts_data/Stats_AIRPORT_YEAR_MONTH.csv` (e.g., `Stats_HNL_2024_01.csv`).

## Execution Flow
1.  Run the **Setup** cell to initialize paths and configurations.
2.  Run **Data Acquisition** (will use local files if downloads fail).
3.  Run **Transformation** to generate the `master_df`.
4.  Run **Analysis** to view the volume vs. punctuality charts.
