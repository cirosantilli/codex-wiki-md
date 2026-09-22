<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

The [contraction mapping theorem](../../../../../contraction-mapping-theorem.md) states that a [contraction mapping](../../../../../contraction-mapping.md) $T:X\to X$ on a nonempty [complete metric space](../../../../../complete-metric-space.md) has a unique [fixed point](../../../../../fixed-point.md). Here contraction means that $d(Tx,Ty)\leq qd(x,y)$ for all $x,y$, with one constant $0\leq q<1$. Choose $x_0\in X$ and define $x_{n+1}=Tx_n$. Successive distances satisfy $d(x_{n+1},x_n)\leq q^nd(x_1,x_0)$, so for every $m\geq1$,

$$
d(x_{n+m},x_n)\leq\sum_{j=n}^{n+m-1}q^jd(x_1,x_0)\leq\frac{q^n}{1-q}d(x_1,x_0).
$$

Thus $(x_n)$ is a [Cauchy sequence](../../../../../cauchy-sequence.md). Completeness gives $x_n\to x_*$. Since a [contraction mapping](../../../../../contraction-mapping.md) is a [continuous function](../../../../../continuous-function.md), $Tx_* =\lim Tx_n=\lim x_{n+1}=x_*$. If $y_*$ were another [fixed point](../../../../../fixed-point.md), $d(x_*,y_*)=d(Tx_*,Ty_*)\leq qd(x_*,y_*)$, forcing distance zero. This proves both existence and uniqueness.

Now suppose $T=f^k$ is a [contraction mapping](../../../../../contraction-mapping.md), where $k$ is a positive integer. Let $y$ be its unique [fixed point](../../../../../fixed-point.md). Since $f$ commutes with its own iterate, $T(fy)=f(Ty)=fy$. Thus $fy$ is also a [fixed point](../../../../../fixed-point.md) of $T$, so $fy=y$. Any [fixed point](../../../../../fixed-point.md) of $f$ is a [fixed point](../../../../../fixed-point.md) of $T$, and must equal $y$. **A contractive iterate therefore gives a unique [fixed point](../../../../../fixed-point.md) of $f$**, without assuming continuity of $f$ itself.

The space $X=C([0,1],\mathbb R)$ is complete for the [uniform norm](../../../../../supremum-norm.md). Indeed, a uniformly [Cauchy sequence](../../../../../cauchy-sequence.md) converges pointwise by completeness of $\mathbb R$; passing to the limit in its uniform Cauchy bound shows [uniform convergence](../../../../../uniform-convergence.md), and the uniform limit of [continuous functions](../../../../../continuous-function.md) is a [continuous function](../../../../../continuous-function.md). The operator $F$ maps this space to itself: $s\mapsto\phi(h(s),s)$ is a [continuous function](../../../../../continuous-function.md), and its integral plus the continuous $g$ is a [continuous function](../../../../../continuous-function.md).

For $n=0$ the desired bound is the definition of $\|h-k\|_\infty$. Suppose it holds for $n$. The [Lipschitz condition](../../../../../lipschitz-continuity.md) and the fact that the same $g$ cancels give

$$
\begin{aligned}|F^{n+1}(h)(t)-F^{n+1}(k)(t)|&\leq\int_0^t M|F^n(h)(s)-F^n(k)(s)|\,ds\\&\leq\frac{M^{n+1}}{n!}\|h-k\|_\infty\int_0^t s^n\,ds\\&=\frac{M^{n+1}t^{n+1}}{(n+1)!}\|h-k\|_\infty.
\end{aligned}
$$

This proves the estimate by induction. Taking the supremum over $0\leq t\leq1$, the Lipschitz constant of $F^n$ is at most $M^n/n!$. These constants tend to zero, since the ratio of successive terms is $M/(n+1)$. Some iterate is consequently a contraction. The preceding result gives a unique [fixed point](../../../../../fixed-point.md) of $F$, which is exactly $\boxed{\text{the unique continuous solution of the integral equation on }[0,1]}$. No assumption $M<1$ is needed.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
