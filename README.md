# coodes - country-codes

## new Update -> performance is now blazingly fast...
we recommend using the newest Version, though every other version still works 100% fine...

## functions: 
### coodes provides **6** functions

##### 1.: findCountryFromAlpha2(code)
accepts alpha2-code (2 letters) as a string - **Capitalization** does **not** matter

##### 2.: findCountryFromAlpha3(code)
accepts alpha3-code (3 letters) as a string - **Capitalization** does **not** matter as well

##### 3.: findCountryFromUN(code)
accepts UN-code (3 numbers) as a **string** or as an **integer**


#### For the following functions:
functions accepts strings of any form, don't worry about capitalization like "United States" or "united states", "United states", "united States", ...
##### 4.: findAlpha2FromCountry(country)

##### 5.: findAlpha3FromCountry(country)

##### 6.: findUNFromCountry(country) 


## example:
import { findCountryFromAlpha2 } from 'coodes-country-codes'

const country = findCountryFromAlpha2("US")
// country = "United States of America"


# Note: 
- every function returns a country by its english name if it exists in the international country codes
- if a country is **not** included in the international country codes, then every function returns **undefined**