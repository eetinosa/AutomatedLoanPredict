# AutomatedLoanPredictor
This repository contains file to automate the loan eligibility process based on customer details provided while filling online application form

##Description

The task is to predict whether the loan will be approved or not based on the details provided by customers. Here is the problem statement for this project:
Based on the details provided by customers, we have to create a model that can decide where or not their loan should be approved. 

Here are a couple of factors that are helpful with respect to this project:

- Amount of loan: The total amount of loan applied by the customer. 
- Income of applicanhttps://github.com/eetinosa/AutomatedLoanPredict/blob/main/data.csvhttps://github.com/eetinosa/AutomatedLoanPredict/blob/main/data.csvt: The income of the applicant (customer) can also be a deciding factor. A higher income will lead to higher probability of loan approval.
- Education of applicant: Educational qualification of the applicant can also be a vital factor to predict the loan status of a customer. 



## Data exploration and pre-processing phase.
To explore the dataset and pre-process it. Find the dataset [here](https://github.com/eetinosa/AutomatedLoanPredict/blob/main/data.csv)The steps taken are as follows:

- Univariate Analysis
- Bivariate Analysis
- Missing Value Treatment
- Outlier Treatment
- Feature Engineering

Explore the variables individually which is called the univariate analysis. Exploring the effect of one variable on the other, or exploring two variables at a time is the bivariate analysis. Look for any missing values or outliers that might be present in the dataset and deal with them. And also create new features using the existing features (Encoding) which is referred to as feature engineering. 

##Model building 
It is a classification problem, Any of the classification models like the logistic regression, decision tree, random forest,can be used etc. Here, I used a random forest as the predictive model for this project.

Random forest classifier creates a set of decision trees from randomly selected subset of training set. It then aggregates the votes from different decision trees to decide the final class of the test object.

Tuning Parametersused for this model

- n_estimators : Number of trees in forest. Default is 10.
- max_depth : represents the depth of each tree in the forest. Here I used 5
- random_state : this is used as a seed to ensure consistency. 
- min_samples_split: minimum number of working set size at node required to split. Default is 2.

![The Loan PRedictor Webpage](https://github.com/eetinosa/AutomatedLoanPredict/blob/main/Loan%20Predictor.PNG)
##How to run the model
On a terminal, run

```bash
git clone https://github.com/eetinosa/AutomatedLoanPredict
cd AutomatedLoanPredict/
code .
source loan/bin/activate
pip install -r requirements.txt
streamlit run app.py
```
