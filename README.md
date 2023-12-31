# bootcamp_final_2023-ellenalamont17
Repository for Earth Data Analytics Bootcamp 2023

[![DOI](https://zenodo.org/badge/728890558.svg)](https://zenodo.org/doi/10.5281/zenodo.10293286)

---

# Habitat suitability model for Sorghastrum nutans, a grass native to North America

![Native Grasslands](https://i.guim.co.uk/img/media/bcc734e9651df1a711870c60728e9e46175dda1c/0_62_2048_1229/master/2048.jpg?width=620&dpr=2&s=none)

*Photo of native grasslands. Photo Credit: [The Guardian](https://www.theguardian.com/environment/2021/nov/05/americas-native-grasslands-disappearing)*

## About this project

Native grasslands account for nearly a quarter of ground surface vegetative cover, but have suffered significant global losses in habitat. While anthropogenic encroachment has contributed to these losses, dramatic changes in climate over the last few decades has taken a toll on grassland ecosystems (Bond, 2008). Consequently, native grasslands are endangered ecosystems, posing economic and ecological threats. Unfortunately, given the complications of a changing climate, restoration of native grasslands is all but simple. Efforts to rebuild and conserve grassland ecosystems now require careful planning and must account for future changes in climate inorder to build ecologic resilence (Kane et al., 2017). Ecologic planning will have to account for longer duration droughts, increased temperatures, and more variable extreme precipitation events predicted by climate forecasts. The time available to understand, conserve, and restore these critical ecosystems are shrinking rapidly, required immediate action.

The purpose of this project is to create a habitat suitability model for one variety of native grass, Sorghastrum nutans, more commonly known as yellow indian grass or wood grass. This grass is found largely in eastern North America but has been observed in limited, select locations globally. The model will combine several soil, topography, and climate datasets to assess suitability. 

**References**

Bond, W.J. (2008). What limits trees in C4 grasslands adn savannas? Annual Review of Ecology, Evolution, and Systematics. v39, p641-659. doi: 10.1146/annurev.ecolsys.39.110707.173411

Kane, Kristen, Diane Debinski, Chris Anderson, John Scasta, David Engle, and James Miller (2017). Using regional climate projections to guide grassland community restoration in the face of climate change. Frontiers Plant Science. v8. https://doi.org/10.3389/fpls.2017.00730

---

## About this notebook

This notebook uses the earth-data-analytics-env and additional import of the xarray-spatial (xrspatial) package.

This code is memory intensive and often crashes codespaces. I recommend running on a desktop with locally downloaded datasets.

Imports, directories, and global variables are defined at the beginning of the notebook. Note that the appropriate UTM zone for the study area should be defined in the global variables section. This is used to reproject data throughout the notebook. The URL for the grassland units is hardcoded into the code and does not need changed, only specific grasslands selected. For the POLARIS soil data, a function is included to autogenerate URLs depending on soil variable, statistic, and soil depth of interest. SRTM URLs are also static, but the type of product created from the elevation can be manipulated. For the Maca climate data, a specific URL will need assigned depending on the specific scenario to be analyzed. The code has not yet been modularized for simple selection like the with soil data. 
