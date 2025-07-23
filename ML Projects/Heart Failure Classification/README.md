# Ensemble Learning with Bagging on Heart Failure Classification
In this assignment, I explored ensemble methods using Bagging to improve classification performance on the Kaggle heart failure dataset.

I first preprocessed the dataset by converting nominal features to numerical using techniques like OneHotEncoding and verified the baseline performance of several classifiers (GaussianNB, Linear SVC, MLPClassifier, DecisionTreeClassifier) with 10-fold cross-validation. RandomForestClassifier was also evaluated as a baseline ensemble method.

Next, I generated ensembles of 100 weak classifiers for each base classifier by underpowering their hyperparameters (e.g., shallow decision trees, small neural networks with limited training iterations).

I implemented two key functions:

ensemble_fit() to train each weak classifier on a random subsample of the training data (bagging),

ensemble_predict() to aggregate predictions from all classifiers in an ensemble via majority voting based on predicted probabilities.

I evaluated ensemble performances over multiple subsample ratios (0.005 to 0.2) using 10-fold cross-validation and compared them to regular classifiers trained on the full dataset or same subsample ratios.

Finally, I visualized the performance of ensembles versus regular classifiers across different subsample ratios for each classifier type, highlighting how bagging improves robustness and accuracy under limited data scenarios.

This assignment demonstrated the benefits and trade-offs of ensemble learning with Bagging, especially for small or noisy datasets in medical classification tasks.