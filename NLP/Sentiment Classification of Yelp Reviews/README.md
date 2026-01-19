# Sentiment Classification of Yelp Reviews

Built and evaluated binary classifiers to predict whether Yelp restaurant reviews are positive (4 stars) or negative (2 stars). Explored feature engineering, supervised learning models, and evaluation metrics.

Key Steps

Data Exploration & Feature Analysis:

Loaded train.tsv, dev.tsv, and test.tsv (balanced dataset: 1,000 positive, 1,000 negative reviews per file).

Tokenized text and analyzed word frequencies for positive/negative sentiment.

Example features and relative frequencies:

Word	Pos %	Neg %
good	56.96	43.80
great	40.24	18.20
delicious	14.91	3.50
friendly	17.72	7.60
not	47.95	71.70
bad	7.61	17.30
like	35.44	43.60
don't	16.62	23.70
never	15.12	12.90
love	22.12	11.40

Observed polarized reviews with slang, sarcasm, and varying length; dataset is balanced.

Classifier 1 – Logistic Regression (Bag-of-Words):

Vectorized text using CountVectorizer (tokenized words, max 5,000 features, binary presence).

Trained Logistic Regression (max_iter=200).

Dev set evaluation:

Precision: 0.8261

Recall: 0.8368

F1 Score: 0.8314

Identified misclassifications, often due to mixed sentiment or minor negative mentions in otherwise positive reviews.

Classifier 2 – Multinomial Naive Bayes:

Same bag-of-words features, trained MultinomialNB.

Dev set evaluation:

Precision: 0.8332

Recall: 0.8348

F1 Score: 0.8340

Slight improvement over Logistic Regression; both classifiers performed similarly overall.

Feature Engineering Enhancements:

Added bigrams to capture word pairs for more context (e.g., "delicious food", "horrible service").

Added English sentiment dictionary using NLTK SentiWordNet to compute review-level sentiment scores.

Best performance achieved with Naive Bayes + bigram features:

Precision: 0.8351

Recall: 0.8519

F1 Score: 0.8434

Test Set Predictions:

Generated predictions for test.tsv using the best model (Naive Bayes + bigrams).

Concepts & Techniques

Text preprocessing and tokenization

Bag-of-words and bigram feature representation

Supervised classifiers: Logistic Regression, Naive Bayes

Feature engineering using sentiment lexicons

Evaluation metrics: precision, recall, F1 score

Analysis of misclassified examples to understand model limitations

Takeaways

Bag-of-words features provide a strong baseline for sentiment classification.

Adding bigrams and lexicon-based sentiment features improves performance by capturing context and word sentiment.

Classifier errors often occur with mixed sentiment reviews or subtle sarcasm, highlighting the challenge of real-world user-generated text.

Naive Bayes was slightly better than Logistic Regression for this task, likely due to its effectiveness with word-count distributions in text.