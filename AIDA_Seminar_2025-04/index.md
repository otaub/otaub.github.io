# Tokenization

# Natural Language Modeling

- Neural networks operate on vectors.
- How to represent language as a vector or a collection of vectors?
- Naive solution: map each letter in the alphabet to a vector. Each vector itself can be learned by the model.
- *Pro*: can be used for any language that shares that alphabet
- *Pro*: small alphabet
- *Con*: creates long sequences of embedding vectors (or tokens)
- Other extreme: encoding each word
- Compromise: encode often occurring combinations of tokens into one (-> compression algorithms)

## Side Effects

* LLMs trained on arbitrarily frankensteined together tokens are not great at counting words.
* Not mentioned: sub-word regularization, i.e. ensure consistency when multiple encodings are possible.

# Biology

- Genetic sequences 
- Letters are used to represent molecules like amino acids or nucleic acids.
- These monomers assemble into long chains.
- There can be very long range dependencies.
- Splitting into "sentences" (e.g. genes) is non-trivial

## ML on Biological Sequences

- Character level language models
- Downstream tasks include:
    - Sequence or character classification e.g. function prediction
    - Sequence or character regression e.g. solubility prediction
    - Sequence alignment
    - Structure prediction
    - Functional network prediction
- Usually uses bi-directional transformers.

## Tokenization

- Canonical letter to token
    - Small alphabet
    - Long sequences
    - Positions and length of two sequences is preserved.
- Natural language tokenizers

## Other Data Structures

- Geometric Attention Autoencoder [ESM 3](https://www.biorxiv.org/content/biorxiv/early/2024/12/31/2024.07.01.600583.full.pdf)
    - "Structural" tokenization
- Atomic tokens
    - If an amino acid is a word, an atom might be a letter.
    - On the atomic level there usually is not a sequence without forks and loops.


- [Alphafold 3](https://www.nature.com/articles/s41586-024-07487-w) can be thought of as a multi-modal model.
- It uses sequences as input and produces point clouds (atom coordinates) as output.
