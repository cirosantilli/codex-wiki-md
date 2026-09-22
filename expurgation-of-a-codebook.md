# Expurgation of a codebook

↑ **Parent:** [Channel code](channel-code.md)

Expurgation discards messages with unusually high conditional decoding error. If a codebook with $2M$ equally likely messages has average error at most $\epsilon$, at least $M$ messages have individual error at most $2\epsilon$, by [Markov's inequality](markov-s-inequality.md). Retaining those messages and restricting the decoder's candidates gives a codebook with maximal error at most $2\epsilon$, provided removal of candidates cannot spoil a previously successful decoding. This is the case for [bounded-distance decoding](bounded-distance-decoding.md) with errors on ambiguity, and for a decoder that retains its former decisions whenever the decoded message remains.

For a sequence of block lengths $n$, halving a book changes its logarithmic rate by $1/n$, which tends to zero. Thus a vanishing average-error bound from a [random coding](random-coding.md) construction can be converted into a vanishing [maximal decoding error probability](maximal-decoding-error-probability.md) at the same limiting rate. The probabilistic construction first supplies a deterministic book with sufficiently small average error; expurgation is a subsequent deterministic step.

## ↑ Ancestors (7)

1. [Channel code](channel-code.md)
2. [Channel coding](channel-coding.md)
3. [Coding theory](coding-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2007/4/b/solution.md)
- [Random coding](random-coding.md)
