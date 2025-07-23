# Suicide Rate Prediction Using Machine Learning
In this assignment, I explored the "Suicide Rates Overview 1985 to 2016" dataset from Kaggle, aiming to develop a machine learning model to predict whether a given instance corresponds to a low or high suicide rate (a binary classification problem).

I began by defining the big-picture question of what critical information can be learned from the dataset to aid in understanding and potentially preventing suicides, acknowledging the complexity and severity of the problem.

Next, I determined the appropriate problem setup as a classification task rather than regression, while also considering whether unsupervised approaches could reveal useful patterns in the data.

I identified the dependent variable to be a binary indicator of low vs. high suicide rate, formulated based on the distribution of the target metric ("number of suicides per 100k").

Then, I analyzed correlations between independent variables and the dependent variable to rank feature importance, guiding feature selection.

I pre-processed the dataset by removing redundant or derived features, selecting a core set of independent features to use for the model while avoiding multicollinearity.

Finally, I implemented a prototype classification model to predict suicide rate categories, focusing on functionality over performance as a foundation for further improvement in future modules.