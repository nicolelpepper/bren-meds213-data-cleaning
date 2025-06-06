# Cleaning the shorebird survey data 


## The data set

ARCTIC SHOREBIRD DEMOGRAPHICS NETWORK [https://doi.org/10.18739/A2222R68W](https://doi.org/10.18739/A2222R68W)

Data set hosted by the [NSF Arctic Data Center](https://arcticdata.io) data repository 

Field data on shorebird ecology and environmental conditions were collected from 1993-2014 at 16 field sites in Alaska, Canada, and Russia.

![Shorebird, copyright NYT](https://static01.nyt.com/images/2017/09/10/nyregion/10NATURE1/10NATURE1-superJumbo.jpg?quality=75&auto=webp)

Data were not collected every year at all sites. Studies of the population ecology of these birds included nest-monitoring to determine the timing of reproduction and reproductive success; live capture of birds to collect blood samples, feathers, and fecal samples for investigations of population structure and pathogens; banding of birds to determine annual survival rates; resighting of color-banded birds to determine space use and site fidelity; and use of light-sensitive geolocators to investigate migratory movements. 

Data on climatic conditions, prey abundance, and predators were also collected. Environmental data included weather stations that recorded daily climatic conditions, surveys of seasonal snowmelt, weekly sampling of terrestrial and aquatic invertebrates that are prey of shorebirds, live trapping of small mammals (alternate prey for shorebird predators), and daily counts of potential predators (jaegers, falcons, foxes). Detailed field methods for each year are available in the `ASDN_protocol_201X.pdf` files. All research was conducted under permits from relevant federal, state, and university authorities.

See `01_ASDN_Readme.txt` provided in the [course data repository](https://github.com/UCSB-Library-Research-Data-Services/bren-meds213-spring-2024-class-data) for full metadata information about this data set.

## Data & File Overview

### File list:
The data used for this is stored in a folder `data` that is broken into subfolders `raw/` for raw data and `processed/` for processed data.

The `raw/` folder contains:

- `01_ASDN_Readme.txt` a read me file for the Artic Shorebird Demographics Network (ASDN) data
- `ASDN_Daily_species.csv` raw data from ASDN containing a record of the species (birds and mammals) encountered during field work each day at each site.
- `ASDN_Snow_survey.csv` raw data from ASDN containing periodic records of snow cover remaining at the sites.
The `processed/` folder contains cleaned version of the ASDN datasets.
- `all_cover_fixed_pepper.csv` a cleaned version of the ASDN datasets
- `snow_cover.csv` a cleaned version of the ASDN snow cover dataset filtered to the snow_cover column.
- `species_presence.csv` a cleaned version of the ASDN daily species dataset

The file organization is as follows:
```
data
|
├── raw/
│    ├── 01_ASDN_Readme.txt
│    ├── ASDN_Daily_species.csv
│    └── ASDN_Snow_survey.csv
│
├── processed/
│    ├── all_cover_fixed_pepper.csv
│    ├── snow_cover.csv 
└──  └── species_presence.csv
```

Additional Related Data:


Data Versions:

