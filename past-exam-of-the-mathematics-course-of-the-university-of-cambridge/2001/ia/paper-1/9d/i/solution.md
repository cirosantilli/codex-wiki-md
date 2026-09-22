<h1 id="9d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $M$ bound all $|a_nw^n|$ and put $q=|z|/|w|<1$. Then

$$
|a_nz^n|=|a_nw^n|q^n\le Mq^n.
$$

The [geometric series](../../../../../../geometric-series.md) $\sum_{n=0}^\infty Mq^n$ converges, so the [comparison test for series](../../../../../../comparison-test-for-series.md) proves **absolute convergence** of $\sum a_nz^n$. This is the [bounded power-series terms force interior absolute convergence](../../../../../../bounded-power-series-terms-force-interior-absolute-convergence.md) principle.

Define the [radius of convergence](../../../../../../radius-of-convergence.md) by

$$
\boxed{\rho=\sup\{|w|:\ \sum_{n=0}^\infty a_nw^n\text{ converges}\},}
$$

allowing $\rho=0$ and $\rho=\infty$. If $|z|<\rho$, the supremum supplies a point of convergence $w$ with $|w|>|z|$; convergence makes its terms bounded, so the argument above gives [absolute convergence](../../../../../../absolute-convergence.md) at $z$. If $|z|>\rho$, convergence is impossible by definition. At $|z|=\rho$, no general conclusion follows. Thus the convergence region has a circular interior centered at zero, with boundary behavior depending on the [power series](../../../../../../power-series.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [9D](../../9d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
