# **<p align="center">Amazon Vine Analysis</p>**

### **<p align="center">A Pyspark analytics report designed to determine if paid reviewers in the Amazon Vine Program are more or less likely to provide a positive review.</p>**

---
## Overview
This report will determine if there is a bias from Paid reviewers of Jelwery products from Amazon. Data was extracted from a dataset on Jewelry reviews provided by AWS. The data was then transformed so that the following four tables were created that matched our schema: review_id, products, customers, vine. Next, we loaded the data into our Amazon RDS via pgAdmin. We then filtered out all reviews with less than 20 votes and kept from that set only the reviews that were more than 50% helpful. Finally, we obtained the total number of reviews, number of five star reviews and percentage of five star reviews for both the Paid and Unpaid reviewers. The results section below shows our findings.

---
## **<p align="center">Results</p>**
---

<p align="center">
   <img width="750" height="250" src="https://github.com/Jamesrx33/Amazon_Vine_Analysis/blob/main/Resources/Results%20Table.png?raw=true">
</p>

1. **Totals Difference:** There were 21 paid vine reviews and 7,689 non-paid reviews.
2. **Five Stars Difference:** Of the Paid Vine reviews, 11 of these reviews were five stars. Of the 7689 non-paid reviews 4,444 were five stars.
3. **Percentage Five Stars:** 52.0% of the Paid Vine reviews were five stars and 57.8% if the non-paid reviews were five stars.

---
## Summary
---
In conclusion, based on these results we would determine that there is not a positivity bias from reviewers in the Paid Vine program. Only 52% of the Vine reviews were five stars, where as 57.8% of the non-vine reviews were five stars. Given the large difference in total number of helpful reviews from non-vine viewers and the fact that a larger percentage were five stars, it would be safer to say it is possible that there is a negative bias from Vine reviews.

**Further Analysis:** I would recommend extending the criteria to 4 or 5 star reviews to get a better sense of the data as a whole. Should this also return a lower percentage of positive Vine reviews, we would confirm our suspicions.

---

## Reference Documentation - [Source Code Repository](https://github.com/Jamesrx33/Amazon_Vine_Analysis), [Download .zip file](https://github.com/Jamesrx33/Amazon_Vine_Analysis/archive/refs/heads/main.zip)
