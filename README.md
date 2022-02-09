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
> - Feature Engineering (binning, encoding)
> - Statistical summaries and visualisations
> - Features correlation

__3. Predictive Modeling__ 
 - Classification models: 
  > - Logistic Regression, 
  > - Support Vector Machine (SVM), 
  > - K-nearest Neaighbors (Knn), 
  > - Ensemble methods: Random Forest (RF), Extra Trees (ET) Boosting and Stacking

-----------------------------------------------------------------------------------------------------------------------
1.
### Objective
- Find the best Classification model and model hyperparameters for a such a dataset (e.g. in terms of performance, time)

- To detect early warning AE signals and assess possible safety concerns for a given vaccine, which may generate hypotheses and prompt further investigations.

### Description
- what is `VAERS`?
  - `Vaccine Adverse Event Reporting System` --- A passive surveillance system that monitors vaccine safety in the U.S. beyond       clinical trials.

- Who reports there? 
  - Anyone can report to VAERS, including patients, parents, and healthcare providers. Healthcare providers are also required       by law to do so. source: (https://vaers.hhs.gov/data/datasets.html)

- How we can make use of this data?
  - "VAERS reports alone cannot be used to determine if a vaccine caused or contributed to an adverse event or illness"(does       not infer causality) source: (https://wonder.cdc.gov/wonder/help/vaers.html)
  
------------------------------------------------

### 2.2. __Exploratory Data Analysis Framework:__ 

Levels of Analysis: Stats, Visualization

-----

#### Part 1. Basic analysis: 
 
- At a glance: categorical values || missing values; what is the best imputation method?

- Feautres Distribution

   - Post-covid19-vaccination Deaths by
   
    > - Vaccination doses counts in 2020 and 2021. 
    > - Vaccine manufacture and vaccine lots. 
    > - Recovery counts by each State. 

   
   - Gender, ageGroup, vaccine brand and vaccine lot distribution in 
   
    > - Hospitalization, Emergency visit, life threatening, disability, prolonged hospitalized days
    > - Myocarditis/Pericarditis, Guillain–Barré Syndrome, Thrombosis with Thrombocytopenia Syndrome (TTS) 
        (Rare but high risk health conditions attributed to the vax administration.)    


####  Part 2. Correlation signals: 

__Q. Does the population-health status play a significant role in having post-vaccine AE or getting recoverd?

   - status of the vaccine recipients:
     (ageGroup, gender, medical history, current illnes, current medication, allergy)
     
     __with__:

   > - __Recovery outcomes:__ (yes, no) after Vaccine administration
   > - __Serious outcomes:__ (yes, no) after Vaccine administration
        (Death, life threatening, disability, emergency visit, prolonged hospitalized days)

