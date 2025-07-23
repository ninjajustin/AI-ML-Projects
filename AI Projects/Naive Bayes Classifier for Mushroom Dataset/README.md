# Naive Bayes Classifier for Mushroom Dataset
This project implements a Naive Bayes Classifier from scratch (without Pandas or OOP) to classify mushrooms as edible or poisonous based on their attributes.

Features
Calculates prior and conditional probabilities with optional Laplace (+1) smoothing.

Supports classification of both labeled and unlabeled data.

Evaluates model performance using 5x2 cross-validation and error rate metric.

Prints detailed error rates per fold with average and variance.

Easily extendable and reusable training, classification, and evaluation functions.

Usage
train(training_data, smoothing=True): Trains the classifier and returns the model.

classify(nbc, observations, labeled=True): Classifies given data using the trained model.

evaluate(data, classification_results): Calculates the classification error rate.

cross_validate(data, train_fn, classify_fn, folds=5, repeats=2, smoothing=True): Performs 5x2 cross-validation with detailed output.

Results & Discussion
Compares performance with and without smoothing.

Analyzes differences and hypotheses for outcomes.

Discusses relation to other classifiers like Decision Trees.