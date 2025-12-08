# Observational-public-health-surveillance-study
 Investigation on amphetamines

 Here is a polished, polite email you can send to his senior manager. Tone is respectful, concise, and appropriate for someone senior:

---

Subject: Request for Updated Point of Contact for [Project Name]

Hi [Her Name],
Hope you are doing well.

I learned last week that [Retired Manager’s Name] has retired. Since I had been coordinating with him on the ongoing [project name] work, I wanted to check in with you regarding the updated point of contact for this project. At the moment, I have not received a transition note or a replacement contact, so I wanted to make sure I reach out to the right person as the work continues.

Whenever convenient, could you please let me know who I should coordinate with going forward?

Thank you very much for your time and guidance.

Best regards,
Phoebe

---

If you want it to sound more formal, more concise, or include a brief project description, I can adjust it.


# Introduction
Central nervous system stimulants, such as amphetamines, have seen widespreaduse over the past century, for legal and illegal purposes. A substantial portion of am-phetamine transactions are carried out in the "black market", hence it is important tostudy their spatial and temporal trends, both for public health and law enforcementpurposes. This repo investigated factors that affect the price (per mg) ofthe drug amphetamines based on a dataset taken from the website StreetRx.com. They gathers user-submitted information on street prices of diverted prescription or illicitdrugs.
## Data
The dataset for amphetamines consists of 76065 observations with 13 variables. I removed entries with NA values (58 rows), and splitted the date variable into year and month. The variables api_temp, form_temp and country has only one level for am-phetamines and hence are discarded. The variable city has about 8000 levels, which is not relevant/interesting without further geographicinformation linking them to states and regions, hence it is removed .For certain levels within the variables source, state and year, the number of entries aretoo small (<10) to be studied in a satisfactory manner, hence i also drop those levels. Since the distribution of ppm is extremely positively skewed, it is necessary to remove outliers that are three standard deviations away from the mean after normalization (this correspondsto a 99.7 percent interval) and performed a log-transformation on the value of ppm. The cleaned dataset consists of 75207 observations with 11 columns: both the origi-nal and log-transformed ppm(Price per mg), state, country, USA_region, source, mgstr,bulk_purchase, Primary_Reason, month and year.
