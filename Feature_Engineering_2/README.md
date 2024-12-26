# Instacart Market Basket Competition on Kaggle

This project focuses on solving the Instacart Market Basket problem with multiple approaches. Please note that the folder structure and file paths may vary slightly as Google Colab and Kaggle environments are used for execution. Ensure that you modify the directory paths accordingly for your code.

The solution is based on the public code of *University of Macedonia* and top 2 competition *ONODERA*.

## Steps to Run the Code

1. **Run `prepare_data_and_word2vec_fe2.ipynb`**:
   - This script prepares the features required for the XGBoost and LightGBM models.

2. **Run `submission_xgb_lgbm_fe2.ipynb`**:
   - This script trains the models (XGBoost and LightGBM) on the prepared features and generates predictions for submission.

## Important Notes on Features

### User Statistics:
- **`user_orders`**: Total number of orders placed by a user.
- **`user_order_stat_at`**: Total number of days since the user started placing orders.
- **`user_mean_days_since_prior`** & **`user_median_days_since_prior`**: Average and median time between user orders.
- **`user_total_products`**: Total number of products purchased by the user.
- **`user_distinct_products`**: Number of distinct products purchased by the user.
- **`user_reorder_ratio`**: Ratio of reordered products by the user.
- **`user_average_basket`**: Average basket size of the user.

### User-Product Statistics:
- **`up_orders`**: Total number of users who purchased a specific product.
- **`up_first_order`**: The order number when the user first purchased the product.
- **`up_last_order`**: The order number when the user last purchased the product.
- **`up_mean_cart_position`** & **`up_median_cart_position`**: Average and median position of the product in the user's cart.
- **`day_since_prior_order_mean`** & **`day_since_prior_order_median`**: Average and median time between purchases of the product.
- **`user_product_reordered_ratio`**: Reorder ratio for a specific user-product pair.
- **`up_order_rate`**: Order rate of the product compared to the total orders of the user.
- **`up_order_since_last_order`**: Number of orders since the user last purchased the product.

### Order Statistics:
- **`last`**: The most recent time between two purchases.
- **`prev1`**: Time since the previous purchase (set to 9999 if the product has not been purchased before).
- **`prev2`**: Time since the second-to-last purchase (set to 9999 if it doesn't exist).
- **`mean`** & **`median`**: Average and median time between consecutive purchases for all products.

## Folder Structure and File Information

- **`Feature_Engineering_2`**:
  - Contains the second approach for feature engineering and traditional ML.
  - Files:
    1. `prepare_data_and_word2vec_fe2.ipynb`: Script for feature preparation.
    2. `submission_xgb_lgbm_fe2.ipynb`: Script for model training and submission.

## Note

Ensure you adapt the folder paths in your code based on the working environment (e.g., Google Colab or Kaggle Notebook) to avoid path errors.
