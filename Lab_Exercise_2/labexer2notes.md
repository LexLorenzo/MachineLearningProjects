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
- Are there any relevant information about parent income with the amount of kids they have?
- The relevance of Marital status, education, and income
- The relevance of Recency and number of people in the family (How much they consume the products)
- Significance on Recency on the number of days
- The Relevance of the Total number of purchases and Recency.
- The Relevance of the Total number of purchases and Website visits.
- The Relevance of the Total number of products purchaced based on the number of purchases
- The number of web purchases on the web visits
- The Loyalty of a customer = (Number of visits + Frequency of purchases) / (Number of dates since enrollment)
  - The higher the loyalty the better chance of saying yes
- 

## Data Pre Processing:

- Nulls in income (We can assume that they did not provide their income. Possible na iset nalang to 0 since konti lang yung mga di nagprovide)
- Convert the bdate into age (Remove invalid ages)
  - All data was obtained from last year
  - Check if the age is in the appropriate age to get any form of promo
- Vague yung marital status na mga nakalagay (possible na ifocus natin sya dun sa traditional marital status lang)
- Remove outliers from income? Not sure
- Bigyan ng definition yung type of education (Especially 2n cycle and basic)
- May mga age na parang inapproriate (Ex: 131)
- Nauna ang DT Customer kesa sa year birth
- New column for the total number of children
- The relevance of Recency and the number of complains

## Bonus:

- Insights that may come for the business
- Comparison of models used
- Possible for profit loss from the complains based on the income and purchases

Goodnight sa mga viewers ko dyan! ;)

## Approach:

- Linear Regression to predict sales
- Bayes rule to combine different probabilities
