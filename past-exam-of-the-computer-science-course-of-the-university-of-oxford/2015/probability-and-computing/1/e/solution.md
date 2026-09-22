<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Choose a positive integer-valued [random variable](../../../../../random-variable-split.md) with [probability mass function](../../../../../probability-mass-function.md)

$$
\boxed{\mathbb P(X=k)=\frac4{k(k+1)(k+2)},\qquad k=1,2,\ldots.}
$$

These masses are positive. They sum to one because the [partial fraction decomposition](../../../../../partial-fraction-decomposition.md)

$$
\frac4{k(k+1)(k+2)}=2\left(\frac1{k(k+1)}-\frac1{(k+1)(k+2)}\right)
$$

makes their sum a [telescoping series](../../../../../telescoping-series.md) with value $2/(1\cdot2)=1$. Its [expectation](../../../../../expected-value-split.md) is another [telescoping series](../../../../../telescoping-series.md):

$$
\mathbb E X=4\sum_{k=1}^\infty\frac1{(k+1)(k+2)}
=4\sum_{k=1}^\infty\left(\frac1{k+1}-\frac1{k+2}\right)=2.
$$

By contrast, since $k+1\leq2k$ and $k+2\leq3k$ for $k\geq1$, its [second moment](../../../../../second-moment.md) satisfies

$$
\mathbb E X^2=4\sum_{k=1}^\infty\frac{k}{(k+1)(k+2)}
\geq\frac23\sum_{k=1}^\infty\frac1k=\infty.
$$

The comparison uses the divergent [harmonic series](../../../../../harmonic-series.md). To check the [variance](../../../../../variance-split.md) directly, for $k\geq4$ we have $(k-2)^2\geq k^2/4$, so the corresponding tail of $\mathbb E[(X-2)^2]$ also diverges. Thus

$$
\boxed{\mathbb E X=2<\infty,\qquad\operatorname{Var}(X)=\infty.}
$$

Here “unbounded” means infinite [variance](../../../../../variance-split.md) for this single [probability distribution](../../../../../probability-distribution-split.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Probability and computing](../../../probability-and-computing-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
