# Life satisfaction vs. life expectancy - Data package

This data package contains the data that powers the chart ["Life satisfaction vs. life expectancy"](https://ourworldindata.org/grapher/life-satisfaction-vs-life-expectancy?tab=table&time=2011..latest&v=1&csvType=filtered&useColumnShortNames=false) on the Our World in Data website.

## CSV Structure

The high level structure of the CSV file is that each row is an observation for an entity (usually a country or region) and a timepoint (usually a year).

The first two columns in the CSV file are "Entity" and "Code". "Entity" is the name of the entity (e.g. "United States"). "Code" is the OWID internal entity code that we use if the entity is a country or region. For normal countries, this is the same as the [iso alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code of the entity (e.g. "USA") - for non-standard countries like historical countries these are custom codes.

The third column is either "Year" or "Day". If the data is annual, this is "Year" and contains only the year as an integer. If the column is "Day", the column contains a date string in the form "YYYY-MM-DD".

The remaining columns are the data columns, each of which is a time series. If the CSV data is downloaded using the "full data" option, then each column corresponds to one time series below. If the CSV data is downloaded using the "only selected data visible in the chart" option then the data columns are transformed depending on the chart type and thus the association with the time series might not be as straightforward.

## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc.. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc..

## About the data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stich together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

### How we process data at Our World In Data
All data and visualizations on Our World in Data rely on data sourced from one or several original data providers. Preparing this original data involves several processing steps. Depending on the data, this can include standardizing country names and world region definitions, converting units, calculating derived indicators such as per capita measures, as well as adding or adapting metadata such as the name or the description given to an indicator.
[Read about our data pipeline](https://docs.owid.io/projects/etl/)

## Detailed information about each time series


## Life Expectancy,age 0 – UN WPP
Period life expectancy for individuals who have reached age 0. Estimates are expressed as the expected age at death, not as years left to live.
Last updated: July 12, 2024  
Date range: 1950–2023  
Unit: years  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
UN, World Population Prospects (2024) – processed by Our World in Data

#### Full citation
UN, World Population Prospects (2024) – processed by Our World in Data. “Life Expectancy,age 0 – UN WPP” [dataset]. United Nations, “World Population Prospects” [original data].
Source: UN, World Population Prospects (2024) – processed by Our World In Data

### What you should know about this data

### Source

#### United Nations – World Population Prospects
Retrieved on: 2024-07-11  
Retrieved from: https://population.un.org/wpp/Download/  


## Self-reported life satisfaction – WHR
Average of survey responses to the 'Cantril Ladder' question in the Gallup World Poll. The survey question asks respondents to think of a ladder, with the best possible life for them being a 10, and the worst possible life being a 0.
Last updated: June 9, 2024  
Next update: June 2025  
Date range: 2011–2023  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
World Happiness Report (2012-2024) – with major processing by Our World in Data

#### Full citation
World Happiness Report (2012-2024) – with major processing by Our World in Data. “Self-reported life satisfaction – WHR” [dataset]. Wellbeing Research Centre, “World Happiness Report 2024”; Various sources, “Population” [original data].
Source: World Happiness Report (2012-2024) – with major processing by Our World In Data

### What you should know about this data
* The Cantril ladder asks respondents to think of a ladder, with the best possible life for them being a 10 and the worst possible life being a 0. They are then asked to rate their own current lives on that 0 to 10 scale.
* The rankings are calculated by the source based on nationally representative samples for the three years prior to the year of the report, so that data for the 2024 report will draw from survey data from 2021-2023. We show the data for final year of the three-year survey period, i.e. we show the 2021-2023 survey data as 2023.
* The only exception is the data for the 2012 report, which uses survey data from 2005-2011, we show this data as the final year of the survey data - 2011.
* The number of people and countries surveyed varies year to year, but typically more than 100,000 people in 130 countries participate in the Gallup World Poll each year.
* The rankings are based entirely on the survey scores, using the Gallup weights to make the estimates representative.
* The data is the compilation of all previous World Happiness Reports, which can be found at https://worldhappiness.report/archive/.

### Sources

#### Wellbeing Research Centre – World Happiness Report
Retrieved on: 2024-06-09  
Retrieved from: https://worldhappiness.report/ed/2024/  

#### Various sources – Population
Retrieved on: 2023-03-31  
Retrieved from: https://ourworldindata.org/population-sources  

#### Notes on our processing step for this indicator
Average of regions is calculated by taking a population-weighted average over all countries within that region.


## Population (historical)
Population by country, available from 10,000 BCE to 2023, based on data and estimates from different sources.
Last updated: July 15, 2024  
Next update: July 2026  
Date range: 10000 BCE – 2023 CE  
Unit: people  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
HYDE (2023); Gapminder (2022); UN WPP (2024) – with major processing by Our World in Data

#### Full citation
HYDE (2023); Gapminder (2022); UN WPP (2024) – with major processing by Our World in Data. “Population (historical)” [dataset]. PBL Netherlands Environmental Assessment Agency, “History Database of the Global Environment 3.3”; Gapminder, “Population v7”; United Nations, “World Population Prospects”; Gapminder, “Systema Globalis” [original data].
Source: HYDE (2023); Gapminder (2022); UN WPP (2024) – with major processing by Our World In Data

### What you should know about this data

### Sources

#### PBL Netherlands Environmental Assessment Agency – History Database of the Global Environment
Retrieved on: 2024-01-02  
Retrieved from: https://doi.org/10.24416/UU01-AEZZIT  

#### Gapminder – Population
Retrieved on: 2023-03-31  
Retrieved from: http://gapm.io/dpop  

#### United Nations – World Population Prospects
Retrieved on: 2024-07-11  
Retrieved from: https://population.un.org/wpp/Download/  

#### Gapminder – Systema Globalis
Retrieved on: 2023-03-31  
Retrieved from: https://github.com/open-numbers/ddf--gapminder--systema_globalis  

#### Notes on our processing step for this indicator
The population data is constructed by combining data from multiple sources:

- 10,000 BCE - 1799: Historical estimates by HYDE (v3.3).

- 1800 - 1949: Historical estimates by Gapminder (v7).

- 1950-2023: Population records by the UN World Population Prospects (2024 revision).


## World regions according to OWID
Last updated: January 1, 2023  
Date range: 2023–2023  


### How to cite this data

#### In-line citation
If you have limited space (e.g. in data visualizations), you can use this abbreviated in-line citation:  
Our World in Data – processed by Our World in Data

#### Full citation
Our World in Data – processed by Our World in Data. “World regions according to OWID” [dataset]. Our World in Data, “Regions” [original data].
Source: Our World in Data

### What you should know about this data

### Source

#### Our World in Data – Regions


    