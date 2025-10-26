## Econometric Analysis of Cash-Transfer Program

### [Link to Blog (includes R code, code output, and written analysis)](https://linusghanadan.github.io/blog/2024-3-6-post/)

### Context

This project was completed for my Policy Evaluation class, taken as part of my Master's program at UC Santa Barbara. Provided with data and questions, I carried out this analysis using appropriate causal inference modeling techniques.

### Central Question

How did the 1998 Prospera cash-transfer program impact the value of a household's animal holdings?

### Summary of Analysis

Compared pre-treatment characteristics in the treatment and control groups of the 1998 Prospera cash-transfer program. Estimated the Average Treatment Effect (ATE) of the program on a household’s value of owned animals with the First-Difference, Fixed-Effects, and Difference-in-Difference estimators.

### Notes on Data

Our data comes from a [2012 research paper published in the American Economic Journal](https://www.aeaweb.org/articles?id=10.1257/app.4.1.164) looking at the Progresa cash-transfer program, which was implemented in rural Mexican villages in 1998. Eligible households that were randomly selected to be part of the program were provided bi-monthly cash-transfers of up to 550 pesos per month. These cash-transfers were conditional on children attending school, family members obtaining preventive medical care, and attending health-related education talks. In total, over 17,000 households were part of the Progresa program.

**The outcome and treatment variables are:**

-   **vani** = value of animals owned by household (in 1997 USD)

-   **treatment** = dummy variable indicating whether an individual was part of the cash-transfer program (equal to 1 if the individual was part of the program)

**There are 55 control variables, including:**

-   **dirtfloor97** = dummy variable indicating whether a household had a dirt floor in 1997

-   **electricity97** = dummy variable indicating whether a household had electricity in 1997

-   **homeown97** = dummy variable indicating whether a household owned a house in 1997

-   **female_hh** = dummy variable indicating whether a household has a female head of household

-   **age_hh** = head of household age

-   **educ_hh** = head of household years of education
