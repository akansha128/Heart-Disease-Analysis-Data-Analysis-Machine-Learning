# Heart-Disease-Analysis-Data-Analysis-Machine-Learning


# Initial Observations:
The dataset contains 1025 rows and 14 columns.

No missing values in any column.

The target column (0 = No heart disease, 1 = Presence of heart disease).

Most columns are integer types, except oldpeak, which is a float.

# Statistical Summary & Key Observations:

### Age:

Ranges from 29 to 77 years.

Median age: 56 years.

More older individuals in the dataset.


### Sex:

0 = Female, 1 = Male.

Mean ~0.70 suggests more males than females.



### Chest Pain Type (cp):

Categories: 0 (typical angina) to 3 (asymptomatic).

Median is 1, meaning most patients have mild to moderate chest pain.




### Resting Blood Pressure (trestbps):

Ranges from 94 to 200 mmHg.

Mean is 131 mmHg, which is slightly above normal.

### Cholesterol (chol):

Ranges from 126 to 564 mg/dL.

Mean 246 mg/dL, which is above normal (<200 mg/dL is ideal).

### Fasting Blood Sugar (fbs):

Binary: 0 (≤120 mg/dL) or 1 (>120 mg/dL).

Only 15% have high fasting blood sugar.

### Resting ECG (restecg):

Categorical: 0 (normal), 1 (ST-T wave abnormality), 2 (left ventricular hypertrophy).

Median is 1, indicating many patients have some ECG abnormality.

### Maximum Heart Rate Achieved (thalach):

Ranges from 71 to 202 bpm.

Higher values generally indicate better heart function.

### Exercise-Induced Angina (exang):

Binary: 0 (No) or 1 (Yes).

33% of patients experience angina during exercise.

### ST Depression (oldpeak):

Measures heart stress post-exercise.

Mean 1.07, some patients have high values (up to 6.2).

### Slope of Peak Exercise ST Segment (slope):

Ranges 0 to 2, with a mean of 1.38.

### Number of Major Vessels (ca):

Ranges from 0 to 4, with a median of 0.

Higher values may indicate heart issues.

### Thalassemia (thal):

Categories 0 to 3 (defects in blood oxygen transport).

Mean is 2.32, indicating moderate levels of abnormalities.

### Target (Heart Disease Presence):

Almost evenly split (mean = 0.51), suggesting balanced classes.

# Correlation Analysis (Heatmap Insights):

![Correlation Heatmap](https://github.com/akansha128/Heart-Disease-Analysis-Data-Analysis-Machine-Learning/blob/main/Correlation%20Analysis.png)


# Correlation Analysis (Heatmap Insights):
### Factors Strongly Related to Heart Disease (Target Column):

cp (Chest Pain Type) → 0.43: Higher chest pain types (especially atypical or non-anginal) correlate with heart disease.

thalach (Max Heart Rate) → -0.42: Higher heart rate is negatively correlated (i.e., healthier individuals achieve a higher max heart rate).

oldpeak (ST Depression) → 0.42: Higher ST depression is linked to heart disease.

slope → -0.34: Lower slope values correlate with disease presence.

ca (Major Vessels Count) → 0.46: More major vessels observed during fluoroscopy indicate a higher risk.

### Other Notable Relationships:

trestbps (Resting Blood Pressure) & age → 0.29: Older individuals tend to have higher blood pressure.

chol & age → 0.22: Cholesterol levels increase with age.

exang (Exercise-Induced Angina) & oldpeak → 0.58: Exercise-induced angina highly affects ST depression.
