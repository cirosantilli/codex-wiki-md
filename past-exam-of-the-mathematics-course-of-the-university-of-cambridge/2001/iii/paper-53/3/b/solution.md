<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $B=\{p:\|p-p_0\|\leq r\}$ and write $\varepsilon=\|A(p_0)-p_0\|$. Integrating the [Fréchet derivative](../../../../../../frechet-derivative.md) along the line segment between two points in the [convex set](../../../../../../convex-set.md) gives

$$
A(p)-A(q)=\int_0^1 DA(q+t(p-q))(p-q)\,dt,
$$

and the [operator norm](../../../../../../operator-norm.md) bound implies

$$
\|A(p)-A(q)\|\leq\kappa\|p-q\|.
$$

In particular, for $p\in B$,

$$
\|A(p)-p_0\|\leq\|A(p)-A(p_0)\|+\varepsilon
\leq\kappa r+\varepsilon\leq r.
$$

Thus the [a posteriori contraction ball](../../../../../../a-posteriori-contraction-ball.md) is mapped into itself. The ball is a closed subset of a [Banach space](../../../../../../banach-space-split.md), hence is a [complete metric space](../../../../../../complete-metric-space.md). Applying the [contraction mapping theorem](../../../../../../contraction-mapping-theorem.md) to $A:B\to B$ gives existence and uniqueness:

$$
\boxed{\varepsilon\leq(1-\kappa)r\quad\Longrightarrow\quad
\text{exactly one fixed point }p_*\in B.}
$$

The estimate also gives $\|p_*-p_0\|\leq\varepsilon/(1-\kappa)$, by applying the same triangle inequality to $A(p_*)=p_*$. Equality in the residual bound is allowed; strict [contraction mapping](../../../../../../contraction-mapping.md) comes from $\kappa<1$, and a [fixed point](../../../../../../fixed-point.md) on the closed ball's boundary is included.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
