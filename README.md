# Employee-turnover-prediction-using-ML-approaches
"Employee turnover prediction Using Machine Learning approaches and performance analysis of ML algorithms", is a research project that I have completed as part of my Mastar's requirement. The goal is to help HR departments make data-driven decision to reduce employee attrition.

In this research, a machine-learning framework was developed for employee turnover prediction. comparing nine machine learning algorithms (Random Forest, Decision Tree, XGBoost, Gradient Boosting, Support Vector Machine, Logistic Regression, CatBoost, Gaussian Naïve Bayes and K-Nearest Neighbour) on structured HR data.

Two data sources were used, a primary dataset collected through surveys from 24 employees and secondary dataset from Kaggle (https://www.kaggle.com/datasets/ziya07/employee-attrition-prediction-dataset) dataset comprising over 10,000 records. Key variables included job satisfaction, monthly income, tenure and work-life balance. Categorical variables were one-hot encoded, numerical features standardized and class imbalance addressed with SMOTE resampling.

.

### Exploratory Data Analysis (EDA)
EDA was conducted to identify trends and relationship between features. Here are the some EDA graphs based on the research.
<p align="center">
  <img src="employee turniver rate" width="300" height="300">
</p>

It indicates class impbalance which later solved by SMOTE resampling.

<table>
<tr>
<td align="center">
<img src="https://github.com/habib-777/AgriFarm/blob/main/Screenshots/AgriFarm.png" width="250" height="250"><br>
(a) Input
</td>

<td align="center">
<img src="https://github.com/habib-777/AgriFarm/blob/main/Screenshots/AgriFarm.png" width="250" height="250"><br>
(b) Prediction
</td>

<td align="center">
<img src="https://github.com/habib-777/AgriFarm/blob/main/Screenshots/AgriFarm.png" width="250" height="250"><br>
(c) Ground Truth
</td>
</tr>
</table>

<p align="center">
  <img src="https://github.com/habib-777/AgriFarm/blob/main/Screenshots/AgriFarm.png" width="250" height="250"/>
  <img src="https://github.com/habib-777/AgriFarm/blob/main/Screenshots/AgriFarm.png" width="250" height="250"/>
  <img src="https://github.com/habib-777/AgriFarm/blob/main/Screenshots/AgriFarm.png" width="250" height="250"/>
</p>

<p align="center">
  <em>(a) Input &nbsp;&nbsp;&nbsp; (b) Prediction &nbsp;&nbsp;&nbsp; (c) Ground Truth</em>
</p>

.

### Machine Learning algorithm anlysis

Comparision of classifiers (train with secondary data) in different matrices (after Tuning)

<table align="center">
<tr align="center">
  <td> </td>
  <td> Train accuracy </td>
  <td> Test accuracy </td>
  <td> Precision </td>
  <td> Re-call </td>
  <td> F!-score </td>
  <td> ROC-AUC </td>
</tr>
<tr align="center">
  <td> CatBoost </td>
  <td> 1.00 </td>
  <td> 0.88 </td>
  <td> 0.97 </td>
  <td> 0.79 </td>
  <td> 0.87 </td>
  <td> 0.93 </td>
</tr>
<tr align="center">
  <td> Random Forest </td>
  <td> 1.00 </td>
  <td> 0.87 </td>
  <td> 1.00 </td>
  <td> 0.74 </td>
  <td> 0.85 </td>
  <td> 0.93 </td>
</tr>
<tr align="center">
  <td> Gradient Boosting </td>
  <td> 0.88 </td>
  <td> 0.87 </td>
  <td> 1.00 </td>
  <td> 0.74 </td>
  <td> 0.85 </td>
  <td> 0.89 </td>
</tr>
<tr align="center">
  <td> XgBoosting </td>
  <td> 0.88 </td>
  <td> 0.87 </td>
  <td> 1.00 </td>
  <td> 0.73 </td>
  <td> 0.85 </td>
  <td> 0.88 </td>
</tr>
<tr align="center">
  <td> SVM </td>
  <td> 1.00 </td>
  <td> 0.86 </td>
  <td> 1.00 </td>
  <td> 0.72 </td>
  <td> 0.84 </td>
  <td> 0.99 </td>
</tr>
<tr align="center">
  <td> Decision Tree </td>
  <td> 0.90 </td>
  <td> 0.79 </td>
  <td> 0.81 </td>
  <td> 0.76 </td>
  <td> 0.78 </td>
  <td> 0.85 </td>
</tr>
<tr align="center">
  <td> Logistic Regression </td>
  <td> 0.54 </td>
  <td> 0.55 </td>
  <td> 0.55 </td>
  <td> 0.56 </td>
  <td> 0.56 </td>
  <td> 0.56 </td>
</tr>
</table>

Comparision of classifiers (train with primary data) in different matrices (after Tuning)

<table align="center">
<tr align="center">
  <td> </td>
  <td> Train accuracy </td>
  <td> Test accuracy </td>
  <td> Precision </td>
  <td> Re-call </td>
  <td> F!-score </td>
  <td> ROC-AUC </td>
</tr>
<tr align="center">
  <td> Gaussian Naïve Bayes  </td>
  <td> 1.00 </td>
  <td> 0.83 </td>
  <td> 1.00 </td>
  <td> 0.50 </td>
  <td> 0.67 </td>
  <td> 0.69 </td>
</tr>
<tr align="center">
  <td> KNN </td>  
  <td> 1.00 </td>
  <td> 0.83 </td>
  <td> 1.00 </td>
  <td> 0.50 </td>
  <td> 0.67 </td>
  <td> 0.75 </td>
</tr>
<tr align="center">
  <td> Random Forest </td>
  <td> 1.00 </td>
  <td> 1.00 </td>
  <td> 1.00 </td>
  <td> 1.00 </td>
  <td> 1.00 </td>
  <td> 1.00 </td>
</tr>
<tr align="center">
  <td> Decision Tree </td>
  <td> 1.00 </td>
  <td> 1.00 </td>
  <td> 1.00 </td>
  <td> 1.00 </td>
  <td> 1.00 </td>
  <td> 1.00 </td>
</tr>  
</table>


<p align="center">
  <img src="https://github.com/habib-777/AgriFarm/blob/main/Screenshots/AgriFarm.png" width="600"/>
  <br>
  <em>Figure 1: System architecture</em>
</p>

now 

<figure>
  <img src="https://github.com/habib-777/AgriFarm/blob/main/Screenshots/AgriFarm.png" width="600">
  <figcaption>Figure 1: Model architecture</figcaption>
  <img src="https://github.com/habib-777/AgriFarm/blob/main/Screenshots/AgriFarm.png" width="600">
  <figcaption>Figure 2: Model architecture</figcaption>
</figure>

<p align="center">
    <img width="800" src="https://github.com/habib-777/AgriFarm/blob/main/Screenshots/AgriFarm.png" alt="Home page">
</p>

