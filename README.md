## Background
I was interested in analyzing a marketing specific dataset to evaluate predictive models. The dataset is related to direct marketing campaigns (phone calls) of a Portuguese banking institution. The goal is to classify if an individual will subscribe to a term deposit. 

A predictive model will be helpful for understanding prospect conversion and/or building a foundation for a multi-touch attribution model. 

## Technique
The models chosen are well-known and documented, and are generally easily interpretable for non-technical stakeholders.

- Logistic Regression is a common approach for classification problems with binary outcomes or two classes. Results are easily interpretable, making it useful for relaying outcomes to non-technical stakeholders.
- Decision Trees are another highly interpretable option. They can be visualized to show the most important features and how decisions are made at each step. While they trade off some flexibility for simplicity, they offer more flexibility compared to logistic regression.
- Random Forest models offer more flexibility, but lose some interpretability. They can deliver higher accuracy because they address correlation issues that may occur in decision tree models.
- XGBoost is a popular model used for a variety of predictive problems, including classification. Since this dataset is small, XGBoost may not be the best fit, but it’s being included to provide a comparison against other models. Similar to straightforward decision trees, the ability to extract feature importance make the results more easily interpretable.
 

## Data Overview
The dataset was provided by UIC Machine Learning repository.
Moro, S., Rita, P., & Cortez, P. (2014). Bank Marketing [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5K306.

- Age: Age of existing client (integer)
- Job: Job type (categorical)
- Marital : Marital status (categorical)
- Education: Level of education (categorical)
- Default: Has credit in default? (boolean)
- Balance: Average yearly balance, in euros (integer) 
- Housing: Has a housing loan? (boolean)
- Loan: Has a personal loan? (binary: "yes","no")
- Contact: Last contact communication type (categorical)
- Day: Last contact day of the month (integer)
- Month: Last contact month of year (categorical)
- Duration: Last contact duration, in seconds (integer)
- Campaign: Number of contacts performed during this campaign and for this client (integer)
- Pdays: Number of days that passed  after the client was last contacted from a previous campaign (integer)
- Previous: Number of contacts performed before this campaign and for this client (integer)
- Poutcome: Outcome of the previous marketing campaign (categorical)
- y - Has the client subscribed a term deposit? (boolean)
