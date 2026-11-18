# Data sources

Raw data is not stored in this repository. Each source below lists where to get it and how it must be credited. Cleaned files used by the models are in `cleaned/`.

| Source | Used for | Licence | Link |
| --- | --- | --- | --- |
| Our World in Data, CO2 and greenhouse gas emissions | Country emissions (Part 2) | CC BY 4.0 | https://github.com/owid/co2-data |
| Global Carbon Budget | National CO2 and land-use emissions | CC BY 4.0 | https://globalcarbonbudget.org |
| ERA5 reanalysis (Copernicus Climate Change Service) | Historical temperature and rainfall (Part 2) | Copernicus licence, attribution required | https://cds.climate.copernicus.eu |
| Hansen Global Forest Change (University of Maryland) | Forest loss labels (Part 1) | CC BY 4.0 | https://glad.earthengine.app/view/global-forest-change |
| Sentinel-2 and Landsat imagery, via Google Earth Engine | Satellite image patches (Part 1) | Copernicus licence and public domain | https://earthengine.google.com |
| Global Forest Watch forest carbon flux | Checking carbon estimates (Part 1) | CC BY 4.0 | https://data-api.globalforestwatch.org/dataset/gfw_forest_carbon_net_flux |
| NASA NEX-GDDP-CMIP6 | Future climate scenarios (Part 2) | CC0 | https://developers.google.com/earth-engine/datasets/catalog/NASA_GDDP-CMIP6 |
| World Bank World Development Indicators | GDP, population, urban share (Part 2) | CC BY 4.0 | https://databank.worldbank.org/source/world-development-indicators |
| ND-GAIN Country Index (University of Notre Dame) | Vulnerability and readiness (Part 2) | Free use with citation | https://gain.nd.edu/our-work/country-index/download-data/ |
| EM-DAT (CRED, UCLouvain) | Checking predictions against recorded disasters | Free academic use; raw data may not be shared | https://www.emdat.be |
| NASA/ORNL biomass carbon density 2010 (Spawn et al. 2020), via Google Earth Engine | Carbon per hectare for the carbon estimate (Part 1) | Public domain | https://developers.google.com/earth-engine/datasets/catalog/NASA_ORNL_biomass_carbon_density_v1 |
| Global Forest Watch tree cover loss by country, via Our World in Data | Checking our loss areas (data/cleaned/part1_gfw_check.csv) | CC BY 4.0 | https://ourworldindata.org/grapher/tree-cover-loss |
| Natural Earth, India point-of-view boundaries | Country shapes for the maps | Public domain | https://www.naturalearthdata.com |

EM-DAT's raw data must not be uploaded here. Only our own aggregated counts are shared.
