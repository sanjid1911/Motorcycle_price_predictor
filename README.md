# 🏍️ Bike Price Predictor

This project uses machine learning models to **predict the selling price of used bikes** based on features like age, seller type, ownership history, and more. It includes data preprocessing, feature engineering, model training (Linear Regression, Random Forest, Lasso Regression), and performance evaluation.

---

## 📁 Dataset

- **File**: `BIKE DETAILS.csv`
- **Location**: `F:\py\learn\Bike price predictor\`
- **Target Variable**: `selling_price`
- **Features**:
  - `year` (used to calculate age)
  - `km_driven`
  - `seller_type`
  - `owner`
  - Others excluding bike name

---

## 🧪 Workflow

1. **Import Libraries & Read Data**
2. **Drop Unnecessary Columns**
3. **Feature Engineering**:
   - Create `Age` from `year`
4. **Handle Missing Values**:
   - Use median for numeric columns
5. **Encode Categorical Variables**:
   - One-hot encoding on `seller_type` and `owner`
6. **Train-Test Split**
7. **Feature Scaling**:
   - StandardScaler applied to numeric columns
8. **Model Training**:
   - Linear Regression
   - Random Forest Regressor
   - Lasso Regression
9. **Evaluation**:
   - Mean Squared Error (MSE)
   - R² Score

---

## 📊 Model Performance

| Model               | MSE             | R² Score     |
|--------------------|-----------------|--------------|
| Linear Regression  | 751,730,840     | 0.7149       |
| Random Forest      | 686,227,425     | 0.7397       |
| Lasso Regression   | 751,726,615     | 0.7149       |

🔍 **Best performing model**: **Random Forest Regressor**

---

## 📦 Libraries Used

- `pandas`
- `numpy`
- `scikit-learn`

---

## 📌 Notes

- Random Forest performed best likely due to its ability to handle non-linear relationships.
- Feature scaling was applied even though Random Forest doesn't strictly require it (for consistency).
- Lasso regression was also used for potential feature selection.

---

