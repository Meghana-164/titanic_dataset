# Titanic Dataset Preprocessing

## Objective

The goal of this task is to preprocess the Titanic dataset to prepare it for further analysis or model building. This includes handling missing values, standardizing numerical features, detecting and removing outliers, and exploring class distribution for the target variable (`Survived`).

---

## Preprocessing Steps

### 1. Loading the Dataset

- Loaded using **pandas**
- Checked for missing values and data types

---

### 2. Feature Selection

Initial features considered:
- `PassengerId`
- `Survived`
- `Pclass`
- `Sex`
- `Age`
- `SibSp`
- `Parch`
- `Ticket`
- `Fare`
- One-hot encoded `Embarked`

---

### 3. Standardization

Applied **standardization** to numerical features:
- `Age`
- `Fare`

Tool used:
- `StandardScaler` from `sklearn.preprocessing`

---

### 4. Outlier Detection & Removal

- **Box plots** were used to visualize potential outliers
- **IQR (Interquartile Range)** method used for detecting and removing outliers

**Final dataset shape** after outlier removal:
- From **(891, 12)** → **(561, 12)**

---




## Next Steps

With the cleaned and preprocessed dataset, we can now proceed with feature engineering and building predictive models.
