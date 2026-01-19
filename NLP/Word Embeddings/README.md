# Word Embeddings

Explored static and contextual word embeddings using Word2Vec, pretrained Google News vectors, and SpaCy contextual embeddings, with visualization and analysis of semantic relationships.

Part A: Static Word Embeddings

Data & Setup: Tokenized 50,000-line corpus (small.txt) with SpaCy; trained Word2Vec (100-dimensional, skip-gram).

Visualization: Reduced embeddings to 2D with UMAP; semantically related words clustered together (e.g., france-paris, russia-moscow).

Pretrained Embeddings: Loaded Google News vectors for higher-quality embeddings.

Analyses:

Similarity & Distance: Tested similarity scores (mother/father vs mother/ocean) and distances.

Most Similar Words: Found nearest neighbors for words like 'fascinating', 'cultivate', 'eggplant'.

Analogies: Explored vector arithmetic (puppies:dog :: X:cat, queen = king - man + woman) and observed unexpected top results in some cases.

Relationship Reasoning:

Synonyms and similar words identifiable by similarity and neighbors.

Antonyms, related words, and hierarchical relationships (subordinate/superordinate) are difficult to infer using only embeddings.

Unrelated words generally have low similarity.

Part B: Contextual Word Embeddings

Used SpaCy to extract contextual embeddings per word in sentence context.

Sense Analysis:

Example word 'bank' in river vs money contexts; embeddings clustered correctly by sense using UMAP, showing contextual separation.

Created custom multi-sense words to validate embedding distinctions.

Comparison: Averaged contextual embeddings for words from Part A; observed similarities to static embeddings but with context-dependent variations.

Key Concepts

Static embeddings vs contextual embeddings

Vector arithmetic for analogy reasoning

Cosine similarity and distance measures

Dimensionality reduction with UMAP for visualization

Sense disambiguation using contextual embeddings

Takeaways

Word2Vec effectively captures semantic similarity and analogy relationships, though limited for antonyms or hierarchical relations.

Contextual embeddings can separate multiple senses of the same word, providing richer representations.

Visualization via UMAP provides intuitive insight into semantic structure of embeddings.