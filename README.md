# Urbanization and native bees in Bogotá

For my Yale Environmental Data Science capstone, I want to understand how
urban development relates to the number of native bee species recorded
along Bogotá

## Research question

How is the proportion of urban infrastructure around each sampling site
associated with recorded native bee richness, after accounting for sampling
effort and local floral richness?

## Data sources

- [Jardín Botánico de Bogotá bee and floral resource survey](https://doi.org/10.15472/o3jie0).
  The survey includes 236 bee records from 55 sites sampled in 2021–2022.
  It also provides site coordinates, sampling effort, and measurements of
  floral resources.
- [MapBiomas Colombia, Collection 3](https://colombia.mapbiomas.org/descargas/mapas-de-las-colecciones/).
  I will use the 2021 and 2022 land-cover maps to estimate the proportion of
  urban infrastructure around each site.

## Repository structure

- `raw_data/` contains instructions for downloading the original survey data.
- `clean_data/` is where the notebook saves the CSV it generates.
- `scripts/` contains the R notebook used to preprocess the bee records.
- `figures/` is for maps and plots I will make later in the project.

## First preprocessing step

In `scripts/01_preprocess_bee_data.ipynb`, I downloaded the original survey ZIP, extracted the bee records, and read the tab-separated file into R. I checked the number of rows and saved all 236 records as a CSV for later analysis.
