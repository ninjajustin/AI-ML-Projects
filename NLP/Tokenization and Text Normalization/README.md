# Tokenization and Text Normalization

Implemented a custom tokenizer and sentence splitter in Python and compared it to NLTK's tools. The lab focused on understanding basic NLP preprocessing, collecting corpus statistics, and analyzing sentence boundaries.

Part A: Tokenization

Built a character-level tokenizer:

Lowercased text, separated punctuation, numbers, and words.

Handled edge cases like hyphenated words, contractions, and abbreviations.

Example output for "NAC has developed a National HIV/AIDS/STI/TB Intervention Strategic Plan (2002-2005).":

['nac', 'has', 'developed', 'a', 'national', 'hiv', '/', 'aids', '/', 'sti', '/', 'tb', 'intervention', 'strategic', 'plan', '(', '2002-2005', ')', '.']


Processed the first 10 lines of tokens.txt and refined edge cases.

Part B: Corpus Statistics

Processed 16,639 lines, 35,452 unique tokens, 401,411 total tokens.

Most frequent tokens: the, ., ,, to, and.

Hapax legomena: 20,197 tokens (56.97% of vocabulary).

Collected token frequencies and ranks, observing typical natural language distributions.

Part C: Zipf’s Law

Generated log-log plot of token frequency vs. rank.

Observed a roughly linear negative slope, confirming Zipf’s Law holds for the corpus.

Part D: Sentence Boundary Detection

Developed a rule-based sentence splitter:

Detected sentence-ending punctuation while accounting for abbreviations, quotes, parentheses, and edge cases.

Estimated accuracy: ~90% (passed 8/9 test cases).

Generated output file JHEDID.txt validated with provided script.

Part E: Comparison with NLTK

NLTK tokenization yielded similar results but with higher accuracy on frequent tokens.

NLTK sentence splitting handled edge cases better (abbreviations, unusual punctuation).

Custom methods provided a strong understanding of NLP preprocessing fundamentals, though NLTK is more robust for production use.

Key Concepts

Tokenization and normalization

Corpus statistics: frequency, rank, hapax legomena

Zipf’s Law visualization

Sentence boundary detection and edge cases

Comparison with NLP libraries (NLTK)

Takeaways

Building a tokenizer and sentence splitter reinforces understanding of text preprocessing challenges.

Edge cases in natural language make rule-based approaches nontrivial.

Tools like NLTK simplify robust preprocessing but custom implementation helps develop deeper NLP intuition.