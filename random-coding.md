# Random coding

↑ **Parent:** [Channel code](channel-code.md)

Random coding constructs a [channel code](channel-code.md) by sampling its codewords from a specified probability distribution and bounding the expected decoding error over that ensemble. If the expected average error is at most $\epsilon$, at least one deterministic codebook has average error at most $\epsilon$; otherwise every book would exceed the expectation bound. This is the [probabilistic method](probabilistic-method.md) applied to communication codes.

For independently uniform binary codewords, a fixed competing word falls in any received word's radius-$r$ [Hamming ball](hamming-ball.md) with probability $2^{-n}\sum_{j=0}^r\binom nj$. The [union bound](boole-s-inequality.md) over competing messages, together with a bound on excessive channel noise, yields the basic random-coding error estimate. [Expurgation of a codebook](expurgation-of-a-codebook.md) can then convert average-error control to [maximal decoding error probability](maximal-decoding-error-probability.md) with negligible loss of asymptotic rate.

## ↑ Ancestors (7)

1. [Channel code](channel-code.md)
2. [Channel coding](channel-coding.md)
3. [Coding theory](coding-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Expurgation of a codebook](expurgation-of-a-codebook.md)
