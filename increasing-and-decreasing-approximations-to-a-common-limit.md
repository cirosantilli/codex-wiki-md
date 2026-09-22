# Increasing and decreasing approximations to a common limit

↑ **Parent:** [Bounded monotone sequence theorem](bounded-monotone-sequence-theorem.md)

For the two [sequences](sequence.md) in [bounded monotone sequence theorem](bounded-monotone-sequence-theorem.md),

$$
a_{n+1}-a_n=\frac1{n(n+1)}>0,\qquad b_{n+1}-b_n=-\frac1{n(n+1)}<0.
$$

Their directions and bounds are explicit. One is a succession of lower approximations and the other a succession of upper approximations to the same [limit of a sequence](limit-of-a-sequence.md). To obtain [absolute error](absolute-error.md) strictly below $\varepsilon>0$, it suffices to choose an [integer](integer.md) $N>1/\varepsilon$, and then every $n\geq N$ works. For $\varepsilon=0.01$, the first such index is $101$; at $100$ the [absolute error](absolute-error.md) equals the tolerance.

A [geometric sequence](geometric-progression.md) offers a faster example. The [recurrence relation](recurrence-relation.md) $c_1=1/2$, $c_{n+1}=(c_n+1)/2$ gives $c_n=1-2^{-n}$. Thus $(c_n)$ is an increasing [bounded sequence](bounded-sequence.md) with [limit of a sequence](limit-of-a-sequence.md) one and [absolute error](absolute-error.md) $2^{-n}$. For $\varepsilon=0.01$, $n=7$ already works, since $2^{-7}=1/128<0.01$, whereas $2^{-6}=1/64>0.01$. The [bounded monotone sequence theorem](bounded-monotone-sequence-theorem.md) guarantees both examples converge; the formulas explain their different speeds.

## ↑ Ancestors (9)

1. [Bounded monotone sequence theorem](bounded-monotone-sequence-theorem.md)
2. [Monotone sequence](monotone-sequence.md)
3. [Sequence](sequence.md)
4. [Sequence and series](sequence-and-series.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Bounded monotone sequences have no universal convergence rate](bounded-monotone-sequences-have-no-universal-convergence-rate.md)
