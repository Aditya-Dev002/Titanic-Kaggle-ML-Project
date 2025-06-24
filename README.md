# Titanic Survival Prediction 🚢

This project is a solution to the [Titanic - Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic/overview) challenge on Kaggle. The goal is to predict whether a passenger survived or not, using basic machine learning techniques.

---

## 📁 Dataset

- **train.csv** – Data with passenger features and survival labels.
- **test.csv** – Similar data without survival labels, used for final prediction.
- **gender_submission.csv** – A sample submission file provided by Kaggle.

---

## 🧹 Data Preprocessing

- Handled missing values:
  - `Age` and `Fare` filled with median values.
  - `Embarked` filled with the most frequent category.
  - `Cabin` column dropped (due to many missing values).
- Converted categorical variables (`Sex`, `Embarked`) using `OrdinalEncoder`.

---

## 🧠 Model Used

- **Logistic Regression** from `scikit-learn`
  - Increased `max_iter` to 200 to avoid convergence warnings.
  - Trained on selected numerical and encoded features.

---

## 📊 Evaluation

- Basic accuracy was calculated on the training split.
- Final accuracy on Kaggle submission: **0.8101**

---
## ⚙️ Configuration

All project settings, preprocessing steps, and model metadata are described in 'titanic_project.yml'.


## ✅ Submission Format

Output was saved in `submission.csv`:
