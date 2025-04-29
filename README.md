# Project Background
In the highly competitive banking industry, customer retention is crucial to maintaining profitability and growth. With increasing customer expectations, rising competition from digital banks, and evolving financial needs, understanding why customers leave has become a strategic imperative.

This Bank Churn Analysis project was initiated to gain a deeper understanding of the factors contributing to customer attrition. By analyzing demographic trends, behavioral patterns, and financial metrics, the goal was to identify high-risk segments, uncover hidden insights, and inform strategic decision-making. Ultimately, the project aims to empower the bank to proactively address churn, enhance customer loyalty, and foster long-term relationships through targeted initiatives and customer-centric strategies.

**Key Insights and Recommendations focused on:**
1. **Customer Activity Level:** An analysis of customer engagement, segmented by active and inactive status, to understand how activity frequency correlates with customer retention and dropout behavior
2. **Geographical Churn Distribution:** Evaluation of churn rates across different countries - France, Germany and Spain - to identify regional churn patterns  and potential areas for localized intervention.
3. **Product Ownership Patterns:** Analysis of the number of banking products held by customers to understand how product portfolio size influences customer loyalty and retention potential.
4. **Financial Risk Indicators (Balance & Credit Score):** Evaluation of customer churn across various account balance tiers and credit score segments to understand the relationship between financial stability and attrition risk.

An interactive Power BI dashboard used to report and explore sales trends can be found [here](https://app.powerbi.com/links/KxNwjSGolO?ctid=16d83ee6-254a-469d-a6cc-54e2ca2313e7&pbi_source=linkShare)

## Data Structure & Initial Checks
The bank's main datastructure for this project involved a single CVS table with 10001 rows, containing the following fields.
customer_id
credit_score
country
gender
age
tenure
balance
product_number
credit_card
active_member
estimated_salary
churn

**Key Early Checks Included:**
- **Missing Values Assessment:** Verified the completeness of customer demigraphic fields, account balances and activity flags to ensure accurate segmentation in Power BI.
- **Duplicate Records Check:** Ensured that customers IDs were unique across tables to maintain integrity during joins and aggregations.
- **Data Type Validation:** Reviewed and corrected inconsistencies in data types for key fields such as balance, credit score, and product count. 


# Executive Summary
## Overview of Findings
1. **Inactive customers are substancially more likely to churn.** Customers who showed no recent activity accounted for a disproportionately high percentage of churn. Their disengagement emerged a sa clear red flag for potential departure, indicating that sustained interaction with bank products and services is vital for retention.
2. **Churn rates vary significantly by geography, with Germany posing the graetest concern.** Despite representing only a quarter of the customer base, Germany contributed nearly 40% of all churned accounts. This suggests that country-specific issues-possibly related to competition, customer experience, or local market expectations areaffecting retention.
3. **Single-product customers are the most vulnerable segment.** A large proportion of churned customers held only one product. By contrast, those with tow products demonstrated stronger loyalty, while customers with three or more products showed a slight rise in churn, potentially due to product complexity or lack of perceived value.

![Image](https://github.com/user-attachments/assets/d9fbf193-0f4b-4599-ae18-f44c9e126e0c)


## Insights Deep Dive

This section explores the key behavioral, demographic, and financial insights that contribute to customer churn. Each insight is supported by quantitative metrics and Power BI visualizations to identify actionable patterns across four critical business dimensions.

**Customer Activity Level**

- An analysis of activity flags shows that inactive customers have a churn rate of 63.92%, making inactivity the most significant early indicator of churn. This group represents just under half of the total customer base, but more than 60% of churned accounts.

- Evaluation of active customer data reveals that although active users comprise 51.5% of all customers, they represent only 36% of churned accounts, underscoring the protective effect of regular engagement.

- Inactive users tend to have lower balances, fewer products, and lower credit scores on average—suggesting a compounding effect of disengagement and low value.

- Churn likelihood increases sharply after 60 days of inactivity. Customers inactive for more than three months were almost twice as likely to churn compared to those recently active.

![Image](https://github.com/user-attachments/assets/74263988-c62f-40e6-8cbe-148c27a66b47)


**Geography-Based Churn**

- An evaluation of country-wise churn shows that Germany accounts for 39.96% of all churned customers, despite making up just 25% of the total customer base. This regional imbalance highlights the need for a location-specific churn mitigation strategy.

- France and Spain display healthier churn behavior, with churn rates 10.38% and 4.5% lower than their population share, respectively. Customers in these countries tend to have better engagement and a more balanced product mix.

- Germany has a higher proportion of inactive customers and single-product users, potentially contributing to its elevated churn rate.

- Customer satisfaction and Net Promoter Scores (NPS), where available, are lower in Germany—further supporting the hypothesis of localized service or experience gaps.




**Product Holding Behavior**

- An analysis of product ownership shows that customers with only one product have a churn rate of 69.17%, making them the most at-risk group. These customers often hold basic checking accounts or a single credit product.

- Customers with two products display the highest loyalty, with a churn rate of only 17.08%. They typically combine a checking account with a savings or credit product.

- Interestingly, customers with three or more products have slightly elevated churn compared to two-product users, possibly due to product complexity, misalignment with needs, or poor onboarding experience.

- Product mix matters: customers with a credit card and savings account are more likely to stay than those with a checking account and investment product only.



**Financial Risk Factors (Balance & Credit Score)**

- Evaluation of account balances reveals that customers in the 1k–10k range have nearly 100% churn, despite being a smaller segment. These accounts are often low-activity or fee-sensitive.

- Customers with a zero balance show moderate churn, indicating many of them may be new sign-ups, dormant users, or trial customers with low initial investment.

- The 100k–200k balance tier represents the most stable group, both in terms of loyalty and volume. These customers form the financial backbone of the bank’s portfolio and tend to hold multiple products.

- Credit score segmentation shows that churn is extremely high for scores ≤400, but stabilizes starting from the 401–500 range, and remains consistently low through the 601–700 band—where most customers fall.






