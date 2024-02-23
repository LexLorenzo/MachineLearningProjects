## Possible business questions to solve:

**This can also be used as a feature for the model**

- How should the deals be posted? (Website ba magfocus or dun sa mga catalogs. Note that medyo marami sa mga nagpurchase using catalog yung nagyes. Note also that marami dun sa mga nagvisit sa site yung nagyes)
- What type of products had the most spent? (Note that the amount spent might correlate to the prices of the products. Ex: wines are expensive compared to others.)
- What type of products are in the boom in the latest? (Note that the wines might have been the boom because consistent yung mga nagyes. )
- Should the promo focus on kids or teens?
- How much purchases has been made in their last purchase?
- Does the age of the customer correlate to their chances of agreeing to the offer?
- Does being a single parent correlate to their chances of availing the promo?
- Is the recency of their last purchase significant to their response?
- Are those who purchases with deals significant to their response? (Karamihan sa mga more than 6 nagyes)
- Are there any relevant information about parent income with the amount of kids they have?
- The relevance of Marital status, education, and income
- The relevance of Recency and number of people in the family (How much they consume the products)
- Significance on Recency on the number of days enrolled
- The Relevance of the Total number/Amount of purchases and Recency.
- The Relevance of the Total Amount of web purchases and Website visits.

  - Can conclude the interst of the customer based on the web

- The Relevance of the Total number of products purchaced based on the number of purchases
- The Loyalty of a customer = (Number of visits + Frequency of purchases) / (Number of days since enrollment)

  - The higher the loyalty the better chance of saying yes

- Number of Purchases and the amount of purchases based on customers loyalty
- The relevance of Recency and the number of complains

## Data Pre Processing:

- [x] Nulls in income (We can assume that they did not provide their income. Possible na iset nalang to 0 since konti lang yung mga di nagprovide. Pwede rin natin palitan ng mean of incomes para di masayang yung data. Possible na kuhain yung mean per Education)
- [x] Convert the bdate into age (Remove invalid ages)
  - [] All data was obtained from last year
  - [x] Check if the age is in the appropriate age to get any form of promo
- [x] Fixed the format for Dt_Customer
- [x] Removed the invalid dates where age is less than 18 to the time of enrolment (I assumed that 18 is the younges- allowed valid members)
- [] Vague yung marital status na mga nakalagay (possible na ifocus natin sya dun sa traditional marital status lang. Possible na convert yung absurd, alone, and YOLO into single)
- [] Remove outliers from income? Not sure
- [x] Remove age outliers
- [x] Nauna ang DT Customer kesa sa year birth
- [x] New column for the total family size

## Discuss the following in write up

- Assumptions in the data
- Definicitons of the contents of marital status and education

## Experiment on

- Effects of outliers in the models
- Difference of converting absurd, alone, and YOLO into single and just dropping them
- Difference of removing the nulls in income or replacing the null values with mean per education.
- Difference of removing outliers and not removing

## Bonus:

- Insights that may come for the business
- Comparison of models used
- Possible for profit loss from the complains based on the income and purchases

## Notes on models:

1. Decision Tree Model:
   Link: https://www.youtube.com/watch?v=RmajweUFKvM
   - madali sya magoverfit kaya kailangan mag generalization
   - kailangan maalis lahat ng outliers dahil malaki din effect nito sa capability ng model
   - wag masyado gawin complicated yung mga questions kasi mahihirapan na makaaccomodate ng new data afterwards pag masyadong complicated
   - #### Provide an entropy score on the dataset para majustify natin kung suitable ba yung model sa specific dataset natin
   - Important yung splitting para makakuha ng maayos na entropy
2. Logistic Regression:
   - Kailangan maresearch ng maigi kung anong threshold gagamitin para madetermine yung probability na yes or no
   - This performs best when linearly seperable yung data. (Kung ito yung pinakamataas yung score pwede natin to mamention)
   -

## Approach:

- Linear Regression to predict sales
- Bayes rule to combine different probabilities

## TODO

1. Create a structure na seperate yung data profiling, cleaning/preprocessing, and each models that will be used
2. Research on possible methods to use in quantifying the string columns

Goodnight sa mga viewers ko dyan! ;)

# Nigel's Results

#### K-nearest

- Cleaned_data.xlsx
  - Accuracy: 0.8420
    Precision: 0.4340
    Recall: 0.2323
    F1: 0.3026
    AUC: 0.5899
- Threshold_Data.xlsx
  - Accuracy: 0.8284
    Precision: 0.3519
    Recall: 0.1919
    F1: 0.2484
    AUC: 0.5653
