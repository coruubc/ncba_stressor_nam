# ncba_stressor
Code for generating the the National Climate-Biodiversity Assessment multi-stressor map

# Obejctive
Our chapter aims to assess the interaction between climate and other non-climatic stressors on biodiversity.

# Instructions
Use data from O’Hara et al. (2021) to map out multi-stressors in the EEZs of USA, Canada and Mexico. Perhaps make a figure with panels with some combination of [Fig 1](https://www.science.org/cms/10.1126/science.abe6731/asset/3f5c83c0-9da0-49b9-a17c-7a4624f70421/assets/graphic/372_84_f1.jpeg) and [Fig 2](https://www.science.org/cms/10.1126/science.abe6731/asset/fe156707-b72f-43d0-8874-93a1571053b3/assets/graphic/372_84_f2.jpeg)

- Code and data are available from the Knowledge Network for Biocomplexity - [KNB](https://knb.ecoinformatics.org/view/doi:10.5063/SJ1J03)

- Available code on [GitHub](https://github.com/oharac/bd_chi)

# Time line

- Map draft for July 30

# Data

## Data and code: At-risk marine biodiversity faces extensive, expanding, and intensifying human impacts**

*This work is dedicated to the public domain under the Creative Commons Universal 1.0 Public Domain Dedication. To view a copy of this dedication, visit https://creativecommons.org/publicdomain/zero/1.0/.*

- `bd_chi_master.zip`, Zip file containing all code and generated data from Github repository: https://github.com/oharac/bd_chi. The [README.md](https://github.com/oharac/bd_chi?tab=readme-ov-file#readme) in the root directory describes the file structure and order of operations to replicate the results.


# References
Casey C. O’Hara et al. ,At-risk marine biodiversity faces extensive, expanding, and intensifying human impacts.Science372,84-87(2021).DOI:10.1126/science.abe6731


# Note: This repository was cloned from [oharac GitHub](https://github.com/oharac/bd_chi). The original `ReadMe` is below for reference

## Files used / modified

- `ms_figs/fig2_impact_intens_map_3panel.Rmd`, this became `ncba_fig2`



## At-risk marine biodiversity faces extensive, expanding, and intensifying human impacts

Repository for code and generated data for "At-risk marine biodiversity faces extensive, expanding, and intensifying human impacts" by Casey C. O'Hara, Melanie Frazier, Benjamin S. Halpern.

External data are freely available from:

* Species range maps: [IUCN Red List of Threatened Species spatial data download](https://www.iucnredlist.org/resources/spatial-data-download)
* Bird species range maps: [BirdLife International Data Zone](http://datazone.birdlife.org/species/requestdis)
* Species information: [IUCN Red List API](https://apiv3.iucnredlist.org/)
* Stressor distributions: [Recent pace of change in human impact on the world's ocean: Cumulative impacts. Knowledge Network for Biocomplexity](doi:10.5063/F12B8WBS)

To replicate the analysis, download necessary data and set up an external directory for these datasets and large files generated during the analysis process.

Run all scripts in the `_setup` directory in numeric order.  It will be necessary to point the scripts to the proper locations in your data directory.  The `common_fxns.R` script may be helpful for setting filename objects to various data locations.

Run all scripts in the root project directory, in numeric order.

Finally, if you wish to generate the figures, run the appropriate scripts in the `ms_figs` directory.

Overview of file structure:

* `_setup`: scripts for pre-processing of data on threats, species range distributions, and stressor distributions.
* `_raw`: lookup tables created by the project team to facilitate the analysis.
* `_data`: data drawn from the IUCN API; note that the setup scripts also place larger IUCN files on the external data directory.
* `_spatial`: spatial data and maps generated in the setup scripts.  Again, note that the setup scripts place larger spatial files on the external data directory.
* `_output`: all finalized datasets are stored here, including rasters of impacts, intensification, stressor footprints, and taxonomic species richness maps.
* `figs`: temporary figure storage
* `ms_figs`: code to generate figures for manuscript
* `ms_tables`: code to generate tables for manuscript



