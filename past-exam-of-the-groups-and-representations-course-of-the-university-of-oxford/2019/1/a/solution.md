<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [subgroup](../../../../subgroup.md) $N\leq G$ is a [normal subgroup](../../../../normal-subgroup.md) if $gNg^{-1}=N$ for every $g\in G$. A [group homomorphism](../../../../group-homomorphism.md) $f:G\to\widetilde G$ satisfies $f(gh)=f(g)f(h)$ for every $g,h\in G$. In particular $f(e)=\widetilde e$ and $f(g^{-1})=f(g)^{-1}$. A [group representation](../../../../group-representation.md) on a [vector space](../../../../vector-space-split.md) $V$ is a [group homomorphism](../../../../group-homomorphism.md) $R:G\to\operatorname{GL}(V)$ into the [general linear group](../../../../general-linear-group.md) of invertible [linear maps](../../../../linear-map.md) on $V$.

For the [kernel of a group homomorphism](../../../../kernel-of-a-group-homomorphism.md), put $K=\ker f=\{g:f(g)=\widetilde e\}$. It contains $e$, and if $k,\ell\in K$ then $f(k\ell^{-1})=f(k)f(\ell)^{-1}=\widetilde e$, so $K$ is a [subgroup](../../../../subgroup.md). For $g\in G$ and $k\in K$,

$$
f(gkg^{-1})=f(g)f(k)f(g)^{-1}=\widetilde e.
$$

Thus $gKg^{-1}\subseteq K$. Applying this inclusion with $g^{-1}$ gives the reverse inclusion, proving that $\ker f$ is a [normal subgroup](../../../../normal-subgroup.md).

For a [normal subgroup](../../../../normal-subgroup.md) $N$, define multiplication of left [cosets](../../../../coset.md) by

$$
\boxed{(gN)(hN)=(gh)N.}
$$

To check independence of representatives, replace $g,h$ by $gn,hm$, with $n,m\in N$. Then

$$
(gn)(hm)=gh(h^{-1}nh)m\in ghN,
$$

because normality gives $h^{-1}nh\in N$. Hence the operation is well-defined. Associativity follows from $(gh)k=g(hk)$ in $G$; the identity is $N=eN$; and the inverse of $gN$ is $g^{-1}N$. These verify the [group axioms](../../../../group-axioms.md), giving the [quotient group](../../../../quotient-group.md) $G/N$. The map $g\mapsto gN$ is a surjective [group homomorphism](../../../../group-homomorphism.md) with [kernel of a group homomorphism](../../../../kernel-of-a-group-homomorphism.md) equal to $N$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
