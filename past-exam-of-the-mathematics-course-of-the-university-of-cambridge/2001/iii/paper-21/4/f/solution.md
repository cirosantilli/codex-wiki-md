<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**True.** The preceding distributional argument alone shows that almost-sure convergence to zero cannot hold with [probability](../../../../../../probability.md) one. To establish almost-sure nonconvergence, rather than merely failure of a probability-one convergence claim, use the [Kolmogorov zero-one law](../../../../../../kolmogorov-s-zero-one-law.md).

Let $A=\{B_n/\sqrt n\to0\}$. For every fixed $m$, subtracting $B_m/\sqrt n\to0$ shows that

$$
A=\left\{\frac{\sum_{k=m+1}^n(B_k-B_{k-1})}{\sqrt n}\longrightarrow0\right\}.
$$

Thus $A$ belongs to the [tail sigma-algebra](../../../../../../tail-sigma-algebra.md) of the independent unit-time increments; it is a [tail event](../../../../../../tail-event.md). The [Kolmogorov zero-one law](../../../../../../kolmogorov-s-zero-one-law.md) gives $\mathbb P(A)\in\{0,1\}$. If its [probability](../../../../../../probability.md) were one, then $B_n/\sqrt n\to0$ in [probability](../../../../../../probability.md), contrary to its standard [normal distribution](../../../../../../normal-distribution.md) at every $n$. Therefore $\mathbb P(A)=0$. Continuous-time convergence would imply integer-time convergence, so

$$
\boxed{\mathbb P\bigl(B_t/\sqrt t\text{ does not converge to }0\bigr)=1.}
$$

The more general [Brownian fluctuations exceed the square-root scale](../../../../../../brownian-fluctuations-exceed-the-square-root-scale.md) result is consistent with this direct tail-event proof. No [independence](../../../../../../independent-random-variables.md) of the normalized values themselves has been assumed.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [4](../../4.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
