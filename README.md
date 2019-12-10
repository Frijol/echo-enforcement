# ECHO Data Project

**Question: is anyone gaming the ECHO enforcement algorithm?**

* Enforcement algorithm: 10 continuous quarters of noncompliance (check this/cite)
* Research plan: Pull data of entities with violations, make a histogram of the number of contiguous months they are in violation. Is there any unusual shape around the algorithm limit for enforcement?

## What data is needed?
* 12-quarter violation history across facilities (can discard those with no violations)
* Recent enforcement (Y/N)
* Other information for further exploration?

## Finding the data
* EPA's ECHO (Enforcement and Compliance History Online) portal ([Data Downloads page](https://echo.epa.gov/tools/data-downloads))
* `echo_exporter_columns_07242019.xlsx` gives data element descriptions for the larger echo_data_exporter

### Columns of interest

#### Necessary to the project
* REGISTRY_ID
* FAC_QTRS_WITH_NC
* FAC_COMPLIANCE_STATUS
* **FAC_3YR_COMPLIANCE_HISTORY**

##### Bonus: clean air/water
* CAA_LAST_PENALTY_AMT
* CAA_QTRS_IN_NC
* CAA_COMPLIANCE_STATUS
* CAA_HPV_FLAG
* CAA_3YR_COMPL_QTRS_HISTORY

#### May be interesting for further analysis

##### Demography
* FAC_INDIAN_CNTRY_FLG
* FAC_PERCENT_MINORITY
* FAC_POP_DEN

##### Industry
* CAA_PERMIT_TYPES
* CAA_NAICS
* CAA_SICS

##### Mapping
* FAC_LAT
* FAC_LONG

##### Enforcement
* FAC_INSPECTION_COUNT
* FAC_DATE_LAST_INSPECTION
* FAC_INFORMAL_COUNT
* FAC_DATE_LAST_INFORMAL_ACTION
* FAC_FORMAL_ACTION_COUNT
* FAC_DATE_LAST_FORMAL_ACTION
* FAC_TOTAL_PENALTIES
* FAC_PENALTY_COUNT
* FAC_DATE_LAST_PENALTY
* FAC_LAST_PENALTY_AMT
* CAA_EVALUATION_COUNT
* CAA_DAYS_LAST_EVALUATION
* CAA_INFORMAL_COUNT
* CAA_FORMAL_ACTION_COUNT
* CAA_DATE_LAST_FORMAL_ACTION
* CAA_PENALTIES
* CAA_LAST_PENALTY_DATE
* CAA_LAST_PENALTY_AMT
* etc with CWA, RCRA, SDWA
* FEC_CASE_IDS
* FEC_NUMBER_OF_CASES
* FEC_LAST_CASE_DATE
* FEC_TOTAL_PENALTIES

##### How much is released
* TRI_IDS
* TRI_RELEASES_TRANSFERS
* TRI_ON_SITE_RELEASES
* TRI_OFF_SITE_TRANSFERS


