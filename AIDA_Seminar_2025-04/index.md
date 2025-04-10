# Tokenization

# Natural Language Modeling
- Neural networks operate on vectors.
- How to represent language as a vector or a collection of vectors?
- Naive solution: map each letter in the alphabet to a vector. Each vector itself can be learned by the model.
- :smile: can be used for any language that shares that alphabet
- :smile: small alphabet
- :frowning: creates long sequences of embedding vectors (or tokens)
- Other extreme: encoding each word
- Compromise: encode often occuring combinations of tokens into one (-> compression algorithms)

## Side Effects
* LLMs trained on arbitrarily frankensteined together tokens are not great at counting words.
* Not mentioned: subword regularization, i.e. ensure consistency when multiple encodings are possible.

# Biology
- Genetic sequences 

## Biological Sequences
## Other Data Structures
- [Alphafold 3](https://www.nature.com/articles/s41586-024-07487-w) can be thought of as a multi-modal model.
- It uses sequences as input and produces point clouds (atom coordinates) as output.
