<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Suppose $m$ has no repeated irreducible factor. For every [polynomial](../../../../polynomial-split.md) $p$ and [integer](../../../../integer-split.md) $n\ge1$, its monic greatest common divisors satisfy $\gcd(p^n,m)=\gcd(p,m)$, since raising $p$ to a power changes no membership of an irreducible factor of the square-free $m$. This is the [square-free minimal polynomial criterion for polynomial kernel stabilization](../../../../square-free-minimal-polynomial-criterion-for-polynomial-kernel-stabilization.md). The kernel identity proved above gives

$$
\ker(p(T)^n)=\ker\gcd(p^n,m)(T)
=\ker\gcd(p,m)(T)=\ker p(T).
$$

Thus **(ii) implies (iii)** over every [field](../../../../field.md).

Over $\mathbb C$, the distinct irreducible factors of $m$ are linear. The [primary decomposition theorem](../../../../primary-decomposition-theorem-for-linear-maps.md) therefore reads $V=\bigoplus_j\ker(T-\lambda_jI)$, a direct sum of [eigenspaces](../../../../eigenspace.md). Taking a [basis](../../../../basis.md) in each summand gives an [eigenbasis](../../../../eigenbasis.md), proving **(ii) implies (i) over the complex numbers**.

Over $\mathbb R$, take $T=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$. Its [minimal polynomial](../../../../minimal-polynomial.md) is $X^2+1$, which is an [irreducible polynomial](../../../../irreducible-polynomial.md) over $\mathbb R$ and has no repeated factor. But it has no real [eigenvalues](../../../../eigenvalue.md), so no real [eigenbasis](../../../../eigenbasis.md). This is the required counterexample. Over a general [field](../../../../field.md), the phrase “no repeated factors” here refers to irreducible factors in $K[X]$, rather than a prior assumption that those factors split.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [2004](../../../2004-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
