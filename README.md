# Employee-turnover-prediction-using-ML-approaches
"Employee turnover prediction Using Machine Learning approaches and performance analysis of ML algorithms", is a research project that I have completed as part of my Mastar's requirement. The goal is to help HR departments make data-driven decision to reduce employee attrition.

In this research, a machine-learning framework was developed for employee turnover prediction. comparing nine machine learning algorithms (Random Forest, Decision Tree, XGBoost, Gradient Boosting, Support Vector Machine, Logistic Regression, CatBoost, Gaussian Naïve Bayes and K-Nearest Neighbour) on structured HR data.

Two data sources were used, a primary dataset collected through surveys from 24 employees and secondary dataset from Kaggle (https://www.kaggle.com/datasets/ziya07/employee-attrition-prediction-dataset) comprising over 10,000 records. Key variables included job satisfaction, monthly income, tenure and work-life balance. Categorical variables were one-hot encoded, numerical features standardized and class imbalance addressed with SMOTE resampling.

.

### Exploratory Data Analysis (EDA)
EDA was conducted to identify trends and relationship between features. The analysis revealed higher turnover among early career employees (within first 2 years of employment) where 'Low compensation and lack of career growth' were major factors. Employees with 'poor work-life balance' were likely to leave.
<p align="center">
  <img src="images/s_turnover.png" width="400" height="300"><br>
</p>

The dataset shows a class imbalance, where the majority of the employees stay while a smaller portion leave. To address this issue SMOTE (Synthetic Minority Oversampling Technique) has been used. The following graphs shows a partial exploratory data analysis.

<p align="center">
  <img src="images/s_turnoverbyDepartment.png" width="350" height="300"/>
  <img src="images/s_turnoverbyJobRole.png" width="350" height="300"/><br>
  <img src="images/s_turnoverbyAge.png" width="350" height="300"/>
  <img src="images/s_turnoverbyworkingYears.png" width="350" height="300"/><br>
  <img src="images/s_turnoverbyWorklifebalance.png" width="350" height="300"/>
  <img src="images/s_turnoverbyPerformance.png" width="350" height="300"/>
</p>

<p align="center">
  <em> &nbsp;&nbsp;&nbsp;  &nbsp;&nbsp;&nbsp; </em>
</p>



### Machine Learning algorithm anlysis

Nine machine learning algorithms (Random Forest, Decision Tree, XGBoost, Gradient Boosting, Support Vector Machine, Logistic Regression, CatBoost, Gaussian Naïve Bayes and K-Nearest Neighbour) were implemented and compared. Several preprocessing steps were applied before modeling training such as irrelevent features removal, checked for missing values and so on. Categorical variables were encoded usimg "One-Hot Encoding".

Models were evaluated using multiple (Accuracy, Precision, Recall, F1 Score, ROC-AUC) matrics. Hyperparameter tuning was conducted to achieve effective machine learning performance. The following tables shows the evaluted result for each machine learning algorithms.

<p align="center">
<em>Comparision of classifiers (train with secondary data) in different matrices (after Tuning)</em>
</p>

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

<p align="center">
<em>Comparision of classifiers (train with primary data) in different matrices (after Tuning)</em>
</p>

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

