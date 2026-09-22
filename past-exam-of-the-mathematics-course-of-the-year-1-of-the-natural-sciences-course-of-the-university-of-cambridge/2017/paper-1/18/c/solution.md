<h1 id="18/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

In $A^{\mathsf T}A$, every row sums to one, so $(1,1,1)$ is an [eigenvector](../../../../../eigenvector.md) with [eigenvalue](../../../../../eigenvalue.md) $1$. The antisymmetric direction $(1,0,-1)$ gives [eigenvalue](../../../../../eigenvalue.md) $2$. A direction orthogonal to both is $(1,-2,1)$, and direct multiplication shows that it lies in the [kernel of a linear map](../../../../../kernel-of-a-linear-map-split.md). Normalizing all three gives the complete system

$$
\boxed{\begin{array}{c|c}
\sigma_1=1&\mathbf v_1=\dfrac1{\sqrt3}(1,1,1)^{\mathsf T}\\[3pt]
\sigma_2=2&\mathbf v_2=\dfrac1{\sqrt2}(1,0,-1)^{\mathsf T}\\[3pt]
\sigma_3=0&\mathbf v_3=\dfrac1{\sqrt6}(1,-2,1)^{\mathsf T}
\end{array}}
$$

They form an [orthonormal basis](../../../../../orthonormal-basis.md) of $\mathbb R^3$. The extra zero [eigenvalue](../../../../../eigenvalue.md) reflects the one-dimensional [kernel of a linear map](../../../../../kernel-of-a-linear-map-split.md) for this rank-two rectangular [matrix](../../../../../matrix.md). The question's symbols $\sigma_m$ denote the [eigenvalues](../../../../../eigenvalue.md) of $A^{\mathsf T}A$; the nonzero [singular values](../../../../../singular-value.md) of $A$ are their [square roots](../../../../../square-root.md), namely $1$ and $\sqrt2$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [18](../../18.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
