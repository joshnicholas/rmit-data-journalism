# CO₂ emissions per capita - Data package

This data package contains the data that powers the chart ["CO₂ emissions per capita"](https://ourworldindata.org/grapher/co-emissions-per-capita?v=1&csvType=full&useColumnShortNames=false) on the Our World in Data website. It was downloaded on September 13, 2026.

### Active Filters

A filtered subset of the full data was downloaded. The following filters were applied:

## CSV structure

Each row is an observation for an entity (usually a country or region) at a timepoint.

- "Entity" — the name of the entity, e.g. "United States".
- "Code" — our internal entity code. For most countries this is the [ISO alpha-3](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-3) code, e.g. "USA"; historical and other non-standard entities get a custom code.
- "Year" or "Day" — the timepoint. Annual data has a "Year" column holding an integer year; otherwise a "Day" column holds a date string in the form "YYYY-MM-DD".
- The final column is the data column — the time series that powers the chart. Downloaded with the "full data" option it corresponds to the time series below; with "only selected data visible in the chart" it is transformed depending on the chart type, so the correspondence may be less direct.


## Metadata.json structure

The .metadata.json file contains metadata about the data package. The "charts" key contains information to recreate the chart, like the title, subtitle etc. The "columns" key contains information about each of the columns in the csv, like the unit, timespan covered, citation for the data etc.

## How we process data at Our World in Data

Our World in Data is almost never the original producer of the data - almost all of the data we use has been compiled by others. If you want to re-use data, it is your responsibility to ensure that you adhere to the sources' license and to credit them correctly. Please note that a single time series may have more than one source - e.g. when we stitch together data from different time periods by different producers or when we calculate per capita metrics using population data from a second source.

Preparing this data involves several processing steps. Depending on the data, this can include standardizing country names and world region definitions, converting units, calculating derived indicators such as per capita measures, as well as adding or adapting metadata such as the name or the description given to an indicator.
[Read about our data pipeline](https://docs.owid.io/projects/etl/).

## Detailed information about the data


### CO₂ emissions per capita
Carbon dioxide (CO₂) emissions from burning fossil fuels and industrial processes. This includes emissions from transport, electricity generation, and heating, but not land-use change.
Last updated: November 13, 2025  
Next expected update: November 2026  
Date range: 1750–2024  
Unit: tonnes per person  
Source: Global Carbon Budget (2025); Population based on various sources (2024) – with major processing by Our World in Data  

#### How to cite this data

Global Carbon Budget (2025); Population based on various sources (2024) – with major processing by Our World in Data

#### What you should know about this data
- Carbon dioxide (CO₂) is the primary greenhouse gas causing climate change.
- Global CO₂ emissions have stayed just below five tonnes per person for over a decade. But across countries, emissions vary widely, rising in some, falling in others.
- Fossil fuel burning is the main source of CO₂ emissions. This data includes fossil CO₂ emissions from activities such as transport, electricity generation, and heating.
- These figures don't include CO₂ emissions from changes in land use, like deforestation or reforestation.
- Emissions from international aviation and shipping are not included in the data for any individual country or region. They are only counted in the global total.
- This data is based on territorial emissions, meaning the emissions produced within a country's borders, but not those from imported goods. For example, emissions from imported steel are counted in the country where the steel is produced. To learn more and look at emissions adjusted for trade, read our article: [How do CO₂ emissions compare when we adjust for trade?](https://ourworldindata.org/consumption-based-co2)
- The data comes from the Global Carbon Budget. Fossil CO₂ emissions are estimated using national statistics on energy use — such as coal, oil, and gas consumption — and industrial production, particularly cement. These figures are converted into CO₂ emissions using standardized emission factors. For more details, read [the Global Carbon Budget paper](https://doi.org/10.5194/essd-15-5301-2023).
- CO₂ emissions per capita are calculated by dividing emissions by population. They represent the average emissions per person in a country or region. To learn more about how different metrics capture the distribution of CO₂ emissions, read our article: [Per capita, national, historical: how do countries compare on CO2 metrics?](https://ourworldindata.org/co2-emissions-metrics)

#### Notes on our processing step for this indicator
- Global emissions are converted from tonnes of carbon to tonnes of carbon dioxide (CO₂) using a factor of 3.664. This is the conversion factor [recommended by the Global Carbon Project](https://globalcarbonbudgetdata.org/downloads/jGJH0-data/Global+Carbon+Budget+v2024+Dataset+Descriptions.pdf). It reflects that one tonne of carbon, when fully oxidized, forms 3.664 tonnes of CO₂, based on the relative molecular weights of carbon and oxygen in CO₂.
- Emissions from the 1991 Kuwaiti oil fires are included in Kuwait's emissions for that year.- To calculate CO₂ emissions per capita, we divide the original data by a country's estimated population. These estimates come from our population dataset based on [multiple sources](https://ourworldindata.org/population-sources).


## Sources

These are the sources behind the data in this package. Each time series above names the ones it draws on in its citation.

### Global Carbon Project – Global Carbon Budget

The Global Carbon Budget was established by the Global Carbon Project (GCP) to track global carbon emissions and sinks.

This dataset makes it possible to assess whether countries are making progress toward the goals of the Paris Agreement and is widely recognized as the most comprehensive report of its kind.

Since 2001, the GCP has published estimates of global and national fossil CO₂ emissions. Initially, these were simple republished data from other sources, but over time, refinements were made based on feedback and correction of inaccuracies.

Producer: Global Carbon Project  
Published: 2025-11-13  
Retrieved on: 2025-11-13  
Retrieved from: https://globalcarbonbudget.org/  
License: CC BY 4.0 (https://doi.org/10.5281/zenodo.5569234)  

Citation: Andrew, R. M., & Peters, G. P. (2025). The Global Carbon Project's fossil CO2 emissions dataset (2025v15) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.17417124

The data files of the Global Carbon Budget can be found at: https://globalcarbonbudget.org/carbonbudget/

For more details, see the original paper:
Friedlingstein, P., O'Sullivan, M., Jones, M. W., Andrew, R. M., Bakker, D. C. E., Hauck, J., Landschützer, P., Le Quéré, C., Luijkx, I. T., Peters, G. P., Peters, W., Pongratz, J., Schwingshackl, C., Sitch, S., Canadell, J. G., Ciais, P., Jackson, R. B., Alin, S. R., Anthoni, P., Barbero, L., Bates, N. R., Becker, M., Bellouin, N., Decharme, B., Bopp, L., Brasika, I. B. M., Cadule, P., Chamberlain, M. A., Chandra, N., Chau, T.-T.-T., Chevallier, F., Chini, L. P., Cronin, M., Dou, X., Enyo, K., Evans, W., Falk, S., Feely, R. A., Feng, L., Ford, D. J., Gasser, T., Ghattas, J., Gkritzalis, T., Grassi, G., Gregor, L., Gruber, N., Gürses, Ö., Harris, I., Hefner, M., Heinke, J., Houghton, R. A., Hurtt, G. C., Iida, Y., Ilyina, T., Jacobson, A. R., Jain, A., Jarníková, T., Jersild, A., Jiang, F., Jin, Z., Joos, F., Kato, E., Keeling, R. F., Kennedy, D., Klein Goldewijk, K., Knauer, J., Korsbakken, J. I., Körtzinger, A., Lan, X., Lefèvre, N., Li, H., Liu, J., Liu, Z., Ma, L., Marland, G., Mayot, N., McGuire, P. C., McKinley, G. A., Meyer, G., Morgan, E. J., Munro, D. R., Nakaoka, S.-I., Niwa, Y., O'Brien, K. M., Olsen, A., Omar, A. M., Ono, T., Paulsen, M., Pierrot, D., Pocock, K., Poulter, B., Powis, C. M., Rehder, G., Resplandy, L., Robertson, E., Rödenbeck, C., Rosan, T. M., Schwinger, J., Séférian, R., Smallman, T. L., Smith, S. M., Sospedra-Alfonso, R., Sun, Q., Sutton, A. J., Sweeney, C., Takao, S., Tans, P. P., Tian, H., Tilbrook, B., Tsujino, H., Tubiello, F., van der Werf, G. R., van Ooijen, E., Wanninkhof, R., Watanabe, M., Wimart-Rousseau, C., Yang, D., Yang, X., Yuan, W., Yue, X., Zaehle, S., Zeng, J., and Zheng, B.: Global Carbon Budget 2023, Earth Syst. Sci. Data, 15, 5301-5369, https://doi.org/10.5194/essd-15-5301-2023, 2023.

### Various sources – Population

Our World in Data builds and maintains a long-run dataset on population by country, region, and for the world, based on various sources.

You can find more information on these sources and how our time series is constructed on this page: https://ourworldindata.org/population-sources

Producer: Various sources  
Published: 2024-07-15  
Retrieved on: 2026-03-31  
Retrieved from: https://ourworldindata.org/population-sources  
License: CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/)  

Citation: The long-run data on population is based on various sources, described on this page: https://ourworldindata.org/population-sources

    