<h1 id="1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [natural filtration](../../../../../../natural-filtration.md) $\mathcal F_n=\sigma(X_1,\ldots,X_n)$. The first exit time is a [stopping time](../../../../../../stopping-time.md). If $r\leq x$, it is zero, so its expectation is already finite. Now assume $0<x<r$.

The positive-increment hypothesis gives a number $h>0$ with $\mathbb P(X_1>h)>0$. Choose an integer $m$ so large that $r/m<h$, and put $p=\mathbb P(X_1>r/m)>0$. A block of $m$ increments all exceeding $r/m$ has probability $p^m$. From any point still in $(0,r)$, that block forces an upper exit before the block ends.

By [independence](../../../../../../independent-random-variables.md), conditional on $\mathcal F_{km}$ and survival to time $km$, the next block has this same probability. Thus the [geometric tail bound from a uniform escape probability](../../../../../../geometric-tail-bound-from-a-uniform-escape-probability.md) gives

$$
\mathbb P(\eta>(k+1)m)\leq(1-p^m)\mathbb P(\eta>km),
\qquad\mathbb P(\eta>km)\leq(1-p^m)^k.
$$

Using the tail-sum formula for the [expected value](../../../../../../expected-value.md) of a nonnegative integer-valued [random variable](../../../../../../random-variable-split.md),

$$
\boxed{\mathbb E\eta=\sum_{n=0}^\infty\mathbb P(\eta>n)\leq m\sum_{k=0}^\infty(1-p^m)^k=\frac{m}{p^m}<\infty.}
$$

This is the [random-walk exit bound from a positive-increment block](../../../../../../random-walk-exit-bound-from-a-positive-increment-block.md). In particular, the exit occurs with probability one. The mean-zero assumption is not needed for this first bound.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [1](../../1.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
