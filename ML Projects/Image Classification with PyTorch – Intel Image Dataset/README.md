# Image Classification with PyTorch – Intel Image Dataset

Implemented image classification on the Intel Image dataset (6 classes, 128×128 RGB images) using PyTorch.

Key Steps:

Data Loading & Preprocessing: Loaded images with OpenCV, resized to 128×128, normalized pixel values to [0–1], and converted to tensors for PyTorch.

Fully Connected Neural Network: Built an MLP with dropout, achieving baseline performance on flattened image inputs (~16% accuracy due to high dimensionality).

Convolutional Neural Network (CNN): Implemented a CNN with two convolutional layers, max-pooling, and batch normalization. Achieved better performance (~20% accuracy on test set).

Regularization & Dropout: Added dropout layers to CNN for robustness. Regularization reduced variance and improved model stability across training iterations.

Concepts & Techniques:

Image preprocessing and feature scaling

Fully connected vs convolutional neural networks

Dropout and batch normalization for regularization

Model evaluation and robustness analysis

Takeaway: CNNs are more effective than MLPs for image data, and adding dropout enhances robustness and generalization, even when limited by CPU-only environments.