# Bioinformatics

- Genetic sequences 
- Letters are used to represent molecules like amino acids or nucleic acids.
- These monomers assemble into long chains.
- There can be very long range dependencies.
- Splitting into "sentences" (e.g. genes, protein domains) is non-trivial.

![Picture](http://isw3.naist.jp/IS/Bio-Info-Unit/gogroup/study/IMG/dogma.jpg)

## ML on Biological Sequences

- Character level language models
- Downstream tasks include:
    - Sequence or character classification e.g. function prediction
    - Sequence or character regression e.g. solubility prediction
    - Sequence alignment
    - Structure prediction
    - Functional network prediction
- Usually uses bi-directional transformers.

[Tokenization](Tokenization_Bio.md)
