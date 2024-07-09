# DIABETES-PREDICTION

About Dataset
This dataset contains medical details of patients, including features such as glucose level, blood pressure, insulin level, BMI, age, and more. The target variable indicates whether a patient has diabetes. The goal of this dataset is to build and evaluate various machine learning or deep learning models to predict the onset of diabetes.

### The goal is to use these features to predict whether a patient has diabetes. 

### Below is a detailed description of each column in the dataset:

- Pregnancies: Number of times the patient has been pregnant.
- Glucose: Plasma glucose concentration a 2 hours in an oral glucose tolerance test.
- BloodPressure: Diastolic blood pressure (mm Hg).
- SkinThickness: Triceps skinfold thickness (mm).
- Insulin: 2-Hour serum insulin (mu U/ml).
- BMI: Body mass index (weight in kg/(height in m)^2).
- DiabetesPedigreeFunction: A function that scores likelihood of diabetes based on family history.
- Age: Age of the patient (years).
- Outcome: Class variable (0 or 1), where 1 represents the presence of diabetes and 0 represents the absence of diabetes.

### Usage
This dataset can be used for binary classification tasks to predict whether a patient has diabetes based on the given features.

I utilized logistic regression to classify individuals as having diabetes or not, achieving an accuracy of 75%.

https://github.com/sidiquegithub/DIABETES-PREDICTION/blob/main/CODE/Diabetes%20Classification.ipynb


## Logistic Regression
STATISTICAL THEORY 

The simple linear regression model is appropriate for relating a quantitative response
variable to a quantitative predictor x.

Now consider 𝑦 as a categorical variable that takes two values, depending on the numerical variable 𝑥. Let $y$ take the vaalues $1$ and $0$ corresponding to $Success$ and $Failure$, respectievely.

Define $p = P(Success) = P(1)$. Then the value of $p$  will depend on the value of some
quantitative variable $x$. 

In Logistic Regression we model some function of mean value of $y$ as a linear function of $\beta_0$ and $\beta_1$
- DEFENITION Logit Function

$$p(x) = \frac{ e^{\beta_0 + \beta_1 x}}{1 + e^{\beta_0 + \beta_1 x}}$$
 
Logistic regression means assuming that $p(x)$ is related to x by the logit function.


Straightforward algebra shows that

$$ \frac{p(x)}{1-p(x)} = e^{\beta_0 + \beta_1 x}$$


If we take $ln$ on both sides 

$$ ln\{\frac{p(x)}{1-p(x)}\} = \beta_0 + \beta_1 x$$
