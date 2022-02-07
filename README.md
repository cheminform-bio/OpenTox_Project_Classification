# VAERS
__1. Project Understanding__ 
- Objective
- Description

__2. Data Understanding__ 
> - Import Libraries
> - Load data

- 2.1. Data Cleaning (On how to get high-quality data?) 
> - Missing values (imputation, masking)
> - Dealing with (duplication records, errors, inconsistency, misspelling, outliers etc)
> - Categorical data: high and low cardinality

- 2.2. Exploratory Data Analysis
> - Feature Engineering (Binning, encoding)
> - Statistical summaries and visualisations
> - Features correlation
-----------------------------------------------------------------------------------------------------------------------
1.
### Objective
- Find Best Model and Model Metrics for such a dataset (e.g. in terms of performance)

- To detect signals of possible vaccine adverse events, which may generate hypotheses and prompt further investigations.

### Description
- what is `VAERS`?
  - `Vaccine Adverse Event Reporting System` --- A passive surveillance system that monitors vaccine safety in the U.S. beyond       clinical trials.

- Who reports there? 
  - Anyone can report to VAERS, including patients, parents, and healthcare providers. Healthcare providers are also required       by law to do so. source: (https://vaers.hhs.gov/data/datasets.html)

- How we can make use of this data?
  - "VAERS reports alone cannot be used to determine if a vaccine caused or contributed to an adverse event or illness"(does       not infer causality) source: (https://wonder.cdc.gov/wonder/help/vaers.html)
