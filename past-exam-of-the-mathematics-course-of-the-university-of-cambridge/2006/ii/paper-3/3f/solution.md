<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

Extend the [Möbius transformations](../../../../../mobius-transformation.md) to isometries of three-dimensional [hyperbolic space](../../../../../hyperbolic-space.md). For any interior point $o$, the [limit set of a Kleinian group](../../../../../limit-set-of-a-kleinian-group.md) is the set of boundary accumulation points of $G o$. Its definition is independent of $o$: two interior orbits stay at a bounded [hyperbolic distance](../../../../../hyperbolic-distance.md), so have the same boundary limits. The [Kleinian limit set](../../../../../limit-set-of-a-kleinian-group.md) is closed and $G$-invariant. Iterating a [loxodromic Möbius transformation](../../../../../loxodromic-mobius-transformation.md) in the positive and negative directions shows that its two fixed points belong to the [Kleinian limit set](../../../../../limit-set-of-a-kleinian-group.md).

The two fixed-point sets in this problem cannot have exactly one common point. Otherwise conjugate that point to infinity and the other fixed point of the first transformation to zero. The transformations then have the forms $f(z)=\alpha z$, with $|\alpha|>1$, and $g(z)=\beta z+b$, with $b\ne0$. But $f^{-n}gf^n(z)=\beta z+b\alpha^{-n}$ is a sequence of distinct group elements converging in the [Möbius group](../../../../../mobius-group.md). Taking quotients of consecutive elements gives nonidentity elements converging to the identity, contrary to [discrete subgroup](../../../../../discrete-subgroup.md). Consequently the [Kleinian limit set](../../../../../limit-set-of-a-kleinian-group.md) contains at least three points.

Let $\xi$ be any point of the [Kleinian limit set](../../../../../limit-set-of-a-kleinian-group.md), and choose distinct $g_n$ with $g_no\to\xi$. The [rank-one convergence of divergent Möbius transformations](../../../../../rank-one-convergence-of-divergent-mobius-transformations.md) supplies a subsequence converging to $\xi$ uniformly away from one exceptional boundary point $\eta$. To see the lemma directly, normalize determinant-one representing [matrices](../../../../../matrix.md) by their norms. The norms tend to infinity, and a subsequential limit has rank one: its kernel is $\eta$ and its image is the attracting point. In the positive-Hermitian-matrix model of [hyperbolic space](../../../../../hyperbolic-space.md), $g_no$ has this same image limit, so the attracting point is indeed $\xi$.

Choose distinct $\zeta_1,\zeta_2$ in the [Kleinian limit set](../../../../../limit-set-of-a-kleinian-group.md) other than $\eta$. Then $g_n\zeta_1$ and $g_n\zeta_2$ both tend to $\xi$, belong to the [Kleinian limit set](../../../../../limit-set-of-a-kleinian-group.md), and remain distinct because $g_n$ is injective. If $\xi$ were isolated, both would eventually equal $\xi$, an impossibility. **The limit set has no isolated points.**

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
