# nrs-household-estimates
Number and percentage of total dwellings in Edinburgh that are occupied, vacant, second homes, are occupied and exempt from paying Council Tax and that are receiving a Single Adult Council Tax discount. An 'occupied dwelling' is roughly equivalent to a household.

This dataset contains information on the number (‘count’) of dwellings in each Data Zone and the numbers and percentages (‘ratio’) that are occupied, vacant, second homes, are occupied and exempt from paying Council Tax and that are receiving a 'single adult' Council Tax discount. The estimates are based on Council Tax data collected in September each year. The estimated total number of dwellings in this dataset differ from those in the ‘Dwellings by Council Tax Band’, ‘Dwellings by Number of Rooms’ and ‘Dwellings by Type’ datasets as these are extracted from a different source (the Assessors’ Portal) at a different time of year (December, or January the following year).

Occupied dwellings are our proxy for a household. The dataset also includes estimates of total dwellings, vacant dwellings, second homes, occupied dwellings which are exempt from Council Tax, and dwellings subject to a Council Tax discount of 25 per cent.

Council Tax data contains information on the various discounts/exemptions awarded to each dwelling in Scotland, from these we can determine which dwellings are occupied and which are vacant or second homes. We remove the vacant dwellings and second homes from the total number of dwellings in each area, giving us the number of occupied dwellings. For full details of the methods used see the ‘Estimates of Households and Dwellings in Scotland’ publications on the National Records of Scotland (NRS) website.

Estimates are missing for Data Zones in some local authorities in some years. This should be taken into account if Data Zone level estimates are aggregated to produce estimates for higher geographies. Summary statistics for Council areas, National Parks, Strategic Development Plan areas, urban-rural classifications and Scottish Index of Multiple Deprivation deciles are published annually in 'Estimates of Households and Dwellings in Scotland' which is available from the NRS website.

Total Dwellings A ‘dwelling’ refers to the accommodation itself, for example a house or a flat, and includes second homes that are not let out commercially. Caravans count as dwellings if they are someone’s main house.

Which Are Occupied Any dwelling apart from those which are vacant or second homes. The number of occupied dwellings is a good estimate of the number of households.

Which Are Vacant This includes dwellings that are exempt from Council Tax and are unoccupied; and dwellings which are recorded on Council Tax systems as being long-term empty properties.

Which Are Second Homes These dwellings are subject to a Council Tax discount of between 10 per cent and 50 per cent due to being second homes. This includes self-catering holiday accommodation available to let for a total of less than 140 days per year. Second homes which are let out for 140 days or more are not included in these figures as they are classed as business so pay non-domestic rates rather than Council Tax. Each Council sets the level of discount for second homes.

With ‘Occupied Exemptions’ Dwellings exempt from Council Tax, which are occupied. This includes: dwellings only occupied by students, armed forces accommodation owned by the Secretary of State for Defence, dwellings which are the sole residence only of people aged under 18 or people who are classed as severely mentally impaired, trial flats used by registered housing associations, and prisons.

With Single Adult Discount Dwellings subject to a Council Tax discount of 25 per cent. This may include, for example, dwellings with a single adult, dwellings with one adult living with one or more children, or with one or more adults who are 'disregarded' for Council Tax purposes.

Statistics provided by National Records of Scotland :  http://statistics.gov.scot/data/household-estimates

## License

Data is licensed under the Open Government License: http://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/

## Requirements

- NodeJS
- npm

## Installation

Clone the repository

```
git clone https://github.com/EdinburghCityScope/nrs-household-estimates.git
```

Install npm dependencies

```
cd nrs-household-estimates
npm install
```

Run the API (from the nrs-household-estimates directory)

```
node .
```

Converting the extracted data into loopback data.

```
node scripts/featureCollectionToLoopbackJson.js
```

Re-build data files from the statistics.gov.scot API

```
node scripts/build-data.js
```
