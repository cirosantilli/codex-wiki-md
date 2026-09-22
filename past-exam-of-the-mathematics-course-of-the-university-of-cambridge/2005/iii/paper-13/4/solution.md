<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $\pi:E\to B$ be an oriented real [vector bundle](../../../../../vector-bundle.md) of rank $r$ over a paracompact base. A [Thom class](../../../../../thom-class.md) is a class $U\in H^r(E,E\setminus B;\mathbb Z)$ restricting on every oriented fiber pair $(\mathbb R^r,\mathbb R^r\setminus0)$ to its positive generator. The [Thom isomorphism theorem](../../../../../thom-isomorphism-theorem.md) states that this class exists uniquely with those fiber restrictions and that

$$
\boxed{H^q(B;\mathbb Z)\xrightarrow{\ \cong\ }H^{q+r}(E,E\setminus B;\mathbb Z),\qquad
 a\longmapsto\pi^*a\smile U.}
$$

Here $B$ is identified with the zero section. Equivalently use the disk/sphere bundle pair. The compact-support version is $H_c^q(B;\mathbb Z)\cong H_c^{q+r}(E;\mathbb Z)$, with fiberwise compact support in the Thom construction. If the bundle is not oriented, the integral assertion requires the corresponding [orientation local system](../../../../../orientation-local-system.md).

For a closed co-oriented embedded submanifold $Y$ of codimension $r$, co-orientation means an orientation of its normal bundle. A [tubular neighborhood](../../../../../tubular-neighborhood.md) identifies a neighborhood of $Y$ with that bundle. Its [Thom class](../../../../../thom-class.md), transferred by excision, is a class in $H^r(M,M\setminus Y;\mathbb Z)$. For compact $Y$ this maps into the direct limit defining [compactly supported cohomology](../../../../../compactly-supported-cohomology.md), giving $\boxed{\varepsilon_Y\in H_c^r(M;\mathbb Z)}$. The construction is independent of the tubular neighborhood and uses the chosen co-orientation. In an oriented ambient manifold it is the [Poincare dual](../../../../../poincare-dual.md) of the oriented submanifold. Here “closed submanifold” has the usual compact-without-boundary meaning; if it meant merely a closed subset and $Y$ were noncompact, the supported relative class would still exist but need not have compact support.

We next prove the fixed-point implication without imposing an unprinted orientability assumption on $M$. Set

$$
L(f)=\sum_k(-1)^k\operatorname{tr}(f^*:H^k(M;\mathbb Q)\to H^k(M;\mathbb Q)).
$$

Use a finite [triangulation](../../../../../triangulation.md) of the closed smooth manifold. The elementary [Hopf trace identity](../../../../../hopf-trace-identity.md) says that the alternating trace of a chain endomorphism equals its alternating trace on [homology](../../../../../homology-split.md). To verify it, split each finite-dimensional chain space as boundaries, a complement representing [homology](../../../../../homology-split.md), and a complement mapping isomorphically onto the preceding boundaries. The traces on these two boundary summands cancel in adjacent degrees, leaving exactly the [homology](../../../../../homology-split.md) traces. The [cohomology](../../../../../cohomology-split.md) traces equal the [homology](../../../../../homology-split.md) traces because the induced maps are dual over $\mathbb Q$.

If $f$ has no fixed points, compactness gives $\delta=\min_x d(x,f(x))>0$. Choose a [triangulation](../../../../../triangulation.md) $K$ of mesh less than $\delta/4$ and a sufficiently fine subdivision $K'$ admitting a simplicial approximation $F:K'\to K$ uniformly within $\delta/4$ of $f$. The subdivision [chain map](../../../../../chain-map.md) $s:C_*(K)\to C_*(K')$ sends each simplex to simplices inside it. For a vertex $v$ of such a small simplex, $d(v,F(v))>3\delta/4$, so $F(v)$ cannot lie in the original coarse simplex. Consequently $F_\#s$ has zero diagonal coefficient on every coarse simplex. Its trace vanishes in every degree, while it induces $f_*$ on [homology](../../../../../homology-split.md). The trace identity yields $L(f)=0$. Taking the contrapositive proves

$$
\boxed{L(f)\ne0\ \Longrightarrow\ f\text{ has a fixed point}.}
$$

This is the [Lefschetz fixed-point theorem](../../../../../lefschetz-fixed-point-theorem.md), established here rather than invoked. For oriented $M$ the same identity is the [graph-diagonal formula for the Lefschetz number](../../../../../graph-diagonal-formula-for-the-lefschetz-number.md): $L(f)=\langle(1,f)^*\varepsilon_\Delta,[M]\rangle$, which vanishes when the graph misses the diagonal. Finally, homotopic maps induce the same [cohomology](../../../../../cohomology-split.md) maps, so their [Lefschetz numbers](../../../../../lefschetz-number.md) agree.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
