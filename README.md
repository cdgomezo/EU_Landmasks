# Country Mask Generator

This repository contains a Python notebook and scripts for generating country-level land masks
at configurable resolutions using shapefiles (e.g. NUTS regions).

## Contents
- `Landmask_NUTS.ipynb`: Jupyter Notebook for generating masks.
- `NUTS_RG_20M_2024_4326_masks_**.nc`: Example NetCDF output at different resolutions.
- `mask_1x2deg.nc`: Example mask at 1°×2° resolution.

## Requirements
- Python ≥3.9
- geopandas
- rasterio
- xarray
- numpy

## Usage
Download the NUTS data as shape file (*.shp) from: https://ec.europa.eu/eurostat/web/gisco/geodata/statistical-units/territorial-units-statistics
Run the notebook to reproduce results with your own shapefile.

```bash
jupyter notebook Landmask_NUTS.ipynb
