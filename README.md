# Forest-Cover-Type-Classification-
Forest cover type classification using Decision Tree, Random Forest, and XGBoost. Random Forest achieved the best performance (95.55% accuracy) with faster training compared to XGBoost, making it the most practical choice.
## Dataset  

**Note:** The dataset is larger than GitHub’s 25 MB file size limit, so it is not stored in this repository.  
You can download it directly from the official source here:  

🔗 [UCI Covertype Dataset](https://archive.ics.uci.edu/ml/datasets/covertype)  

After downloading, place the dataset (CSV file) into the project folder (e.g., `data/` directory) before running the code.  

## Methodology  
1. **Data Cleaning & Preprocessing**  
   - Handled categorical variables and missing values.  
   - Scaled/encoded features where necessary.  
2. **Model Training**  
   - Baseline model: Decision Tree.  
   - Ensemble models: Random Forest and XGBoost.  
3. **Evaluation**  
   - Accuracy, confusion matrix, and feature importance.  
   - Hyperparameter tuning for each model.  
4. **Comparison**  
   - Trade-offs between accuracy, training time, and resource usage.  

## Results  
- **Decision Tree**:  
  - Baseline accuracy: 93.89% → 94.25% after tuning.  
  - Simple and interpretable, but less robust.  

- **Random Forest**:  
  - Best accuracy: **95.55%** with 120 trees.  
  - Outperformed Decision Tree and trained much faster than XGBoost.  
  - Best balance of performance and efficiency.  

- **XGBoost**:  
  - Accuracy: 95.19% with tuned parameters (n_estimators=2000, learning_rate=0.05, max_depth=7).  
  - Very computationally expensive (~20 min training vs. 4 min for Random Forest).  

## Tools & Libraries  
- Python  
- Pandas – preprocessing  
- Scikit-learn – Decision Tree, Random Forest, evaluation  
- XGBoost – gradient boosting  
