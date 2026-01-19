# Lexical Semantics & Hypernym Extraction

Explored WordNet and implemented Hearst-pattern-based hypernym extraction with Python and NLP tools.

Key Steps

WordNet Exploration:

Retrieved synsets, hypernyms, troponyms, and lowest common ancestors.

Example: 'sink.n.01' → hypernym 'plumbing_fixture.n.01'; 'dog.n.01' & 'insect.n.01' → common ancestor 'animal.n.01'.

Found 5 named astronauts as instances of astronaut.n.01.

Hearst Pattern Extraction:

Implemented regex-based detection for patterns like "such X as Y" and "Y and other X" on Wikipedia sentences.

Detected candidate hyponym/hypernym pairs, with precision & recall initially ~18%.

Showed successes (e.g., "Dogs and other mammals" → ('dogs', 'mammals')) and failures (false matches due to noisy contexts).

Extension with Word Embeddings:

Used spaCy embeddings to filter unlikely hyponym candidates by computing vector similarity.

Slightly improved precision (~19%) but recall dropped (~12%), reducing false positives and increasing robustness of extractions.

Concepts & Techniques

Lexical semantics: synsets, hypernyms, troponyms, IS-A hierarchies

Hearst patterns & regex-based relation extraction

Named entity filtering & vector similarity with word embeddings

Precision/recall evaluation and error analysis

Takeaway: Simple Hearst patterns effectively detect hypernymy but struggle with noisy text; integrating embeddings improves precision, highlighting the tradeoff between recall and precision in pattern-based NLP methods.