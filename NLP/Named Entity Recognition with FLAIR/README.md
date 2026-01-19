# Named Entity Recognition with FLAIR

Implemented a neural sequence tagger for Named Entity Recognition (NER) using the FLAIR LSTM-CRF framework on the CoNLL 2003 English dataset. Explored training dynamics, data size effects, label simplification, and custom examples.

Key Steps

Corpus & Label Setup:

Loaded CoNLL 2003 data (train, dev, test).

Built label dictionary for LOC, PER, ORG, MISC.

Model & Training:

Used StackedEmbeddings: GloVe + forward/backward Flair embeddings.

Bi-LSTM + CRF sequence tagger trained for multiple runs (max 20 epochs).

Evaluated variability across runs:

F1-Score: min 0.9205, mean 0.9222, max 0.9232

Individual entity performance: PER highest (~0.97 F1), MISC lowest (~0.82 F1).

Visualized training loss and F1-score over epochs for dev/test sets.

Training Data Size Effects:

Incrementally trained on chunks of 25K lines to study learning curves.

Observed F1-score generally increased with more data, plateauing as more training lines were added.

Label Simplification (Type-agnostic NER):

Mapped all entity types to a single ENT label.

Achieved higher overall scores (Precision 0.9466, Recall 0.9566, F1 0.9516).

Demonstrated that fewer labels simplify the model’s task, improving performance.

Custom Test Sentences:

Created 10+ sentences with PER, ORG, LOC entities, including easy and difficult examples.

Model correctly identified well-known and lesser-known entities alike (e.g., IU → PER, The Academy → ORG, Busan → LOC).

Concepts & Techniques

Sequence labeling with Bi-LSTM + CRF

Pretrained embeddings: GloVe + Flair (contextualized embeddings)

Training dynamics, variability, and F1 evaluation

Data scaling and learning curves

Label simplification and its effect on performance

Custom evaluation on real-world sentences

Takeaways

FLAIR’s Bi-LSTM-CRF tagger is highly effective for NER; careful embedding choices improve performance.

Increasing training data improves F1, but returns diminish as model converges.

Simplifying labels can significantly boost precision and F1.

Model performs well even on unseen, less-common entities, demonstrating robustness for real-world text.