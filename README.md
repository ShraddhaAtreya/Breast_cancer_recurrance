**Overview :** This project utilizes Machine Learning and Generative Adversarial Networks (GANs) to predict whether a patient diagnosed with breast cancer is likely to experience recurrence or non-recurrence of the disease. The model is trained using Random Forest Classification with hyperparameter tuning and data augmentation techniques.

**Dataset :** The dataset used in this project is sourced from the UCI Machine Learning Repository:

**Dataset Link:** https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer/breast-cancer.data

**Attributes:**

1. Class: Recurrent (1) or Non-Recurrent (0)
2. Age
3. Menopause
4. Tumor size
5. Invasive node
6. Node caps
7. Degree of malignancy
8. Breast side (left/right)
9. Breast quadrant
10. Irradiation history

**Features & Implementation**

Preprocessing: Missing values handled using mode imputation. Categorical encoding via One-Hot Encoding.

Data Balancing: Used SMOTETomek to handle class imbalance.

Model Training: Random Forest Classifier with Grid Search CV for hyperparameter tuning.

Data Augmentation: Used Generative Adversarial Networks (GANs) to generate synthetic training data.

Prediction Function: Takes patient details and predicts if the cancer is Recurrent or Non-Recurrent.
