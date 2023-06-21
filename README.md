# Interconnect_16thProject
Interconnect, a telecommunications operator, wants to forecast their customer churn rate. If it is known that a customer plans to leave, they will be offered promotional codes and special package options. Interconnect's marketing team has collected some customer personal data, including information about the selected data packages and their contracts.

In this project, I attempted to build a model using gradient boosting algorithms, specifically LightGBM and CatBoost. I performed target data balancing using the upsampling method and applied one-hot encoding. After tuning the hyperparameters using GridSearchCV, it was found that LightGBM achieved a higher ROC-AUC score (0.986) compared to the CatBoost model, both with max_depth=5, learning_rate=0.1, and n_estimators=200.

The values indicated by the confusion matrix were also promising, with FP (False Positive) = 13 and FN (False Negative) = 0. This means that the model successfully avoided scenarios where it wrongly offered promo codes to customers who wouldn't actually leave, and it also didn't miss out on offering anything to customers who ended up leaving.
