<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the ordinary real [inner product](../../../../../inner-product-split.md) $\langle u,v\rangle=\int_a^buv\,dx$ on the domain of functions obeying the two separated boundary conditions. [Integration by parts](../../../../../integration-by-parts.md) gives the [Lagrange identity for a Sturm-Liouville operator](../../../../../lagrange-identity-for-a-sturm-liouville-operator.md)

$$
\langle u,Lv\rangle-\langle Lu,v\rangle=\big[p(vu'-uv')\big]_a^b.
$$

At $a$, the two boundary-value vectors $(u(a),u'(a))$ and $(v(a),v'(a))$ satisfy the same homogeneous linear relation. If $A_2=0$, both function values vanish; if $A_2\ne0$, their derivatives are the same constant multiple $-A_1/A_2$ of their values. Either way $vu'-uv'=0$. The same argument applies at $b$. Hence

$$
\boxed{\langle u,Lv\rangle=\langle Lu,v\rangle.}
$$

This proves symmetry, and the regular separated [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md) has the same adjoint domain, so $L$ is [self-adjoint](../../../../../self-adjoint-operator.md). To see the domain point, require the boundary form to vanish against every admissible $u$: the independently variable endpoint data force an adjoint-domain function to obey those same endpoint relations.

As usual, each endpoint pair $(A_1,A_2)$ and $(B_1,B_2)$ must be nonzero, and the coefficients must have the regularity needed for these operations. An identically zero pair would impose no condition at that endpoint and would not give the claimed [self-adjoint operator](../../../../../self-adjoint-operator.md). The related operator $\omega^{-1}L$ is self-adjoint in the [weighted inner product](../../../../../weighted-inner-product.md) $\int_a^b\omega uv\,dx$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
