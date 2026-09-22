<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [minimal polynomial](../../../minimal-polynomial.md) of $T$ is the monic nonzero [polynomial](../../../polynomial-split.md) of smallest degree annihilating $T$. Such a [polynomial](../../../polynomial-split.md) exists, since sufficiently many powers of $T$ are linearly dependent in the finite-dimensional space $\operatorname{End}(V)$. If two monic annihilators had the same least degree, their difference would be an annihilator of smaller degree and hence zero. Thus it is unique. Division with remainder also shows that every annihilating [polynomial](../../../polynomial-split.md) is a multiple of it.

The [primary decomposition theorem](../../../primary-decomposition-theorem-for-linear-maps.md) states that if $m=\prod_{j=1}^r f_j^{e_j}$ with distinct monic [irreducible polynomials](../../../irreducible-polynomial.md), then

$$
V=\bigoplus_{j=1}^r V_j,\qquad V_j=\ker f_j(T)^{e_j}.
$$

These subspaces are $T$-invariant, and the restriction to $V_j$ has [minimal polynomial](../../../minimal-polynomial.md) $f_j^{e_j}$.

Let $r=\gcd(q,m)$, chosen monic. The [Bézout's identity for polynomials](../../../bezout-s-identity-for-polynomials.md) gives $r=aq+bm$. If $q(T)v=0$, then $r(T)v=a(T)q(T)v+b(T)m(T)v=0$. Conversely, $q=rh$, so $r(T)v=0$ implies $q(T)v=0$. Therefore

$$
\boxed{\ker q(T)=\ker\gcd(q,m)(T).}
$$

The following Roman scopes correspond to the three labelled conditions, with their implications proved from the indicated condition.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2004](../../2004-split.md)
3. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations II course of the University of Oxford](../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
