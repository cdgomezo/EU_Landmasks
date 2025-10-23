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

### NUTS to ISO3 Mapping

| NUTS Code | ISO3 | Country |
|:-----------|:------|:-----------------------------|
| AL | ALB | Albania |
| AT | AUT | Austria |
| BA | BIH | Bosnia and Herzegovina |
| BE | BEL | Belgium |
| BG | BGR | Bulgaria |
| CH | CHE | Switzerland |
| CY | CYP | Cyprus |
| CZ | CZE | Czechia |
| DE | DEU | Germany |
| DK | DNK | Denmark |
| EE | EST | Estonia |
| EL | GRC | Greece *(NUTS uses EL, not GR)* |
| ES | ESP | Spain |
| FI | FIN | Finland |
| FR | FRA | France |
| HR | HRV | Croatia |
| HU | HUN | Hungary |
| IE | IRL | Ireland |
| IS | ISL | Iceland |
| IT | ITA | Italy |
| LI | LIE | Liechtenstein |
| LT | LTU | Lithuania |
| LU | LUX | Luxembourg |
| LV | LVA | Latvia |
| ME | MNE | Montenegro |
| MK | MKD | North Macedonia |
| MT | MLT | Malta |
| NL | NLD | Netherlands |
| NO | NOR | Norway |
| PL | POL | Poland |
| PT | PRT | Portugal |
| RO | ROU | Romania |
| RS | SRB | Serbia |
| SE | SWE | Sweden |
| SI | SVN | Slovenia |
| SK | SVK | Slovakia |
| TR | TUR | Türkiye |
| UA | UKR | Ukraine |
| UK | GBR | United Kingdom *(NUTS uses UK, not GB)* |
| XK | XKO | Kosovo *(unofficial ISO3 used in EU datasets)* |


```bash
jupyter notebook Landmask_NUTS.ipynb
