# earthquake-analysis
Python script for analyzing yearly earthquake counts using FDSN catalogs (USGS, ISC, EMSC, etc.). Generates time series plots and CSV outputs. Default region is global, but users can easily define custom geographic coordinates.

## Features
- Yearly earthquake counts
- Custom magnitude
- Different catalogs (USGS, ISC, EMSC, EARTHSCOPE, ETH, GEONET, ORFEUS, EPOSFR, BGR, INGV)
- CSV export
- Plot visualization

## Instalation
Clone this repository
Create virtual environment: python -m venv .venv
Activate virtual environment: source .venv/bin/activate
Install requirements: python -m pip install -r requirements.txt

## Disclaimer
This repository provides tools for downloading and visualizing earthquake data from external sources (FDSN catalogs such as USGS, ISC, EMSC). The author does not guarantee the accuracy, completeness, or reliability of the data and is not responsible for any conclusions drawn from their use. Users are responsible for verifying data and interpreting results.

## Usage
By default, the script uses global coordinates. To analyze a different region, modify the coordinates in the regions dictionary. You can set the parameters of your analysis in parameters structure in code.

```python
'world': {'type': 'box', 'coords': [-90.0, 90.0, -180.0, 180.0]}
# parameters
params = {
    'catalog_keys': usgs,  # select catalog
    'place_names': world,  # select area
    'minmag': 4,           # minimum magnitude
    'years': range(1980, 2026)
}
