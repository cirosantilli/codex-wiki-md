<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The printed assertion for every cohomological degree is false.** The valid conclusion supplied by the stated [Hartogs extension theorem](../../../../../../hartogs-s-extension-theorem.md) is the degree-zero isomorphism. Indeed, around each removed point choose a small coordinate ball on which the [holomorphic vector bundle](../../../../../../holomorphic-vector-bundle.md) $E$ is trivial. A [holomorphic section](../../../../../../holomorphic-section.md) on the punctured ball has finitely many holomorphic coefficient functions, each of which extends by [Hartogs extension theorem](../../../../../../hartogs-s-extension-theorem.md) when the complex dimension is at least two. Uniqueness of holomorphic extension makes these local extensions agree with the original section on overlaps, giving

$$
\boxed{H^0(X,\mathcal O(E))\cong H^0(X_0,\mathcal O(E|_{X_0})).}
$$

This also identifies the [direct image sheaf](../../../../../../direct-image-sheaf.md) $j_*\mathcal O(E|_{X_0})$ with $\mathcal O(E)$ for the inclusion $j:X_0\hookrightarrow X$. It does not identify higher [sheaf cohomology](../../../../../../sheaf-cohomology.md).

Here is an explicit higher-degree obstruction. Take $X=\mathbb P^2$, remove $[0:0:1]$, and take the trivial line bundle. Cover $X_0$ by $U=\{x\ne0\}$ and $V=\{y\ne0\}$. On $U$ use coordinates $t=y/x$, $s=z/x$; on $V$ use $u=x/y=1/t$, $v=z/y=s/t$. Both charts are $\mathbb C^2$, and the overlap is $\mathbb C^*\times\mathbb C$. For every integer $m\geq2$, the [holomorphic function](../../../../../../holomorphic-function.md)

$$
g_m=\frac{z^m}{x^{m-1}y}=\frac{s^m}{t}
$$

defines a [Čech cocycle](../../../../../../cech-cocycle-condition.md). It cannot be a [Čech coboundary](../../../../../../cech-coboundary.md) $b(1/t,s/t)-a(t,s)$ with $a,b$ entire on their charts. Taking the coefficient of $s^m$, the term from $a$ has only nonnegative powers of $t$, whereas the term from $b$ has the form $t^{-m}b_m(1/t)$ and only powers at most $-m$. Neither can provide the coefficient $t^{-1}$. Uniqueness of [Laurent series](../../../../../../laurent-series.md) proves the contradiction. The same argument applied to each fibre degree proves that all the classes $[g_m]$, $m\geq2$, are linearly independent.

These classes remain nonzero in [Čech cohomology](../../../../../../cech-cohomology.md) of $X_0$, rather than merely of this cover. The low-degree [Mayer-Vietoris sequence for sheaf cohomology](../../../../../../mayer-vietoris-sequence-for-sheaf-cohomology.md) injects the quotient of overlap sections by the two chart-section groups into $H^1(X_0,\mathcal O)$. Concretely, a [partition of unity](../../../../../../partition-of-unity.md) gives smooth $f_U,f_V$ with $f_V-f_U=g$; their common [Dolbeault operator](../../../../../../dolbeault-operator.md) defines a global $(0,1)$-form. If that form were $\bar\partial$-exact, subtracting its global smooth primitive would make $f_U,f_V$ holomorphic and split $g$. The nonsplitting just proved therefore gives the same obstruction in [Dolbeault cohomology](../../../../../../dolbeault-cohomology.md), and the [Dolbeault theorem](../../../../../../dolbeault-theorem.md) identifies it with [sheaf cohomology](../../../../../../sheaf-cohomology.md). Thus $H^1(X_0,\mathcal O)$ is infinite dimensional. In contrast, $H^1(\mathbb P^2,\mathcal O)$ is finite dimensional by compact [Dolbeault Hodge decomposition](../../../../../../dolbeault-hodge-decomposition-on-a-compact-hermitian-manifold.md) for the [Fubini-Study form](../../../../../../fubini-study-form.md). Hence **the two degree-one groups cannot be isomorphic**, disproving the printed all-degree request already in complex dimension two.

In complex dimension one, even the degree-zero conclusion fails. Take $X=\mathbb P^1$, remove its point at infinity and use the trivial line bundle. Holomorphic functions on compact connected $\mathbb P^1$ are constant by the [maximum modulus principle](../../../../../../maximum-modulus-principle.md), whereas $X_0\cong\mathbb C$ has nonconstant entire functions such as $z$. Therefore **the restriction map is not onto even in degree zero**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
