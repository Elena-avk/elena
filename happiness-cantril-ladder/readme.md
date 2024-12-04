# Self-reported life satisfaction - Data package

This data package contains the data that powers the chart ["Self-reported life satisfaction"](https://ourworldindata.org/grapher/happiness-cantril-ladder?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website. It was downloaded on December 04, 2024.

## CSV Structure

The high level structure of the CSV file is that each row is an observation for an entity (usually a country or region) and a timepoint (usually a year).

The first two columns in the CSV file are "Entity" and "Code". "Entity" is the name of the entity (e.g. "United States"). "Code" is the OWID internal entity code that we use if the entity is a country or region. For normal countries, this is the same as the [iso alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code of the entity (e.g. "USA") - for non-standard countries like historical countries these are custom codes.

The third column is either "Year" or "Day". If the data is annual, this is "Year" and contains only the year as an integer. If the column is "Day", the column contains a date string in the form "YYYY-MM-DD".

The final column is the data column, which is the time series that powers the chart. If the CSV data is downloaded using the "full data" option, then the column corresponds to the time series below. If the CSV data is downloaded using the "only selected data visible in the chart" option then the data column is transformed depending on the chart type and thus the association with the time series might not be as straightforward.

## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc.. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc..

## About the data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stich together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

## Detailed information about the data


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


    