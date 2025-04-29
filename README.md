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



