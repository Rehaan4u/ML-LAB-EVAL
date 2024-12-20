# ML-LAB-EVAL
This work is submitted for the lab evaluation of the course Machine learning (UML501). This project aims to predict the performance of a fuel cell using machine learning techniques. 

## Methodology

1. **Data Loading and Preprocessing:**
   - The dataset is loaded using Pandas.
   - Columns ('Target1', 'Target2', 'Target3', 'Target4') are dropped according to instructions.
   - PyCaret's `setup` function is used for preprocessing, including:
     - Data splitting (70% train, 30% test)
     - Normalization (Robust scaler)
     - Transformation (Yeo-Johnson)
     - PCA (Incremental)
     - Outlier removal (5% threshold)

2. **Model Comparison and Selection:**
    - PyCaret's `compare_models` function is used to evaluate various regression models.
    - A list of 8 selected models is created for further analysis.
3. **Model Training and Evaluation:**
    - Each selected model is trained using PyCaret's `create_model` function.
    - Predictions are made on the entire dataset using `predict_model`.
4. **Results and Metrics:**
    - Performance metrics (R2, MAE, MSE,RMSE,MAPE) are collected for each model using PyCaret's `pull` function.
  
## Detailed Result Analysis
![Screenshot 2024-12-20 192506](https://github.com/user-attachments/assets/7b0bc4ba-10b0-45dc-86ef-f9049369a4fe)


## Results

The best-performing model is `Extra Trees Regressor` with an R-squared value of `0.8537`. 


