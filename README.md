# Brooklyn Housing
Investigated household selling prices across past 5 years in Brooklyn, and predicted pricing deltas using linear and logistic regression models to identify outlier instances

# Data Overview
House Sales data was available from 5 calendar years. Each of this was stored in system generated CSVs. All files were cleaned and made consistent before concatenating to build a central data repository.
Additional filters were employed to focus on single-family residences and single-unit apartments or condos for this analysis

# Modeling
Close to 25 different linear regression iterations were employed to check the best model fit, while trying to keep model dof below 40. 
Final model predicts square root of price using the following variables (More details in the analysis report):
- Brooklyn geographical subdivisions (Categorized e.g., Northern, Central, Eastern localities etc.)
- Building Class Category (Categorized)
- Land sqft (Continuous transformed)
- Gross sqft (Continuous transformed)
- Quarter of Sale (Categorized, Q1 2016 to Q4 2020)
- Neighborhood Affluence Level (Categorized e.g., Expensive neighborhoods etc.)

Model Performance: Adjusted R2 of 0.67; RMSE: 441420 USD

# Model Insights
Proving that were was a statistically significant increase in housing prices between Q3 2020 and Q4 2020. If a house sold in Q3 2020 was instead sold in Q4 2020, it could have achieved a delta of ~70,000$ just by the factor of sales date. (More details on the analysis report)  
