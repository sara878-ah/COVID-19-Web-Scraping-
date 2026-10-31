# COVID-19 Web Scraping | Python

A Python mini-project that extracts COVID-19 country statistics from the Worldometers coronavirus table, cleans selected fields with pandas, and exports the result as a CSV dataset.

## Project Workflow

1. Request the source webpage with `requests`.
2. Locate the country statistics table using BeautifulSoup.
3. Extract country, total cases, and total deaths fields.
4. Clean commas and convert numeric fields using pandas.
5. Save the processed table to `Data.csv` (and optionally `Data.xlsx` when running the script).

## Tools & Libraries

- Python
- requests
- BeautifulSoup (`beautifulsoup4`)
- pandas
- openpyxl (for Excel export)

## Repository Files

| File | Description |
| --- | --- |
| [covid_19_web_scraping.py](covid_19_web_scraping.py) | Python script for extracting and cleaning the data |
| [Data.csv](Data.csv) | Previously exported country-level dataset |

## Run Locally

```bash
pip install pandas requests beautifulsoup4 openpyxl
python covid_19_web_scraping.py
```

The script writes output files to your current working directory.

## Important Notes

- The committed `Data.csv` is a **saved data snapshot**, not continuously updated COVID-19 statistics.
- The current script depends on the source website's HTML table structure and fixed row positions. Changes to the website may require updating the extraction logic.
- `Data.xlsx` can be generated locally by the script, but it is **not included** in this repository.

## Skills Demonstrated

Web scraping · HTML parsing · pandas data cleaning · numeric conversion · CSV export
