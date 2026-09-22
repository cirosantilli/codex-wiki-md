# Binary rate-distortion function

↑ **Parent:** [Hamming distortion](hamming-distortion.md)

For a stationary source of [independent and identically distributed](independent-and-identically-distributed-random-variables.md) fair [bits](bit.md), with [Hamming distortion](hamming-distortion.md) and binary [reconstruction alphabet](reconstruction-alphabet.md),

$$
\boxed{R(D)=\begin{cases}1-h_2(D),&0\leq D\leq1/2,\\0,&D\geq1/2.\end{cases}}
$$

The [binary entropy](binary-entropy.md) convention is $0\log_2 0=0$. Once $D\geq1/2$, always reconstructing zero meets the distortion constraint without sending any [bits](bit.md). The formula $1-h_2(D)$ must not be extended to $D>1/2$: a looser constraint cannot increase the required rate.[§25.1.1, Bernoulli Source, printed p. 255](6-441-information-theory-spring-2016-lecture-notes-by-yury-polyanskiy-and-others/chapter-25-evaluating-r-d-lossy-source-channel-separation.md)

The short argument identifies both sides of the optimum. For any feasible binary reconstruction, put $E=X\oplus\widehat X$, using [exclusive or](exclusive-or.md). Knowing $\widehat X$ makes $X$ and $E$ determine one another, so the [conditional entropy](conditional-entropy.md) obeys

$$
H(X\mid\widehat X)=H(E\mid\widehat X)\leq H(E)=h_2(\mathbb P(E=1))\leq h_2(D)
$$

when $0\leq D\leq1/2$. The last step uses the increase of [binary entropy](binary-entropy.md) on that interval. Hence $I(X;\widehat X)=1-H(X\mid\widehat X)\geq1-h_2(D)$. Conversely, choose $\widehat X=X\oplus N$ with an [independent](independent-random-variables.md) [Bernoulli random variable](bernoulli-distribution.md) $N$ of parameter $D$. This [binary symmetric channel](binary-symmetric-channel.md) has [expected distortion](expected-distortion.md) $D$ and [mutual information](mutual-information.md) $1-h_2(D)$, attaining the bound.

## ↑ Ancestors (8)

1. [Hamming distortion](hamming-distortion.md)
2. [Rate-distortion function](rate-distortion-function.md)
3. [Rate-distortion theory](rate-distortion-theory.md)
4. [Information theory](information-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Rate-distortion function](rate-distortion-function.md)
