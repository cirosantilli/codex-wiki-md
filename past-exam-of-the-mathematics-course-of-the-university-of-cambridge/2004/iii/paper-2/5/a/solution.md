<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $g\in GL_n(q)$, make $V=\mathbb F_q^n$ a [module](../../../../../../module-mathematics.md) over the [polynomial ring](../../../../../../polynomial-ring.md) $R=\mathbb F_q[t]$ by $t\cdot v=gv$. The [structure theorem for finitely generated modules over a principal ideal domain](../../../../../../structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain.md) and [primary decomposition](../../../../../../primary-decomposition.md) give

$$
V\cong\bigoplus_{f\ne t}\bigoplus_{j\ge1}\bigl(R/(f^j)\bigr)^{m_j(f)}.
$$

Here $f$ ranges over [monic polynomials](../../../../../../monic-polynomial.md) that are [irreducible polynomials](../../../../../../irreducible-polynomial.md), and $t$ is excluded because $g$ is invertible. Associate the [integer partition](../../../../../../integer-partition.md) $\lambda_f$ having $m_j(f)$ parts equal to $j$. It has finite support and satisfies $\sum_f\deg(f)|\lambda_f|=n$. Two matrices are conjugate exactly when their R-modules are isomorphic, so this gives a bijective parameterization of [conjugacy classes](../../../../../../conjugacy-class.md).

The [centralizer](../../../../../../centralizer.md) is the R-module [automorphism](../../../../../../automorphism.md) [group](../../../../../../group-split.md). Homomorphisms between distinct primary components vanish: coprimeness of their annihilating [polynomials](../../../../../../polynomial-split.md) makes each such map zero. Fix one $f$ of degree $d$, put $Q=q^d$, and write $m_j=m_j(f)$. A map $R/(f^a)\to R/(f^b)$ is determined by an [image](../../../../../../image-of-a-function.md) killed by $f^a$, so its space has dimension $d\min(a,b)$ over $\mathbb F_q$. Consequently the [endomorphism](../../../../../../endomorphism.md) algebra $E$ has

$$
|E|=Q^{\sum_{a,b}\min(a,b)m_am_b}=Q^{\sum_i(\lambda'_i)^2},
$$

where $\lambda'$ is the [conjugate partition](../../../../../../conjugate-partition.md).

Its semisimple quotient is $\prod_jM_{m_j}(\mathbb F_Q)$: reduce the maps between the equal-length summands modulo $f$ and discard the maps between unequal lengths. Composition through a different length acquires a factor of $f$ when it returns to the original length, so these reductions define an algebra homomorphism. It is onto, and its [kernel](../../../../../../kernel-of-a-linear-map.md) is nilpotent. One can see the latter directly by expanding a sufficiently long product into paths through the finitely many possible summand lengths: repeated returns through unequal lengths or equal-length [kernel](../../../../../../kernel-of-a-linear-map.md) factors accumulate powers of $f$, while a strictly monotone path has bounded length. Eventually every path vanishes in every summand.

An element is invertible exactly when its [image](../../../../../../image-of-a-function.md) in that quotient is invertible, since a nilpotent error is inverted by a finite [geometric series](../../../../../../geometric-series.md). The fraction of units is therefore $\prod_j|GL_{m_j}(Q)|/Q^{m_j^2}=\prod_j\prod_{r=1}^{m_j}(1-Q^{-r})$. Multiplying the independent primary contributions gives the [primary matrix centralizer formula](../../../../../../primary-matrix-centralizer-formula.md):

$$
\boxed{|C_{GL_n(q)}(g)|=\prod_{f\ne t}q^{\deg(f)\sum_i(\lambda'_{f,i})^2}\prod_{j\ge1}\prod_{r=1}^{m_j(f)}(1-q^{-r\deg(f)}).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
