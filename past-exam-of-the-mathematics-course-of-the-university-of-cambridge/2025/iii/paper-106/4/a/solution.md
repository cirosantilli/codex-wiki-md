<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a real [locally convex space](../../../../../../locally-convex-space.md) $(X,\mathcal P)$, the [continuous dual space](../../../../../../continuous-dual-space-split.md) $X^*$ consists of all continuous real-linear maps $X\to\mathbb R$. If $g\in Y^*$ on a subspace $Y$, continuity gives seminorms $p_1,\ldots,p_k\in\mathcal P$ and $C>0$ such that

$$
|g(y)|\leq C\max_i p_i(y)
\qquad(y\in Y).
$$

The right side is a continuous sublinear functional on $X$. The dominated [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) extends $g$ to a linear $f:X\to\mathbb R$ satisfying the same bound, so $f\in X^*$.

If $Y$ is closed and $x_0\notin Y$, the Hausdorff locally convex quotient $X/Y$ has a continuous seminorm $p$ with $p(x_0+Y)>0$. On $Y+\mathbb Rx_0$, define $g(y+tx_0)=t$ and rescale $p$ so that $|g|\leq p$. Hahn--Banach extends it to $f\in X^*$ with $f|_Y=0$ and $f(x_0)=1$.

The [separation of a point and an open convex set](../../../../../../separation-of-a-point-and-an-open-convex-set.md) says that if $C\subseteq X$ is nonempty, open, and convex and $x_0\notin C$, there is $f\in X^*$ such that

$$
f(c)<f(x_0)
\qquad(c\in C).
$$

To prove it, choose $a\in C$, put $U=C-a$, and let $p_U$ be its [Minkowski functional](../../../../../../minkowski-functional.md). For $z=x_0-a\notin U$, $p_U(z)\geq1$. Define $h(tz)=tp_U(z)$ on $\mathbb Rz$; then $h\leq p_U$. Hahn--Banach extends $h$ to $f\leq p_U$. Since $p_U(u)<1$ for $u\in U$, one has $f(c-a)<1\leq f(x_0-a)$, proving the claim.

If $K$ is closed and convex and $x_0\notin K$, a [Hahn-Banach separation theorem](../../../../../../hahn-banach-separation-theorem.md) gives $f\in X^*$ and a real number separating $x_0$ from $K$. The corresponding inverse image of an open interval is a weak neighbourhood of $x_0$ disjoint from $K$, so $K$ is closed in $\sigma(X,X^*)$.

The unit sphere $S_X$ of a normed space is norm closed. If $X$ is infinite-dimensional, every basic weak neighbourhood of an interior point $x\in B_X$ constrains only finitely many functionals $f_1,\ldots,f_n$. Their common kernel contains a nonzero $y$. Continuity of $t\mapsto\|x+ty\|$, together with its value below one at $t=0$ and divergence as $|t|\to\infty$, supplies $t$ with $\|x+ty\|=1$. Since all $f_i$ have the same values at $x+ty$ and $x$, every weak neighbourhood of $x$ meets $S_X$. Points outside $B_X$ are separated from it by Hahn--Banach, so the [weak closure of the unit sphere](../../../../../../weak-closure-of-the-unit-sphere.md) is exactly $B_X$. In particular, $S_X$ is not weakly closed.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
