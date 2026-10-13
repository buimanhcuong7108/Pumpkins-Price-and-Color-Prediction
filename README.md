# 🎃 Predicting Pumpkin Prices

This project explores historical pumpkin prices using the records in `US-pumpkins.csv`. It walks through a basic machine-learning workflow: inspecting and preparing the data, exploring price patterns, fitting regression models, and comparing model estimates with observed prices.

## 🎯 Project goals

- 🔎 Review the dataset's available fields and check records for issues that may affect analysis.
- 🧹 Prepare relevant input features and a price value to predict.
- 📊 Explore how recorded prices vary by date, season, and other attributes present in the dataset.
- 🤖 Train regression models and evaluate their predictions against observed prices.
- ⚠️ Consider the limitations of drawing conclusions from historical data.

## 📈 Prediction with linear regression and polynomial regression

The project uses two regression approaches to estimate pumpkin prices:

- **Linear regression** provides a straightforward baseline by modeling price as a linear relationship with the selected features.
- **Polynomial regression** adds polynomial feature terms to model curved relationships that a straight-line model may not capture. Higher-degree terms can fit the training data more closely, but may also overfit, so model performance should be checked on held-out data.

Comparing the approaches helps illustrate how model complexity affects predictions. The results depend on the features selected, data preparation, and evaluation method; they should not be treated as a guarantee that one model will predict future prices accurately. ⚖️

## 🎨 Predicting pumpkin color with logistic regression

Logistic regression can also be used to classify pumpkin color. In this task, the color field is the target, and selected dataset features—excluding the target itself—are used as inputs. Prepare the features by handling missing values and encoding categorical fields, then train the classifier on a training split. Evaluate its predictions on held-out data with classification metrics such as accuracy and a confusion matrix. Results depend on the available color labels and selected features, so predictions are estimates rather than guaranteed classifications.

## 🗂️ Data and interpretation

The analysis is limited to the fields and records available in `US-pumpkins.csv`. The dataset may omit factors that influence prices, such as changes in supply, demand, or local market conditions. Predictions are estimates learned from historical observations, not guaranteed forecasts, and actual prices may differ. 📝
