# Retail Sales Prediction - Regression Supervised ML Project
## Project Overview
This project focuses on tackling the business problem of accurately predicting sales figures using multiple regression algorithms. By analyzing historical sales data and leveraging advanced machine learning techniques, we aimed to enhance forecasting precision significantly, thereby supporting data-driven decision-making and improving sales strategies for the business.

## Data Preparation and Cleaning
## Handling Zero Sales Rows
Initially, we observed that the Sales column contained 172,817 rows with zero sales. To investigate the impact of these zero sales on our model's performance, we created two separate dataframes:

Filtered Dataframe: Removed rows with zero sales and trained the model on the remaining data.
Complete Dataframe: Included all rows, including those with zero sales, and trained another model.
Training the model on the filtered dataframe yielded an accuracy score of around 74%. However, when we trained the model using the complete dataframe, we achieved an accuracy near 98%. This significant improvement led us to conclude that the zero sales rows contain valuable information, and removing them would result in a loss of crucial data. Therefore, we decided to retain these rows for our final model.

## Exploratory Data Analysis (EDA)
Using Python, Pandas, and Matplotlib, we conducted detailed EDA to uncover trends and analyze historical sales data. Key factors influencing sales, such as promotions, holidays, and competition, were identified. This analysis provided actionable insights for strategic planning, highlighting the importance of these factors in predicting sales accurately.

## Data Preprocessing
Given the large dataset with over a million entries, effective data preprocessing was crucial. We employed various techniques to prepare the data for model training:

One-Hot Encoding: Categorical variables were transformed into numerical format using one-hot encoding.
Standard Scaling: Data was scaled to ensure uniformity and improve the performance of machine learning algorithms.
Handling Missing Values: Missing values were addressed using appropriate strategies, ensuring the completeness and accuracy of the dataset.
These preprocessing steps were implemented using Scikit-learn, which provided robust tools for efficient data preparation.

## Model Training and Evaluation
Algorithms Used
We experimented with various regression algorithms to identify the best-performing model. The algorithms included:

Random Forest: Provided the best RMPSE (Root Mean Square Percentage Error) score.
Gradient Boosting Techniques: Implemented algorithms like AdaBoost and XGBoost, which showed promising results.
## Hyperparameter Tuning
To enhance model performance, we performed hyperparameter tuning. This process involved adjusting the model parameters to find the optimal settings that prevent overfitting and improve generalization. We used techniques such as grid search and cross-validation to systematically explore different parameter combinations.

## Evaluation Metrics
Models were evaluated using metrics such as R2 score and mean squared error (MSE). These metrics helped in assessing the accuracy and reliability of the predictions. The high accuracy of 98% achieved by our final model underscored the effectiveness of our approach.

## Key Insights and Conclusions
The key insights from this project are:

Retention of Zero Sales Rows: Removing rows with zero sales significantly reduces the amount of information available to the model. Retaining these rows led to a substantial improvement in prediction accuracy.
Importance of EDA: Detailed exploratory data analysis revealed critical factors influencing sales, such as promotions and holidays, which are vital for accurate forecasting.
Robust Preprocessing: Effective data preprocessing, including handling missing values and scaling, is essential for improving model performance.
Model Performance: The Random Forest algorithm and gradient boosting techniques provided the best results, with the final model achieving a prediction accuracy of 98%.
