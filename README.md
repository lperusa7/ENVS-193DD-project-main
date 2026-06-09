# NCOS Mesa Vegetation Monitoring: Effects of Prescribed Burn on Native and Non-Native Grass Cover

This repository contains data, code, and outputs for an analysis of vegetation change on the 
North Campus Open Space (NCOS) Mesa Perennial Grassland at UC Santa Barbara. The project examines how a 2023 prescribed burn affected native and non-native grass percent cover across seven permanent monitoring transects (GL-prefix) surveyed annually from 2021 to 2025. Analysis includes time series visualization, species-level percent cover change, and statistical testing. This project was completed as a final project for ENVS 193DD: Data Science for Environmental Studies.

## File Structure

```
ENVS-193DD-project-main/.            # Root project directory
├── code/                           
│   ├── ecology.csl                  # Citation style file (Ecology journal format)
│   ├── final_paper.pdf              # Rendered final paper
│   ├── final_paper.qmd              # Quarto document for final paper
│   ├── references.bib               # BibTeX database of all cited references
│   ├── timeline-checkin.pdf         # Rendered timeline check-in
│   └── timeline-ckeckin.qmd         # Quarto document for timeline check-in
├── data/
│   ├── raw/
│   │   ├── NOAA-weather-data.csv    # NOAA weather data
│   │   ├── veg.csv                  # Monitoring report vegetation data
│   │   └── vp_veg_metadata.csv.     # Monitoring report vegetation metadata 
├── outputs/
│   ├── figure_1.png                 # Native vs. non-native grass cover over time figure
│   ├── figure_2.png                 # Sweet and bur clover over time figure
│   ├── figure_3.png                 # Mean percent cover change before and after the burn figure
│   ├── figure_4.png                 # Mean percent cover before and after disturbance figure
│   └── ttest_table.png              # Paired t-test results for the four focal
└── README.md                        # Project overview and file documentation (this file)
```

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

- [Final Paper](https://github.com/lperusa7/ENVS-193DD-project-main/blob/main/code/final_paper.pdf)
- [Timeline Check-in](https://github.com/lperusa7/ENVS-193DD-project-main/blob/main/code/timeline-checkin.pdf)

## Related Repositories

- [Project Proposal](https://github.com/lperusa7/project-proposal)
- [Literature Dissection](https://github.com/lperusa7/literature-dissection)