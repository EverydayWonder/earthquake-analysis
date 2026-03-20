# earthquake-analysis
Python script for analyzing yearly earthquake counts using FDSN catalogs (USGS, ISC, EMSC, etc.). Generates time series plots and CSV outputs. Default region is global, but users can easily define custom geographic coordinates.

## Features
- Yearly earthquake counts
- Custom magnitude
- Different catalogs (USGS, ISC, EMSC, EARTHSCOPE, ETH, GEONET, ORFEUS, EPOSFR, BGR, INGV)
- CSV export
- Plot visualization

## Usage
By default, the script uses global coordinates:

```python
'world': {'type': 'box', 'coords': [-90.0, 90.0, -180.0, 180.0]}
To analyze a different region, modify the coordinates in the regions dictionary.

## Requirements
obspy
matplotlib
