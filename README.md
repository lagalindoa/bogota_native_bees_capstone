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

- `data/raw/` contains instructions for obtaining the original data.
- `data/processed/` holds the tables produced by the preprocessing scripts.
- `scripts/` contains the code used to clean and analyze the data.
- `results/` is for figures, maps, and summaries.

## First preprocessing step

I will link bee records to sampling sites using the event ID and count
distinct native bee species recorded at each site. The output will keep
all 55 sites and retain sampling effort and floral richness for analysis.
