# Housing Price Prediction with Random Forest

This project demonstrates how to **predict house prices** using a **Random Forest** model, leveraging the **Ames Housing Dataset**. The pipeline includes data cleaning, feature engineering, hyperparameter tuning, and model evaluation.

---

## 1. Load and Preprocess Data
In this step, the dataset is loaded from a CSV file, and then missing values are handled using strategies such as median or mode filling. Certain columns may also be dropped if they exceed a missing-value threshold. Finally, the **categorical features** are one-hot encoded for compatibility with our model.

### Expected Outcome
- A clean feature set ready for modeling.  
- A numeric target column (`SalePrice`).

---

## 2. Train a Random Forest Model
After preprocessing, the data is split into **training** and **test** sets. We then perform hyperparameter tuning (e.g., `n_estimators`, `max_depth`) using techniques like **GridSearchCV** or **RandomizedSearchCV**.

### Expected Outcome
- The optimal hyperparameters for the Random Forest model.  
- A fitted model capable of predicting housing prices on unseen data.

---

## 3. Model Evaluation
We evaluate the model using **Mean Squared Error (MSE)** and **R²** on both training and test sets. These metrics help us understand the model’s accuracy and how well it generalizes.

### Expected Outcome
- **Train/Test MSE** and **Train/Test R²** values for quick comparison.  
- Evidence of whether the model is overfitting or generalizing effectively.

### Visualizations
1. **Actual vs. Predicted Plot**
![1_actual_vs_predicted](https://github.com/user-attachments/assets/8e15762b-e7a3-49ec-89b6-d0a0eb1de49d)

3. **Residual Plot**  
![2_residual_plot](https://github.com/user-attachments/assets/994be5e7-9027-43a0-b98a-824742c1ffba)

---

## 4. Feature Importance Analysis
The feature importances from the Random Forest model are extracted and visualized in a bar chart, showing which features have the greatest impact on predicting house prices.

### Expected Outcome
- A **bar chart** detailing the top contributing features for price prediction.

### Image
3. **Feature Importance Plot**  
![4_feature_importance](https://github.com/user-attachments/assets/0047837c-491d-490a-a070-938622cc77e9)

---

## How to Run
1. **Clone** this repository.  
2. **Install** dependencies from `requirements.txt` (e.g., `pip install -r requirements.txt`).  
3. **Run** the notebook or Python script to:
   - Load the Ames Housing dataset (`AmesHousing.csv`)
   - Clean and preprocess data
   - Train the Random Forest model
   - Evaluate and visualize results

Feel free to open an **issue** or submit a **pull request** if you have any suggestions or would like to contribute.  
