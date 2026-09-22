<h1 id="31e/solution">Solution</h1>

↑ **Parent:** [31E](../31e.md)

A map is [Devaney-chaotic](../../../../../devaney-chaos.md) on $\Lambda$ when it is [topologically transitive](../../../../../topological-transitivity.md), it has [dense periodic points](../../../../../dense-periodic-points.md) in $\Lambda$, and it has [sensitive dependence on initial conditions](../../../../../butterfly-effect.md). A one-dimensional map is [Glendinning-chaotic](../../../../../glendinning-chaos.md) when some iterate has a [horseshoe for an interval map](../../../../../horseshoe-for-an-interval-map.md): there are an interval $J$ and two disjoint subintervals $K_0,K_1\subseteq J$ such that $F^n(K_0)=F^n(K_1)=J$.

The map $F(x)=ax\pmod1$ is the [beta transformation](../../../../../beta-transformation.md) with slope $a>1$. On every interval of continuity of $F^n$, it is affine with slope $a^n$. The endpoints of these intervals are iterated preimages of the discontinuity set. Choosing $n$ with $a^n>2$, the standard full-branch lemma for the beta transformation supplies two disjoint continuity intervals $K_0,K_1$ on which $F^n$ maps bijectively onto $[0,1)$. Thus $F^n$ has a horseshoe, proving Glendinning chaos.

For Devaney chaos one may either use the standard theorem that a full-branch expanding interval map is Devaney-chaotic, or verify its ingredients directly. Every nonempty open interval expands by the factor $a$ on each uninterrupted iterate; after subdivision at preimages of discontinuities, one of its images contains a full branch and hence eventually covers $[0,1)$. This proves topological transitivity. Applying an inverse branch of a sufficiently high iterate to a full branch gives a contraction whose unique fixed point is periodic; choosing the branch inside any prescribed open interval proves that periodic points are dense. Finally, two sufficiently close points that follow the same branch separate by the factor $a$ on each iterate until their distance exceeds a fixed positive constant, proving sensitive dependence. Hence $F$ is also Devaney-chaotic for every real $a>1$.

## ↑ Ancestors (10)

1. [31E](../31e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
