# google-advanced-data-analytics
 
For the capstone project of the Google Advanced Data Analytics professional certificate, you are tasked with helping a fictional automobile company with investigating their high employee turnover rate and to construct a model to help predict whether an employee will leave the company.

The data that is provided to you has already had some preprocessing and clearning done. For example, there were no missing values and some of the variables had already been normalized between 0 and 1, yet there were a couple spelling mistakes that required fixing.

The plan was to start with a basic logistic regression model and then ultimately compare the results between a random forest model and an XGBoost model. Including the initial logistic regression model was primarily to get additional experience in using scikit-learn models and to help get more familair with parameters, debugging, etc.

The EDA process already exposed a couple interesting observations such as the fact that employees that left tended to have more monthly average hours than employees that stayed. However, the HR and marketing departments were opposite. Additionally, among employees that left, those from accounting had disproportionately lower satisfaction levels compared to other departments.

Ultimately, the random forest model had a slightly better F1 and accuracy score. However, the XGBoost model was only marginally lower and actually had a higher recall score which would probably be preferred. The goal is to minimize employee turnover, so we would prefer to have false positives in the model rather than false negatives; i.e. we want to minimize predictions from the model that say an employee will stay when they actually will leave, and it is not the end of the world if the model predicts someone will leave but actually stay.
