<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the standard regular [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md) hypotheses: positive weight $w$, real coefficients, and real [self-adjoint](../../../../../self-adjoint-operator.md) [boundary conditions](../../../../../boundary-condition.md). The positive weight and boundary-domain assumptions are implicit in the requested real [orthonormal basis](../../../../../orthonormal-basis.md); real differential coefficients alone would not guarantee them for arbitrary complex boundary conditions.

Multiply the [eigenfunction](../../../../../eigenfunction.md) equation by $\overline{y_n}$ and integrate. By [self-adjointness](../../../../../self-adjoint-operator.md), the number $\int_a^b\overline{y_n}\mathcal Ly_n\,dx$ is real, whereas

$$
\int_a^b\overline{y_n}\mathcal Ly_n\,dx=\lambda_n\int_a^bw|y_n|^2dx.
$$

The second [integral](../../../../../integral-split.md) is strictly positive, so $\boxed{\lambda_n\in\mathbb R}$. Because the coefficients and [boundary conditions](../../../../../boundary-condition.md) are real, the real and imaginary parts of any complex [eigenfunction](../../../../../eigenfunction.md) separately obey the same equation and conditions. At least one is nonzero, so a real [eigenfunction](../../../../../eigenfunction.md) can be chosen. More generally, each [eigenspace](../../../../../eigenspace.md) has a real basis, which can be orthonormalized using the [weighted inner product](../../../../../weighted-inner-product.md).

The [orthogonality of Sturm-Liouville eigenfunctions](../../../../../orthogonality-of-sturm-liouville-eigenfunctions.md), with normalization chosen to one, is

$$
\boxed{\int_a^bw(x)\overline{y_m(x)}y_n(x)\,dx=\delta_{mn}.}
$$

For the real choice, omit the complex conjugate.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
