# What Attention Buys: A Controlled Study on Multi30K

A comparison of two LSTM sequence-to-sequence models for English-to-German translation, with and without Luong attention.
- [Paper - zenodo](https://zenodo.org/records/24351642)

## Models

- [En2de](https://github.com/Meshojs/en2de): LSTM encoder-decoder without attention.
- [En2de-A](https://github.com/Meshojs/En2de-A): LSTM encoder-decoder with Luong attention.

Both models were implemented in PyTorch and trained on the Multi30K dataset.

## Results

| Model | BLEU-4 |
|---|---:|
| En2de | 16.82 |
| En2de-A | **25.14** |

**Improvement: 8.32 BLEU points.**

## Configuration

| Setting | Value |
|---|---|
| Dataset | Multi30K |
| Language pair | English → German |
| Architecture | 2-layer LSTM |
| Embedding size | 256 |
| Hidden size | 512 |
| Tokenizer | BPE (16K vocabulary) |
| Epochs | 25 |
| Optimizer | Adam |
| Decoding | Greedy |

## Paper

[Read the paper](paper.pdf)

## Author

Mashary Ramadan
