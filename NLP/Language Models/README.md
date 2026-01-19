# Language Models

Implemented and evaluated character-level language models for text generation, perplexity estimation, language identification, and gender bias detection in tennis Q&A data.

Key Steps & Concepts

Character-level LM & Text Generation:

Trained 4-gram character LM on subtitles.txt.

Explored continuations for 'atio', 'nivi', 'supe'.

Generated sample text strings (up to 80 chars) showing realistic sentence fragments.

Perplexity Computation:

Implemented standard per-character perplexity and smoothed perplexity using a small constant for unseen characters.

Tested on example sentences to measure how well the model predicts natural vs. nonsense text.

Language Identification:

Trained unigram, bigram, and 4-gram models for six European languages.

Predicted language of test sentences using lowest smoothed perplexity.

Accuracy improved with higher-order n-grams:

Unigram: ~90–98%

Bigram: ~98–100%

4-gram: 99–100%

Gender Bias Detection in Tennis Questions:

Built n-gram models (1–8) to classify questions directed at male vs. female players.

Best overall accuracy with 4-gram models: ~64–67% depending on label.

Longer n-grams helped capture contextual cues in text for better predictions.

Techniques & Tools

NLP Concepts: Character n-grams, smoothing, perplexity, text generation

Applications: Language ID, bias detection, model evaluation

Libraries/Tools: Python, custom LM implementation, text preprocessing

Insights: Higher-order models improve accuracy but require more data; smoothing prevents infinite perplexity for unseen sequences; gender classification is sensitive to dataset imbalance.