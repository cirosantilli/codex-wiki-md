<h1 id="7/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Multiply the equation for $y_n$ by $y_m$ and the equation for $y_m$ by $y_n$, then subtract. The common $h$ terms cancel, and [integration by parts](../../../../../integration-by-parts.md) gives the [Lagrange identity for a Sturm-Liouville operator](../../../../../lagrange-identity-for-a-sturm-liouville-operator.md):

$$
(\lambda_n-\lambda_m)\int_a^bw y_ny_m\,dx=\left[g(y_ny_m'-y_my_n')\right]_a^b.
$$

At each endpoint the two pairs $(y_n',y_n)$ and $(y_m',y_m)$ satisfy the same nontrivial homogeneous linear equation. They therefore lie on the same one-dimensional line, and their determinant vanishes. The boundary expression is zero. Since the [eigenvalues](../../../../../eigenvalue.md) are distinct, division gives the required [orthogonality of Sturm-Liouville eigenfunctions](../../../../../orthogonality-of-sturm-liouville-eigenfunctions.md):

$$
\boxed{\int_a^b w(x)y_n(x)y_m(x)\,dx=0.}
$$

For complex-valued eigenfunctions of a real self-adjoint problem one may choose real [eigenfunctions](../../../../../eigenfunction.md), or use the conjugated version as a [weighted inner product](../../../../../weighted-inner-product.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
