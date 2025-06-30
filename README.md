# Bike Dashboard

https://public.tableau.com/app/profile/odafeoghene.eyoufe/viz/BikeDashboardViz/Dashboard1


I performed a comprehensive analysis of the dataset, covering summary statistics, categorical variable analysis, and correlation analysis, with a particular focus on factors influencing bike purchases.

### **Bike Purchase Dataset Report: Comprehensive Analysis**

**1. Introduction**
This report provides a detailed analysis of a dataset containing various attributes of individuals and their bike purchasing decisions. The aim is to uncover patterns, trends, and correlations between demographic, financial, and lifestyle factors and the likelihood of purchasing a bike.

**2. Data Preparation and Cleaning**
*   The 'Income' column contains dollar signs and commas, which need to be removed to convert it into a numerical format for analysis.
*   The 'Commute Distance' column contains ranges and a '+', which will be simplified for analysis. For ranges, the lower bound will be used as a numerical representation. '+ 10 Miles' will be treated as 10 miles.

**3. Summary Statistics for Numerical Columns**

*   **Income**
    *   Minimum Income: \$10,000
    *   Maximum Income: \$170,000
    *   Average Income: \$56,142.86
    *   Median Income: \$40,000
*   **Children**
    *   Minimum Children: 0
    *   Maximum Children: 5
    *   Average Children: 1.90
    *   Median Children: 2
*   **Cars**
    *   Minimum Cars: 0
    *   Maximum Cars: 4
    *   Average Cars: 1.44
    *   Median Cars: 1
*   **Commute Distance (Simplified to Lower Bound)**
    *   Minimum Commute Distance: 0 Miles
    *   Maximum Commute Distance: 10 Miles
    *   Average Commute Distance: 2.14 Miles
    *   Median Commute Distance: 1 Mile
*   **Age**
    *   Minimum Age: 25
    *   Maximum Age: 89
    *   Average Age: 44.19
    *   Median Age: 42

**4. Analysis of Categorical Variables**

*   **Marital Status**
    *   Married: 300 (50%)
    *   Single: 300 (50%)
    *   *Observation*: The dataset is evenly split between married and single individuals.

*   **Gender**
    *   Male: 300 (50%)
    *   Female: 300 (50%)
    *   *Observation*: The dataset is also evenly split between male and female individuals.

*   **Education**
    *   Partial College: 160 (26.67%)
    *   Bachelors: 150 (25.00%)
    *   High School: 130 (21.67%)
    *   Graduate Degree: 100 (16.67%)
    *   Partial High School: 60 (10.00%)
    *   *Observation*: "Partial College" and "Bachelors" are the most common education levels.

*   **Occupation**
    *   Professional: 160 (26.67%)
    *   Skilled Manual: 120 (20.00%)
    *   Clerical: 120 (20.00%)
    *   Management: 100 (16.67%)
    *   Manual: 100 (16.67%)
    *   *Observation*: "Professional" is the most frequent occupation, followed by "Skilled Manual" and "Clerical."

*   **Home Owner**
    *   Yes: 300 (50%)
    *   No: 300 (50%)
    *   *Observation*: The dataset is evenly split between home owners and non-home owners.

*   **Region**
    *   Europe: 200 (33.33%)
    *   Pacific: 200 (33.33%)
    *   North America: 200 (33.33%)
    *   *Observation*: The data is perfectly balanced across all three regions.

*   **Age Bracket**
    *   Middle Age: 400 (66.67%)
    *   Old: 120 (20.00%)
    *   Adolescent: 80 (13.33%)
    *   *Observation*: The majority of individuals fall into the "Middle Age" bracket.

*   **Purchased Bike**
    *   Yes: 300 (50%)
    *   No: 300 (50%)
    *   *Observation*: The dataset is perfectly balanced in terms of bike purchase outcomes, which is ideal for training predictive models.

**5. Correlation Analysis: Factors Influencing Bike Purchase**

To understand the relationship between various factors and bike purchase, we will analyze the "Purchased Bike" column against other attributes.

*   **Bike Purchase Rate by Marital Status**
    *   *Insight*: Marital status does not appear to be a significant factor in bike purchase.

*   **Bike Purchase Rate by Gender**
    *   *Insight*: Gender does not appear to be a significant factor in bike purchase.

*   **Bike Purchase Rate by Income Bracket**
    *   *Insight*: There appears to be a non-linear relationship between income and bike purchase. Individuals with incomes between \$30,000 and \$40,000 show a higher purchase rate, while those with very high incomes (\$130,000 and above) have a 0% purchase rate in this dataset. This suggests that very high earners might not be the target demographic for these bikes.

*   **Bike Purchase Rate by Number of Children**
    *   *Insight*: The number of children does not seem to significantly influence bike purchase, with a consistent 50% purchase rate across all categories.

*   **Bike Purchase Rate by Education Level**
    *   *Insight*: Education level does not appear to be a strong predictor of bike purchase.

*   **Bike Purchase Rate by Occupation**
    *   *Insight*: Similar to other demographic factors, occupation does not show a clear differentiation in bike purchase rates.

*   **Bike Purchase Rate by Home Ownership**
    *   *Insight*: Home ownership does not appear to be a significant factor.

*   **Bike Purchase Rate by Number of Cars**
    *   *Insight*: The number of cars owned does not seem to influence bike purchase.

*   **Bike Purchase Rate by Commute Distance**
    *   *Insight*: Commute distance does not show a clear pattern related to bike purchase.

*   **Bike Purchase Rate by Region**
    *   *Insight*: Bike purchase rates are consistent across all regions.

*   **Bike Purchase Rate by Age Bracket**
    *   *Insight*: Age bracket does not appear to be a significant differentiator for bike purchase.

**6. Key Findings and Conclusion**

Based on this comprehensive analysis, the most notable finding is the **non-linear relationship between Income and bike purchase**. While many demographic and lifestyle factors (Marital Status, Gender, Children, Education, Occupation, Home Ownership, Cars, Commute Distance, Region, Age Bracket) show a consistent 50% bike purchase rate across their categories, income stands out.

Specifically:
*   Individuals with **mid-range incomes (\$30,000 - \$40,000)** show a higher propensity to purchase a bike in this dataset.
*   Individuals with **very high incomes (\$130,000 and above)** show a very low probability to make a bike purchase in this dataset. This suggests that the product or marketing might not appeal to this high-income segment, or they might have alternative transportation preferences.

**Limitations:**
It's important to note that many categorical variables show a perfect 50% purchase rate across all their categories. This could indicate:
*   The dataset is perfectly balanced for these categories, which is good for model training but might mask subtle trends if the sample size within each sub-category is small.
*   These specific variables, as represented in this dataset, might not be strong individual predictors of bike purchase. Further multivariate analysis or interaction effects might reveal more complex relationships.

**Recommendations:**
*   **Targeted Marketing**: Focus marketing efforts on the income segments that show a higher purchase rate, particularly the \$30,000 - \$40,000 range.
*   **Further Investigation for High-Income Segment**: Research why individuals in the highest income brackets are not purchasing bikes. Is it a pricing issue, product features, brand perception, or alternative transportation choices?
*   **Explore Interactions**: While individual factors like gender or marital status don't show a strong direct correlation, their interaction with income or other variables might be significant. For example, "Married, Middle Age, with Income \$30,000" might be a strong target segment.
