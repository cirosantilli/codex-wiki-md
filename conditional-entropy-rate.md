# Conditional entropy rate

↑ **Parent:** [Entropy rate](entropy-rate.md)

For a [strictly stationary process](strictly-stationary-process.md) on a [finite alphabet](finite-alphabet.md), put $a_1=H(X_1)$ and $a_n=H(X_n\mid X_1,\ldots,X_{n-1})$ for $n\geq2$. Each $a_n$ is the average remaining uncertainty in the next symbol after its history is known. More history can improve prediction, so this sequence is nonincreasing:

$$
a_{n+1}=H(X_{n+1}\mid X_1,\ldots,X_n)
\leq H(X_{n+1}\mid X_2,\ldots,X_n)=a_n.
$$

The inequality uses [conditioning reduces entropy](conditioning-reduces-entropy.md); the last equality uses [strict stationarity](strictly-stationary-process.md). Nonnegative $a_n$ therefore have a [limit](limit-of-a-function.md). By the [chain rule for information entropy](chain-rule-for-information-entropy.md),

$$
\frac{H(X_1,\ldots,X_n)}n=\frac1n\sum_{j=1}^n a_j.
$$

The [Cesàro mean](cesaro-mean.md) converges to the same [limit](limit-of-a-function.md), proving the equality with the [entropy rate](entropy-rate.md). This is a statement about average [information entropy](information-entropy-split.md). A constant almost-sure limit of the realized [information content](information-content.md) requires the further hypotheses in the [Shannon-McMillan-Breiman theorem](shannon-mcmillan-breiman-theorem.md); [stationarity without ergodicity in an information source](stationarity-without-ergodicity-in-an-information-source.md) explains the distinction.

## ↑ Ancestors (6)

1. [Entropy rate](entropy-rate.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Entropy rate](entropy-rate.md)
