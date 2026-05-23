# NCOS Mesa Vegetation Monitoring: Effects of Prescribed Burn on Native and Non-Native Grass Cover

This repository contains data, code, and outputs for an analysis of vegetation change on the 
North Campus Open Space (NCOS) Mesa Perennial Grassland at UC Santa Barbara. The project examines how a 2023 prescribed burn affected native and non-native grass percent cover across seven permanent monitoring transects (GL-prefix) surveyed annually from 2021 to 2025. Analysis includes time series visualization, species-level percent cover change, and statistical testing. This project was completed as a final project for ENVS 193DD: Data Science for Environmental Studies.

## File Structure

```
ENVS-193DD-project-main/
├── code/
│   ├── Background.qmd
│   ├── exploratory-visualization1.qmd
│   ├── exploratory-visualization2.qmd
│   ├── stats.qmd
│   ├── storymap_structure_outline.qmd
│   ├── timeline-checkin.qmd
│   ├── visualizations.qmd
│   └── wrangling-brainstorm.qmd
├── data/
│   ├── raw/
│   │   ├── veg.csv
│   │   └── vp_veg_metadata.csv
│   │   └── NOAA-weather-data.csv
│   └── processed/
├── outputs/
│   ├── fig_1.png
│   ├── fig_2.png
│   ├── figure_3.png
│   ├── figure_4.png
│   └── ttest_table.png
└── README.md
```

## Dependencies

## Dependencies

This project uses R and the following packages:

- `tidyverse` — data wrangling and visualization
- `janitor` — data cleaning
- `here` — relative file paths
- `ggrepel` — label placement in figures
- `cowplot` — figure layout and alignment
- `ggtext` — markdown text rendering in figures (italic species names)
- `flextable` — t-test results table
- `webshot2` — saving flextable as image
- `naniar` — missing data visualization
- `patchwork` — combining multiple plots
- `scales` — axis formatting

Install all packages with:

```r
install.packages(c("tidyverse", "janitor", "here", "ggrepel", "cowplot", 
                   "ggtext", "flextable", "webshot2", "naniar", "patchwork", "scales"))
```

## Rendered Documents

- [Timeline Check-in](https://github.com/lperusa7/ENVS-193DD-project-main/blob/main/code/timeline-checkin.pdf)