# coodes - country-codes

## functions: 
### coodes provides **3** functions

##### 1.: findCountryFromAlpha2(code) {}
accepts alpha2-code (2 letters) as a string - **Capitalization** does **not** matter.

##### 2.: findCountryFromAlpha3(code) {}
accepts alpha3-code (3 letters) as a string - **Capitalization** does **not** matter as well.

##### 2.: findCountryFromUN(code) {}
accepts UN-code (3 numbers) as a **string** or as an **integer**


## example:
import {
    findCountryFromAlpha2, 
    findCountryFromAlpha3, 
    findCountryFromUN
} from 'coodes-country-codes'

const country = findCountryFromAlpha2("US")
// returns "United States of America"

const country2 = findCountryFromAlpha2("us")
// returns "United States of America

const country3 = findCountryFromAlpha3("USA")
// returns "United States of America"

const country4 = findCountryFromAlpha3("usa")
// returns "United States of America

const country4 = findCountryFromUN("840")
// returns "United States of America

const country4 = findCountryFromAlpha3(840)
// returns "United States of America


# Note: 
- every function returns a country by its english name if it exists in the international country codes
- if a country is **not** included in the internation country codes, then every function returns **undefined**