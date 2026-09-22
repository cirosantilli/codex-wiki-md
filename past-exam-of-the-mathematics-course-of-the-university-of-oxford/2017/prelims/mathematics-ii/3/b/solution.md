<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the [radius of convergence](../../../../../../radius-of-convergence.md) of the [power series](../../../../../../power-series.md) by

$$
R=\sup\left\{|w|:w\in\mathbb C,\ \sum_{n=0}^{\infty}a_nw^n\text{ converges}\right\}\in[0,\infty],
$$

with $R=\infty$ when this [set](../../../../../../set-split.md) is unbounded. It is nonempty because the [power series](../../../../../../power-series.md) converges at zero.

If $|z|<R$, the definition of [supremum](../../../../../../supremum.md) supplies a point $w$ of convergence with $|z|<|w|$. The terms $a_nw^n$ of a convergent [series](../../../../../../series-mathematics.md) tend to zero and are bounded, say $|a_nw^n|\leq M$. Therefore

$$
|a_nz^n|\leq M\left(\frac{|z|}{|w|}\right)^n.
$$

The right-hand side has a convergent [geometric series](../../../../../../geometric-series.md), since $|z|/|w|<1$. The [comparison test](../../../../../../direct-comparison-test.md) proves [absolute convergence](../../../../../../absolute-convergence.md) at $z$.

If $|z|>R$ and the [power series](../../../../../../power-series.md) converged at $z$, then $|z|$ would belong to the [set](../../../../../../set-split.md) whose [supremum](../../../../../../supremum.md) is $R$, an immediate contradiction. Thus

$$
\boxed{|z|<R\Rightarrow\text{absolute convergence},\qquad |z|>R\Rightarrow\text{divergence}.}
$$

No assertion about the boundary $|z|=R$ follows from this argument. If $R=0$ the first assertion is vacuous; if $R=\infty$ the second is vacuous.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Mathematics II](../../../mathematics-ii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
