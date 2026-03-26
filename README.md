## Project Evolution

This project follows a structured and iterative approach to understanding and predicting creative fatigue in paid social advertising.

- **Initial Phase: Rule-Based Labelling**
The study began with a rule-based fatigue labelling strategy based on consecutive declines in Click-Through Rate (CTR). While this provided an initial foundation, it resulted in limited fatigue detection and introduced class imbalance due to overly strict conditions.

- **Experimentation Phase: Modeling & Imbalance Handling**
In this phase, multiple machine learning models were explored, including Logistic Regression, Random Forest, and XGBoost. Due to the imbalance created by the initial labelling approach, techniques such as SMOTE and ADASYN were applied to improve minority class detection. This phase focused on evaluating model performance, understanding the limitations of linear approaches, and analyzing the impact of different balancing techniques.

- **Final Phase: Refined Methodology & Temporal Analysis**
The final version adopts a more robust fatigue definition based on sustained post-peak CTR decline, resulting in a more realistic and stable target variable. The modeling approach was refined, with XGBoost delivering the most consistent and reliable performance. To enhance interpretability, SHAP analysis was used to identify key drivers of fatigue. In addition, survival analysis techniques were incorporated to capture the temporal dynamics of creative fatigue, including the Kaplan–Meier survival curve to estimate fatigue probability over time and the Cox Proportional Hazards model to analyze the influence of features on the hazard of fatigue occurrence.
