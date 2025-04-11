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

[Biology](Biology.md)
