# HausaMT v1.0: Towards English–Hausa Neural Machine Translation

This is an ongoing work on Neural Machine Translation for English-Hausa. According to [Sebastian Ruder](https://ruder.io/4-biggest-open-problems-in-nlp/), one of the biggest open problems for NLP is NMT for low-resource languages. NMT suffers a language diversity problem and growing up in a multi-lingual community with about 300 languages and thousands of dialects, I decided to work on NMT for the second largest Afro-Asiatic language after Arabic — Hausa Language. Hausa is also the third largest trade language across a larger swathe of West Africa after English and French. I have started working on this and the results are pretty good so far. I’m currently collaborating with scholars from the [Niger-Volta Language Technologies Institute](https://github.com/Niger-Volta-LTI) and working with some starter notebooks created by the [Masakhane](https://www.masakhane.io) community.


# Datasets and Summary
![](https://github.com/WalePhenomenon/Hausa-NMT/blob/master/Table1.png)


### Pre-Processing and Training

- We used Byte Pair Encoding (BPE) word-level tokenization
- Trained using the Transformer Encoder-Decoder architecture on [JoeyNMT](https://joeynmt.readthedocs.io/en/latest/)
- 30 epochs
- Plateau scheduling
- Learning rate: 0.0003
- 4096 batch size
- Xavier initializer (same used for embedding layer)
- For transformer encoder and decoder: 6 layers, 4 heads, 256 embedding dim, 0.2 embedding dropout rate, 0.3 dropout rate, 256 hidden layer size

### Results

![](https://github.com/WalePhenomenon/Hausa-NMT/blob/master/Table2.png)

![Sample Translation](https://github.com/WalePhenomenon/Hausa-NMT/blob/master/Old_Hausa_MT/Dev_Test_1_Examples.png)







