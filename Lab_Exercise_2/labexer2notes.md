## Possible business questions to solve:

- How should the deals be posted? (Website ba magfocus or dun sa mga catalogs. Note that medyo marami sa mga nagpurchase using catalog yung nagyes. Note also that marami dun sa mga nagvisit sa site yung nagyes)
- What type of products had the most spent? (Note that the amount spent might correlate to the prices of the products. Ex: wines are expensive compared to others.)
- What type of products are in the boom in the latest? (Note that the wines might have been the boom because consistent yung mga nagyes. )
- Should the promo focus on kids or teens?
- How much purchases has been made in their last purchase?
- Does the age of the customer correlate to their chances of agreeing to the offer?
- Does being a single parent correlate to their chances of availing the promo?
- Is the recency of their last purchase significant to their response?
- Are those who purchases with deals significant to their response? (Karamihan sa mga more than 6 nagyes)

## Possible data cleaning:

- Nulls in income (We can assume that they did not provide their income. Possible na iset nalang to 0 since konti lang yung mga di nagprovide)
- Convert the bdate into age (Remove invalid ages)
- Vague yung marital status na mga nakalagay (possible na ifocus natin sya dun sa traditional marital status lang)
- Remove outliers from income? Not sure
- Bigyan ng definition yung type of education (Especially 2n cycle and basic)
- May mga age na parang inapproriate (Ex: 131)

## Bonus:

- Insights that may come for the business
- Comparison of models used

## Notes on models:

1. Decision Tree Model:
    Link: https://www.youtube.com/watch?v=RmajweUFKvM
    * madali sya magoverfit kaya kailangan mag generalization
    * kailangan maalis lahat ng outliers dahil malaki din effect nito sa capability ng model
    * wag masyado gawin complicated yung mga questions kasi mahihirapan na makaaccomodate ng new data afterwards pag masyadong complicated
    * #### Provide an entropy score on the dataset para majustify natin kung suitable ba yung model sa specific dataset natin
    * Important yung splitting para makakuha ng maayos na entropy
    

Goodnight sa mga viewers ko dyan! ;)
