<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $v_2,v_3,v_4$ be the three supplied coefficient vectors, in their displayed order. Multiplication by the [sample covariance matrix](../../../../../../../sample-covariance-matrix.md) gives

$$
\begin{aligned}
\Sigma v_2&=(408,0,-408,4080)^T=408v_2,\\
\Sigma v_3&=(300,-600,300,0)^T=300v_3,\\
\Sigma v_4&=(2040,0,-2040,-408)^T=204v_4.
\end{aligned}
$$

The four vectors are pairwise orthogonal, with norms $\sqrt3$, $\sqrt{102}$, $\sqrt6$ and $\sqrt{204}$. Hence $u_j=v_j/\|v_j\|$ form an [orthonormal basis](../../../../../../../orthonormal-basis.md) of [eigenvectors](../../../../../../../eigenvector.md). The [variance](../../../../../../../variance-split.md) of the [principal component](../../../../../../../principal-component.md) with unit coefficient vector $u_j$ is its [eigenvalue](../../../../../../../eigenvalue.md) $\lambda_j$. Using unnormalized coefficient vectors would instead give variances $\lambda_j\|v_j\|^2$ and would not produce the desired proportions.

The total [variance](../../../../../../../variance-split.md) is

$$
\operatorname{tr}\Sigma=904+950+904+404=3162=2250+408+300+204.
$$

Therefore the [explained variance of a principal component](../../../../../../../explained-variance-of-a-principal-component.md) is

$$
\boxed{\begin{array}{c|r|r}
\text{component}&\lambda_j&100\lambda_j/3162\\\hline
1&2250&71.16\%\\
2&408&12.90\%\\
3&300&9.49\%\\
4&204&6.45\%
\end{array}}
$$

The first two [principal components](../../../../../../../principal-component.md) together account for $2658/3162\simeq84.06\%$, and the first three account for $2958/3162\simeq93.55\%$ of the total [variance](../../../../../../../variance-split.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 46](../../../../paper-46-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
