*UCSB MEDS* - *EDS 213 - Database Management*

# Cleaning the shorebird survey data 
![Database Management](https://img.shields.io/badge/Database_Managements-cornflowerblue?style=for-the-badge&logo=R) ![UCSB MEDS](https://img.shields.io/badge/UCSB%20MEDS-yellow?style=for-the-badge) 

**Author:** Nicole Pepper

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

### Additional Related Data:
Additional data from the ASDN can be found on the NSF Arctic Data Center at [this link](https://arcticdata.io/catalog/view/doi:10.18739/A2222R68W).

### Data Versions:
This data was accessed and forked from a GitHub repo by the UCSB Library Research Data Services at [this link](https://github.com/UCSB-Library-Research-Data-Services/bren-meds213-data-cleaning).

### Data Specific Information:
##### `all_cover_fixed_pepper.csv` a cleaned version of the ASDN datasets:
- Number of variables: 11
- Number of cases/rows: 42,829
- Missing data code: NA, NAs were given to all values where total cover didn't add up to 100%
- Variable list:
  
| Variable      | Description                                                | Type                 |
|---------------|------------------------------------------------------------|----------------------|
| Site          | Four-letter unique code of site where data was collected   | string               |
| Year          | Year that data was collected                               | integer              |
| Date          | Date that data was collected                               | date                 |
| Plot          | Name of study plot where data was collected                | string               |
| Location      | Name of dedicated snow-survey location     | string               |
| Snow_cover    | Percent cover of snow cover                    | integer              |
| Water_cover   | Percent cover of water water                                     | integer              |
| Land_cover    | Percent cover of exposed land                              | integer              |
| Total_cover   | Sum of the three cover columns - sums to 100%.  | integer              |
| Observer      | Name of person who conducted the survey                        | string               |
| Notes         | Futher comments on the survey                        | string              |

### Sharing & Access Information:

##### License: [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/)
Please acknowledge this dataset and the authors in any analysis, publication, presentation, or other output that uses these data. If you use the full dataset, we suggest you cite it as:

##### How to Cite Data:
Lanctot, RB, SC Brown, and BK Sandercock. 2016. Arctic Shorebird Demographics Network. NSF Arctic Data Center. doi: [https://arcticdata.io/catalog/view/doi:10.18739/A2222R68W](https://arcticdata.io/catalog/view/doi:10.18739/A2222R68W).

If you use data from only one or a few sites, we suggest you cite data for each site as per this example, using the corresponding site PIs as the authors:
Lanctot, R.B. and Saalfeld, S.T. 2016. Barrow, 2014. Arctic Shorebird Demographics Network. NSF Arctic Data Center. [Insert site-specific DOI here]

[Link to specific dois](https://arcticdata.io/catalog)



  
