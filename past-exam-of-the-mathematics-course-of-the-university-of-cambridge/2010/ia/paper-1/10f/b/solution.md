<h1 id="10f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The assumed [differentiability](../../../../../../differentiability.md) makes $e$ continuous. The identity $e'=e$ then implies inductively that $e$ has continuous [derivatives](../../../../../../derivative.md) of every order and

$$
e^{(k)}(t)=e(t)\quad(k\geq0),\qquad e^{(k)}(0)=1.
$$

Fix $x\ne0$. By the [extreme value theorem](../../../../../../extreme-value-theorem.md), the [continuous function](../../../../../../continuous-function.md) $|e|$ is bounded on the closed interval between $0$ and $x$; let $M_x$ be its maximum. Applying the [Taylor theorem with Lagrange remainder](../../../../../../taylor-theorem-with-lagrange-remainder.md) about $0$ gives some $\xi_n$ between $0$ and $x$ such that

$$
e(x)=\sum_{k=0}^n\frac{x^k}{k!}
+\frac{e(\xi_n)}{(n+1)!}x^{n+1},
\qquad
\left|e(x)-\sum_{k=0}^n\frac{x^k}{k!}\right|
\leq M_x\frac{|x|^{n+1}}{(n+1)!}.
$$

For the last factor, successive ratios are $|x|/(n+2)$, which are at most $1/2$ once $n$ is sufficiently large. A [geometric sequence](../../../../../../geometric-progression.md) bound therefore proves that $|x|^{n+1}/(n+1)!\to0$. The [partial sums](../../../../../../partial-sum.md) converge to $e(x)$, so

$$
\boxed{e(x)=\sum_{n=0}^{\infty}\frac{x^n}{n!}\quad\text{for every }x\in\mathbb R.}
$$

At $x=0$ the equality follows directly from $e(0)=1$. The proof obtains this [Taylor series](../../../../../../taylor-series.md) solely from the differential identity, continuity on a fixed finite interval, and the [Taylor remainder](../../../../../../taylor-remainder.md) estimate.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10F](../../10f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
