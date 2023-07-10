# Cardiovascular Disease Analysis using R

### 2/07/2023

Exploring risk factors for cardiovascular diseases in adults

This dataset contains detailed information on the risk factors for cardiovascular disease. It includes information on age, gender, height, weight, blood pressure values, cholesterol levels, glucose levels, smoking habits and alcohol consumption of over 70 thousand individuals. Additionally it outlines if the person is active or not and if he or she has any cardiovascular diseases.

Source: https://www.kaggle.com/datasets/thedevastator/exploring-risk-factors-for-cardiovascular-diseas

In the dataset are:

- Numeric values for age, height, weight, systolic blood pressure (ap_hi) and diastolic blood pressure (ap_lo).
- Binary values for gender, alcohol consumption (alco), smoking habits (smoke), active person (active), cardiovascular diseases (cardio). In the gender variable it's not defined which value correspond to which gender. In the rest of the cases 0 = No and 1 = Yes. 
- Levels in the cholesterol and glucose (gluc) variables. In this cases I will consider that  1 = normal, 2 = above normal, 3 = well above normal. 


The aim of this analysis it's finding correlation between variables and determining which ones contributes to develop cardiovascular diseases.
Also build a predictive model using some variables.




# Some plots of the analysis


![Lifestyle plot](https://user-images.githubusercontent.com/126076818/220638184-9a693f3e-07c0-4d4e-a05b-32952876de12.png)

![Chol and gluc plot](https://user-images.githubusercontent.com/126076818/220639856-9498e8e2-a0be-4de6-9fbc-19b038634c29.png)

![Age tendency plot](https://user-images.githubusercontent.com/126076818/220639772-756bc195-3b88-4e8e-b193-faf46cc239f5.png)

![Logistic regression model](https://user-images.githubusercontent.com/126076818/220639897-09b169a0-9d53-44b3-800a-92e22cc9b924.png)


# Conclusions:

From these dataset it can be concluded the next things for adults between 39 and 65 years old:

- Lifestyle: being an active person reduces the probabilities of having cardiovascular diseases.

- Gender: there isn't difference between genders and risk of having cardiovascular diseases.

- Cholesterol and glucose levels: higher cholesterol and glucose levels are highly correlated with cardiovascular diseases.

- Age: Age and proportion of people with cardiovascular disease are highly correlated. In older people (from 60 to 65 years old) the risk is much higher than in the less-older ones (from 39 to 45 years old).

- BMI: positive correlation between BMI and proportion of people with cardiovascular disease. Obesity class 2 group is the most risky one.

- MAP: poositive correlation between MAP and proportion of people with cardiovascular disease. Hypertension stage 2 group is the most risky one.

- Predictive model: a logistic regression model with the age, BMI and MAP variables was made. This model has a 70% of accuracy when predicting the probability of having cardiovascular diseases.
