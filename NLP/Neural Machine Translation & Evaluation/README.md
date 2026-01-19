# Neural Machine Translation & Evaluation

Explored Neural Machine Translation (NMT) using Joey NMT, Opus-MT, and M2M100 models, and evaluated translations with standard metrics.

Key Steps

Model Comparison:

Joey RNN vs. Joey Transformer on WMT English→German benchmark.

Transformer BLEU 27.4 outperformed RNN BLEU 26.0 and slightly exceeded Sockeye’s best-reported scores.

Spanish → English Translation:

Translated 1,012 sentences using Opus-MT and M2M100 models.

Evaluation metrics:

Opus-MT: BLEU 28.56, ChrF 58.35, TER 60.91

M2M100: BLEU 23.77, ChrF 55.06, TER 66.40

Round-Trip Translation:

Translated English → Spanish → French → Russian → English.

Overall meaning preserved; minor changes in phrasing and detail observed (e.g., “influenced” → “suffers”).

User Study:

6 experts vs. 8 novices on translation tasks using Joey NMT.

Experts completed the quiz faster (77 min) and with higher accuracy (82%) than novices (118 min, 66%).

Concepts & Techniques

Neural machine translation (RNNs, Transformers)

Translation evaluation metrics: BLEU, ChrF, TER

Round-trip translation to test meaning preservation

User study design and analysis for usability and comprehension

Takeaway

Transformers outperform RNNs in translation quality. Round-trip translation preserves overall meaning but can introduce minor phrasing errors. User expertise significantly affects translation speed and accuracy, highlighting the importance of human factors in NMT deployment.