<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $S=s=\begin{pmatrix}0&1\\1&0\end{pmatrix}$. Entrywise [complex conjugation](../../../../complex-conjugation.md) interchanges the diagonal entries of $r$ and fixes $s$, so

$$
SR_2(r)^*S^{-1}=R_2(r),\qquad SR_2(s)^*S^{-1}=R_2(s).
$$

Since $r,s$ generate the [group](../../../../group-split.md), these identities hold for every element. Thus $S$ is an invertible [intertwiner](../../../../intertwiner.md), proving

$$
\boxed{R_2^*\cong R_2.}
$$

The [character](../../../../character-of-a-representation.md) of a [tensor product representation](../../../../tensor-product-of-group-representations.md) is the product of the factor [characters](../../../../character-of-a-representation.md). Hence $\chi_{R_2\otimes R_2}=(4,1,0)$. Its [character inner products](../../../../character-inner-product.md) with the three rows of [solution](../c/solution.md) give multiplicities $(1,1,1)$, so

$$
\boxed{R_2\otimes R_2\cong\mathbf1\oplus\varepsilon\oplus R_2.}
$$

For explicit [Clebsch-Gordan decomposition of group representations](../../../../clebsch-gordan-decomposition-of-group-representations.md) [bases](../../../../basis.md), let $e_+,e_-$ be the coordinate [basis](../../../../basis.md). The [symmetric tensor](../../../../symmetric-tensor.md) $e_+\otimes e_-+e_-\otimes e_+$ spans $\mathbf1$; the [antisymmetric tensor](../../../../antisymmetric-tensor.md) $e_+\otimes e_--e_-\otimes e_+$ spans $\varepsilon$; and the ordered pair $e_-\otimes e_-,e_+\otimes e_+$ carries $R_2$, since $r$ acts by $\operatorname{diag}(\alpha,\alpha^2)$ and $s$ exchanges them. In particular $S^2R_2=\mathbf1\oplus R_2$ and $\Lambda^2R_2=\varepsilon$.

Multiplying by the [sign representation](../../../../sign-representation.md) preserves the [character](../../../../character-of-a-representation.md) of $R_2$, because its [character](../../../../character-of-a-representation.md) is zero on all three reflections. Thus $\varepsilon\otimes R_2\cong R_2$, and associativity gives

$$
\begin{aligned}
R_2^{\otimes3}
&\cong(\mathbf1\oplus\varepsilon\oplus R_2)\otimes R_2\\
&\cong R_2\oplus R_2\oplus(\mathbf1\oplus\varepsilon\oplus R_2).
\end{aligned}
$$

Therefore

$$
\boxed{R_2\otimes R_2\otimes R_2\cong\mathbf1\oplus\varepsilon\oplus3R_2.}
$$

The [dimensions](../../../../dimension-vector-space.md) give $8=1+1+3\cdot2$. Its two one-dimensional summands can also be seen directly: $e_+^{\otimes3}+e_-^{\otimes3}$ and $e_+^{\otimes3}-e_-^{\otimes3}$ transform as $\mathbf1$ and $\varepsilon$, respectively.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
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
