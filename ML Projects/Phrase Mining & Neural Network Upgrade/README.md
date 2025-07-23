# Phrase Mining & Neural Network Upgrade with MNIST
This assignment consists of two parts: a priori phrase mining from a literary corpus and extending a neural network architecture for image classification using the MNIST dataset.

Part 1: Phrase Mining from Alice in Wonderland
Used the NLTK Gutenberg corpus to load Alice in Wonderland as 1,703 transactions (sentences).

Applied a priori analysis using cleaned tokens (after removing stopwords and symbols with regex).

Explored frequent word patterns using FP-Growth via Weka or mlxtend, tuning support thresholds to discover meaningful itemsets.


Part 2: Neural Network Enhancement for MNIST
Modified the NeuralNetMLP class from a single hidden layer to a two-hidden-layer neural network.

Used ReLU activations and optimized the architecture to handle the MNIST handwritten digit dataset.

Trained and evaluated the model, achieving improved classification accuracy with the deeper architecture.

Demonstrated the benefit of additional hidden layers in learning more complex patterns from image data.

This project showcases the integration of text mining and neural network design, highlighting practical applications of both symbolic and connectionist approaches in machine learning.