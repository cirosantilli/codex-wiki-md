<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [scalar fields](../../../../scalar-field.md) commute, so a degree-$d$ expression in one doublet belongs to a [symmetric power](../../../../symmetric-power.md), rather than an arbitrary [tensor product](../../../../tensor-product.md). Put $x=\phi_1$, $y=\phi_2$. The [generators of a group](../../../../generator-of-a-group.md) $r=\tau_1\tau_2$ and $s=\tau_3$ act by

$$
r:(x,y)\mapsto(\alpha x,\alpha^{-1}y),\qquad s:(x,y)\mapsto(y,x).
$$

A [monomial](../../../../monomial.md) $x^a y^b$ is fixed by $r$ precisely when $a-b$ is divisible by three. Imposing $s$ then pairs the exponents. Through degree four the resulting holomorphic [polynomial invariants](../../../../polynomial-invariant.md) are

$$
\begin{array}{c|l}
\text{degree}&\text{basis}\\\hline
0&1\\
1&\text{none}\\
2&xy\\
3&x^3+y^3\\
4&x^2y^2
\end{array}
$$

In particular, two explicit invariant terms are $\phi_1\phi_2$ and $\phi_1^3+\phi_2^3$. Their invariance follows directly from $\alpha^3=1$ and the interchange of the two components. A quartic example is $(\phi_1\phi_2)^2$.

For a physical real [scalar potential](../../../../scalar-potential.md), [complex conjugate](../../../../complex-conjugate.md) fields are allowed as well. The [Hermitian inner product](../../../../hermitian-inner-product.md) $\phi^\dagger\phi$ and its square are also invariant, while a holomorphic term can enter with its [complex conjugate](../../../../complex-conjugate.md), for example $b(\phi_1^3+\phi_2^3)+\bar b(\bar\phi_1^3+\bar\phi_2^3)$. There is still no invariant linear term, because neither the doublet nor its [conjugate representation](../../../../conjugate-representation.md) contains a [trivial representation](../../../../trivial-representation.md). Thus the possible nonconstant total degrees are

$$
\boxed{S_3:\quad 2,3,4.}
$$

The constant term is unrestricted.

For the [fundamental representation](../../../../fundamental-representation.md) of the [special unitary group](../../../../special-unitary-group.md) $SU(2)$, its central element $-I$ sends $\phi\mapsto-\phi$ and $\bar\phi\mapsto-\bar\phi$. Every odd-degree [polynomial](../../../../polynomial-split.md) changes sign, excluding degrees one and three. Further, $SU(2)$ acts transitively on the unit sphere in $\mathbb C^2$: a unit vector $(u,v)^T$ is the first column of

$$
\begin{pmatrix}u&-\bar v\\v&\bar u\end{pmatrix}\in SU(2).
$$

An invariant [polynomial](../../../../polynomial-split.md) must therefore depend only on $\phi^\dagger\phi$. Through quartic order the general real [scalar potential](../../../../scalar-potential.md) is

$$
\boxed{V=V_0+m^2\phi^\dagger\phi+\lambda(\phi^\dagger\phi)^2,
\qquad V_0,m^2,\lambda\in\mathbb R.}
$$

Hence the possible nonconstant degrees are $2,4$; the cubic term permitted by $S_3$ is excluded by $SU(2)$.

If the notation $V(\phi)$ is instead read as restricting to holomorphic [polynomials](../../../../polynomial-split.md) alone, the distinction matters: a single commuting $SU(2)$ doublet has no nonconstant holomorphic [polynomial invariant](../../../../polynomial-invariant.md). The candidate contraction $\epsilon_{ab}\phi_a\phi_b=\phi_1\phi_2-\phi_2\phi_1$ vanishes identically. The quadratic and quartic $SU(2)$ terms above require [complex conjugate](../../../../complex-conjugate.md) fields. This also explains why counting a [trivial representation](../../../../trivial-representation.md) in $\mathbf2\otimes\mathbf2$ alone would give an incorrect holomorphic answer.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
