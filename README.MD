# Instacart Market Basket Competition on Kaggle

This project implements four approaches to solve the Instacart Market Basket problem, with two traditional Machine Learning (ML) methods and two Deep Learning (DL) methods. For detailed instructions and explanations, please refer to the README file in each folder.

## Folder Structure and Results

### 1. **Feature_Engineering_1**: First Approach of Traditional ML
- **Description**: This approach involves feature engineering for traditional machine learning models.
- **Results**:
  - Public Score: **0.38415** (Top 670)
  - Private Score: **0.38232** (Top 650)

### 2. **Feature_Engineering_2**: Second Approach of Traditional ML
- **Description**: An alternative feature engineering strategy, tested with both LightGBM and XGBoost models.
- **Results**:
  - **LightGBM**:
    - Public Score: **0.40242** (Top 448)
    - Private Score: **0.40136** (Top 438)
  - **XGBoost**:
    - Public Score: **0.32484** (Top >1000)
    - Private Score: **0.32412** (Top >1000)

### 3. **LSTM and WaveNet**: First Approach of DL
- **Description**: A deep learning approach using LSTM and WaveNet architectures to process sequential data.
- **Results**:
  - Public Score: **0.40906** (Top 4)
  - Private Score: **0.40815** (Top 3)

### 4. **Conformer**: Second Approach of DL
- **Description**: A state-of-the-art deep learning model (Conformer) for modeling sequential and contextual dependencies. However, due to the limitation of time and resources, we've just already trained the model with 400 steps. The result was promising since it outperformed 400 steps-trained-LSTM 
- **Results of 400-steps-trained Conformer**:
  - Public Score: **0.39220** (Top 572)
  - Private Score: **0.39045** (Top 573)
- **Results of 400-steps-trained LSTM**:
  - Public Score: **0.38796** (Top 596)
  - Private Score: **0.38637** (Top 597)


https://github.com/fannam/Rec_sys_Instacart-
