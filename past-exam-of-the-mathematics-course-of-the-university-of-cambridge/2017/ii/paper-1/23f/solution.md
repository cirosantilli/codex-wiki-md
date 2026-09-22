<h1 id="23f/solution">Solution</h1>

↑ **Parent:** [23F](../23f.md)

Consider the singularity of the injective [entire function](../../../../../entire-function.md) $f$ at infinity. If removable, it is bounded outside a disk and therefore bounded globally; [Liouville theorem](../../../../../liouville-theorem.md) makes it constant, a contradiction. If essential, the [Casorati-Weierstrass theorem](../../../../../casorati-weierstrass-theorem.md) says its values outside every large disk are dense. Choose a small neighbourhood $U$ of a finite point; the [open mapping theorem](../../../../../open-mapping-theorem-functional-analysis.md) puts a nonempty open disk inside $f(U)$. A point outside a disk containing $U$ would map into that open disk, duplicating a value already attained in $U$. This contradicts injectivity. Thus infinity is a pole, so $f$ is a [polynomial](../../../../../polynomial-split.md). If its degree were greater than one, its [derivative](../../../../../derivative.md) would have a root; the local power-series form at that point has local degree at least two and cannot be injective. Hence

$$
\boxed{f(z)=az+b,\qquad a\ne0}.
$$

For a nonconstant [holomorphic map](../../../../../holomorphic-map.md) of connected compact [Riemann surfaces](../../../../../riemann-surfaces.md) of degree $d$, the [Riemann-Hurwitz formula](../../../../../riemann-hurwitz-formula.md) is

$$
2g_R-2=d(2g_S-2)+\sum_{p\in R}(e_p-1),
$$

where $g_R,g_S$ are genera and $e_p$ is the local mapping degree, the multiplicity in the target fibre. There are finitely many points with $e_p>1$.

For a degree-two sphere map, the formula gives total ramification two. Since $e_p\le2$, there are exactly two distinct ramification points, each of local degree two. Their images are distinct, since a fibre has total multiplicity two. Choose a [Möbius transformation](../../../../../mobius-transformation.md) $T$ taking $0,\infty$ to these domain points and $S_0$ taking their images to $0,\infty$. The resulting rational map has its only zero at zero of order two and its only pole at infinity of order two, hence is $cz^2$ with $c\ne0$. Replace $S_0$ by $S(z)=c^{-1}S_0(z)$, obtaining

$$
\boxed{S\circ f\circ T(z)=z^2}.
$$

## ↑ Ancestors (10)

1. [23F](../23f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
