# Heart-Disease-Detection-Using-Multple-Machine-Learning-Models
# Heart Disease Detection Process

## 1. Data Collection
The dataset for heart disease detection typically contains medical information collected from patients. Each row represents a patient, and each column represents a specific feature or attribute related to their health.

## 2. Data Preprocessing
Before training the models, the data must be preprocessed. This includes handling missing values, encoding categorical variables, scaling numerical features, and splitting the data into training and testing sets.

## 3. Feature Selection
The dataset includes several important features related to heart health. In this case, the following features are selected for model training:

- **Age**: Age of the patient.
- **Sex**: Gender of the patient (1 = male; 0 = female).
- **ChestPainType**: Type of chest pain experienced (e.g., typical angina, atypical angina, non-anginal pain, asymptomatic).
- **RestingBP**: Resting blood pressure (in mm Hg).
- **Cholesterol**: Serum cholesterol level (in mg/dl).
- **FastingBS**: Fasting blood sugar > 120 mg/dl (1 = true; 0 = false).
- **RestingECG**: Resting electrocardiographic results (e.g., normal, ST-T wave abnormality, left ventricular hypertrophy).
- **MaxHR**: Maximum heart rate achieved.
- **ExerciseAngina**: Exercise-induced angina (1 = yes; 0 = no).
- **Oldpeak**: ST depression induced by exercise relative to rest.
- **ST_Slope**: The slope of the peak exercise ST segment (e.g., upsloping, flat, downsloping).

## 4. Model Training
Several machine learning models are trained to predict the presence of heart disease. In this example, the following models are used:

- Logistic Regression (y_predLR)
- Random Forest (Y_predRF)
- Decision Tree (y_predDT)
- XGBoost (y_predXGB)
- Multinomial Naive Bayes (y_predMNB)
- Gaussian Naive Bayes (y_predGNB)
- Gradient Boosting Classifier (y_predGBC)
- AdaBoost Classifier (y_predABC)
- Bernoulli Naive Bayes (y_predBNB)

## 5. Model Evaluation
The performance of each model is evaluated using accuracy scores, which measure the percentage of correct predictions made by the model on the test set. The accuracy scores for each model are as follows:

- **Logistic Regression (y_predLR)**: 0.8424
- **Random Forest (Y_predRF)**: 0.8424
- **Decision Tree (y_predDT)**: 0.8043
- **XGBoost (y_predXGB)**: 0.8696
- **Multinomial Naive Bayes (y_predMNB)**: 0.8152
- **Gaussian Naive Bayes (y_predGNB)**: 0.8424
- **Gradient Boosting Classifier (y_predGBC)**: 0.875
- **AdaBoost Classifier (y_predABC)**: 0.8533
- **Bernoulli Naive Bayes (y_predBNB)**: 0.7935

## 6. Best Model Selection
Among all the models, the Gradient Boosting Classifier (y_predGBC) achieves the highest accuracy score of 0.875, making it the best-performing model for this heart disease detection task.

## Columns in the Dataset
Here is a detailed description of the columns used in the dataset:

- **Age**: The age of the patient.
- **Sex**: The gender of the patient (1 = male, 0 = female).
- **ChestPainType**: The type of chest pain experienced:
  - 0: Typical angina
  - 1: Atypical angina
  - 2: Non-anginal pain
  - 3: Asymptomatic
- **RestingBP**: The resting blood pressure in mm Hg.
- **Cholesterol**: The serum cholesterol level in mg/dl.
- **FastingBS**: Fasting blood sugar level (1 if > 120 mg/dl, 0 otherwise).
- **RestingECG**: The resting electrocardiographic results:
  - 0: Normal
  - 1: ST-T wave abnormality
  - 2: Left ventricular hypertrophy
- **MaxHR**: The maximum heart rate achieved.
- **ExerciseAngina**: Exercise-induced angina (1 = yes, 0 = no).
- **Oldpeak**: ST depression induced by exercise relative to rest.
- **ST_Slope**: The slope of the peak exercise ST segment:
  - 0: Upsloping
  - 1: Flat
  - 2: Downsloping

By preprocessing this data, selecting the relevant features, and training various machine learning models, it is possible to predict the presence of heart disease in patients with a high degree of accuracy. The Gradient Boosting Classifier, in particular, has shown to be the most effective model in this example.
