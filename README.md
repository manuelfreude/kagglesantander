# Prediction for Santander Customer Transaction
kaggle competition @ https://www.kaggle.com/c/santander-customer-transaction-prediction

### Python project summary

- Loaded dataset of 200,000 rows and 202 anonymized and uncorrelated columns
- Developed 9 classifier algorithms to predict transaction probability
- Fine-tuned four top performers incl. grid search and visualized performance

### Project results

![Results](https://github.com/manuelfreude/kagglesantander/blob/master/santander_results.png)

Of the initial 9 classifiers, the best-performing ones were Bagging, AdaBoost, MLP/neural nets and LightGBM. Fine-tuning further raised each one's performance except for MLP. The best-performing algorithm was AdaBoost with a LightGBM base estimator, which was subsequently used for predicting the customer transaction probability for the test dataset in the kaggle contest.

The initial submission ranked 1,145 out of 1,398 or top 57%, and was passed down the ranks to the top 67% of 9,038 participants at the end of the competition.

![kaggle_i](https://github.com/manuelfreude/kagglesantander/blob/master/kaggle_dashboard_santander_i.png)

### Conclusion / further improvements

Santander provided a completely anonymized and uncorrelated dataset. Therefore, feature engineering along a detailed understanding of things behind the data was not possible. Feature engineering with statistical measures for the given variables (e.g. mean, running averages etc.) would have added further value to the classifier's performance. Yet the competition was more of an algorithm tuning one, I was happy with the final ranking and moved on to the LANL earthquake prediction, for which I have conducted statistical feature engineering for the given variables.
