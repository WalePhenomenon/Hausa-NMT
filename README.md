# Hausa-NMT: Empirical Study of Neural Machine translation for English-Hausa-English

This is an ongoing work on Neural Machine Translation for English-Hausa. According to [Sebastian Ruder](https://ruder.io/4-biggest-open-problems-in-nlp/), one of the biggest open problems for NLP is NMT for low-resource languages. NMT suffers a language diversity problem and growing up in a multi-lingual community with about 300 languages and thousands of dialects, I decided to work on NMT for the second largest Afro-Asiatic language after Arabic — Hausa Language. Hausa is also the third largest trade language across a larger swathe of West Africa after English and French. I have started working on this and the results are pretty good so far. I’m currently collaborating with scholars from the [Niger-Volta Language Technologies Institute](https://github.com/Niger-Volta-LTI) and working with some starter notebooks created by the [Masakhane](https://www.masakhane.io) community.

# First Run

### Dataset used for first trial run

- English - Hause Parallel Corpus from JW300 Dataset on Opus
- 237,065 parallel sentences
- Reduced to 212,320 after dropping duplicates
- Split into train (168,856), test (41,464) and dev (1,000) set

### Pre-Processing and Training

- Byte Pair Encoding (BPE) was used to tokenize and “boost” performance
- Trained using the Transformer Encoder-Decoder architecture on [JoeyNMT](https://joeynmt.readthedocs.io/en/latest/)
- 30 epochs
- Plateau scheduling
- Learning rate: 0.0003
- 4096 batch size
- Xavier initializer (same used for embedding layer)
- For transformer encoder and decoder: 6 layers, 4 heads, 256 embedding dim, 0.2 embedding dropout rate, 0.3 dropout rate, 256 hidden layer size

### Results: Validation Loss and Bleu Score


## Second Run

- Trained on more datasets
- Added Tanzil (Quran), Wikimedia and Tatoeba parallel corpus to it.
- Total number of en-ha parallel sentences: 351,024
- Training set: 98%, dev: 1000, test: 2%
- Used BPE and the same architecture

### Results on Dev Test for Second Run




