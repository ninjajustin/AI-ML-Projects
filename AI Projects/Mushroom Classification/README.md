# Decision Tree Classifier with ID3 Algorithm on Mushroom Dataset
In this assignment, I implemented a Decision Tree classifier using the ID3 algorithm (without pruning or normalized information gain) to classify mushrooms based on their attributes. Key aspects include:

Data: Used the UCI Mushroom dataset (preprocessed by removing instances with missing values "?").

Implementation Restrictions:

No Pandas or OOP — used Python built-ins like dictionaries and named tuples as abstract data types.

Recursive tree construction following the ID3 pseudocode.

Core Functions:

train(training_data): builds the decision tree data structure from training data.

classify(tree, observations): classifies new data based on the learned tree.

evaluate(dataset, classifications): computes the classification error rate (not accuracy).

cross_validate(data): performs 5x2 fold cross-validation with shuffled folds, printing error rates with 4 decimal precision following course standards.

pretty_print_tree(tree): outputs a readable textual representation of the final decision tree trained on the full dataset.

Handling Missing Values: Removed observations containing missing attribute values to simplify training and classification.

This project demonstrates a fundamental machine learning pipeline from data preprocessing, model training, evaluation using proper cross-validation, and interpretable model visualization.