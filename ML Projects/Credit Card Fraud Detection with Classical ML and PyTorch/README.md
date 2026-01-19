# Credit Card Fraud Detection with Classical ML and PyTorch

Implemented a fraud detection system on the Kaggle Credit Card Fraud dataset (~285k transactions, 31 features) using classical ML and PyTorch neural networks.

Key Steps:

Data Exploration & Preprocessing: Checked dataset integrity, visualized distributions, handled class imbalance (~0.17% fraud), and standardized numeric features.

Evaluation Metric: Used F1 score due to extreme class imbalance.

Baseline Models: SVC, Decision Tree, MLP, Random Forest (50/50 train-test split). Random Forest and MLP performed best.

Regularization & Tuning: Optimized hyperparameters for SVC, Decision Tree, and MLP; improved generalization and stability.

Custom PyTorch Models: Implemented MLP with two hidden layers; extended with dropout for robustness.

Cross-Validation: 10-fold CV confirmed consistent performance (~0.81 F1) across all models.

Concepts & Techniques:

Imbalanced classification, feature scaling, hyperparameter tuning

Neural network implementation in PyTorch (forward pass, training loop)

Regularization (L2, dropout) and ensemble methods

Cross-validation for reliable evaluation

Practical ML engineering: handling environment issues, reproducibility

Takeaway: Robust, regularized models like Random Forest and MLP with dropout achieve reliable fraud detection while generalizing well to unseen data.