<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Because $F_1$ is [projective twistor space](../../../../../../projective-twistor-space.md), the printed column represents the line $p=[e_1]$, not a distinguished nonzero vector. Its [stabilizer subgroup](../../../../../../stabilizer-subgroup.md) consists of matrices whose first column is a nonzero multiple of $e_1$:

$$
\boxed{H_p=\left\{\begin{pmatrix}a&b\\0&B\end{pmatrix}:B\in GL(3,\mathbb C),\ b\in\mathbb C^{1\times3},\ a\det B=1\right\}.}
$$

The block form is necessary to preserve the line, and conversely every such determinant-one matrix preserves it. By transitivity, the orbit map $g\mapsto g[e_1]$ is onto $F_1$. Its two values agree precisely when $g^{-1}g'\in H_p$, equivalently when $gH_p=g'H_p$. This gives the [homogeneous space](../../../../../../homogeneous-space.md) identification

$$
\boxed{F_1\cong SL(4,\mathbb C)/H_p.}
$$

The dimensions also agree: $\dim_{\mathbb C}SL(4)=15$, while the free $B$ and $b$ parameters give $\dim_{\mathbb C}H_p=9+3=12$; the quotient has dimension three.

**This coset space is not a quotient group**, because $H_p$ is not a [normal subgroup](../../../../../../normal-subgroup.md). For example $h=I+E_{12}\in H_p$. Let $g$ have upper-left block $\begin{pmatrix}0&-1\\1&0\end{pmatrix}$ and identity on the other two coordinates. Then $g\in SL(4,\mathbb C)$ but $ghg^{-1}=I-E_{21}$ sends $e_1$ to $e_1-e_2$, so it is not in $H_p$. Thus multiplying coset representatives does not define a well-defined group operation.

If instead one required the literal vector $e_1$ to be fixed, one would have $a=1$ and $B\in SL(3,\mathbb C)$; its quotient would be $\mathbb C^4\setminus\{0\}$, not $F_1$. The projective reading is required by the printed target quotient and the [flag manifold](../../../../../../flag-manifold.md) definition.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
