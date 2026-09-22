<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose a complete orthonormal system of [eigenfunctions](../../../../../../eigenfunction.md) $\phi_n$ for the [self-adjoint](../../../../../../self-adjoint-operator.md) problem. Expand $f=\sum_n f_n\phi_n$ and $y=\sum_n c_n\phi_n$, with

$$
f_n=\langle\phi_n,f\rangle=\int_a^b\phi_n^*(\xi)f(\xi)w(\xi)\,d\xi.
$$

Substitution into $Ly=f$ gives $\lambda_nc_n=f_n$. Since no [eigenvalue](../../../../../../eigenvalue.md) is zero, the [Sturm-Liouville eigenfunction expansion](../../../../../../sturm-liouville-eigenfunction-expansion.md) is

$$
\boxed{y(x)=\sum_n\frac{\phi_n(x)}{\lambda_n}\int_a^b\phi_n^*(\xi)f(\xi)w(\xi)\,d\xi.}
$$

For [eigenfunctions](../../../../../../eigenfunction.md) not normalized to one, divide each term additionally by $\langle\phi_n,\phi_n\rangle$. The expansion is understood in the weighted function space and, with sufficient data regularity, in the operator domain. A zero [eigenvalue](../../../../../../eigenvalue.md) would instead require its corresponding source coefficient to vanish and would leave an arbitrary homogeneous component.

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
