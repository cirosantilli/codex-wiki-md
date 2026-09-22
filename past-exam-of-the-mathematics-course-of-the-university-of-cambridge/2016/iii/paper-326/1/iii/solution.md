<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose a [singular system of a compact operator](../../../../../../singular-system-of-a-compact-operator.md) with $Kv_j=\sigma_j u_j$, $K^*u_j=\sigma_jv_j$ and $\sigma_j>0$. The [Picard criterion](../../../../../../picard-criterion.md), together with range orthogonality, gives

$$
\boxed{f\in\operatorname{ran}K\iff f\perp\ker K^*\ \text{and}\ \sum_j\frac{|\langle f,u_j\rangle|^2}{\sigma_j^2}<\infty.}
$$

For necessity, expand a solution's component in $(\ker K)^\perp$ in the [orthonormal](../../../../../../orthonormal-set.md) vectors $v_j$; its coefficients must be $\langle f,u_j\rangle/\sigma_j$. Their square sum is finite by [Bessel's inequality](../../../../../../bessel-s-inequality.md). Conversely, the displayed square sum defines a convergent [Hilbert space](../../../../../../hilbert-space-split.md) series

$$
K^\dagger f=\sum_j\frac{\langle f,u_j\rangle}{\sigma_j}v_j.
$$

Applying the [bounded linear operator](../../../../../../continuous-linear-operator.md) $K$ to the partial sums yields the expansion of $f$ in $\overline{\operatorname{ran}K}=(\ker K^*)^\perp$. Thus its limit solves $Ku=f$. The perpendicularity condition is essential here: the [Picard criterion](../../../../../../picard-criterion.md) alone characterizes the domain of the generalized inverse, which also includes components in $\ker K^*$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
