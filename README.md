# Observational-public-health-surveillance-study
 Investigation on amphetamines

HI looked into the initial FSV for AH4950 and confirmed that BDFS scores range from 101–754. Since Equifax discontinued BDFS, its white paper isn’t available online. During our 1-1, the score range you saw was most likely from the Commercial Insight Delinquency Score instead, which ranges from 397–695.

Given the model’s age, MRO is requesting the model calibration plan or the redevelopment schedule. Mike had briefly discussed a tentative redevelopment date with me before he retired, but there is no formal plan documented yet.

Mike had briefly discussed a tentative redevelopment date with me before he retired, but there is no formal plan documented yet. I’ll share the full details once the report is finalized, but I wanted to flag these items early so we stay aligned.

Thanks again, and congratulations on your new role.

Best regards,
Phoebe


# Introduction
Central nervous system stimulants, such as amphetamines, have seen widespreaduse over the past century, for legal and illegal purposes. A substantial portion of am-phetamine transactions are carried out in the "black market", hence it is important tostudy their spatial and temporal trends, both for public health and law enforcementpurposes. This repo investigated factors that affect the price (per mg) ofthe drug amphetamines based on a dataset taken from the website StreetRx.com. They gathers user-submitted information on street prices of diverted prescription or illicitdrugs.
## Data
The dataset for amphetamines consists of 76065 observations with 13 variables. I removed entries with NA values (58 rows), and splitted the date variable into year and month. The variables api_temp, form_temp and country has only one level for am-phetamines and hence are discarded. The variable city has about 8000 levels, which is not relevant/interesting without further geographicinformation linking them to states and regions, hence it is removed .For certain levels within the variables source, state and year, the number of entries aretoo small (<10) to be studied in a satisfactory manner, hence i also drop those levels. Since the distribution of ppm is extremely positively skewed, it is necessary to remove outliers that are three standard deviations away from the mean after normalization (this correspondsto a 99.7 percent interval) and performed a log-transformation on the value of ppm. The cleaned dataset consists of 75207 observations with 11 columns: both the origi-nal and log-transformed ppm(Price per mg), state, country, USA_region, source, mgstr,bulk_purchase, Primary_Reason, month and year.
