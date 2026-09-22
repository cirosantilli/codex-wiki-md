<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Differentiate the position vector with respect to the three coordinates:

$$
\begin{aligned}
\mathbf r_\rho&=(\sinh\rho\cos u\cos v,\sinh\rho\cos u\sin v,\cosh\rho\sin u),\\
\mathbf r_u&=(-\cosh\rho\sin u\cos v,-\cosh\rho\sin u\sin v,\sinh\rho\cos u),\\
\mathbf r_v&=(-\cosh\rho\cos u\sin v,\cosh\rho\cos u\cos v,0).
\end{aligned}
$$

Their pairwise [dot products](../../../../../dot-product.md) vanish. For example, $\mathbf r_\rho\cdot\mathbf r_u=-\sinh\rho\cosh\rho\sin u\cos u+\sinh\rho\cosh\rho\sin u\cos u=0$. Thus these are [orthogonal coordinates](../../../../../orthogonal-coordinates.md) wherever the coordinate tangents are nonzero. Their [scale factors of orthogonal coordinates](../../../../../scale-factors-of-orthogonal-coordinates.md) are

$$
h_\rho^2=h_u^2=\sinh^2\rho\cos^2u+\cosh^2\rho\sin^2u=\sinh^2\rho+\sin^2u,\qquad h_v=\cosh\rho\cos u.
$$

The absolute [Jacobian determinant](../../../../../jacobian-determinant.md) is their product, giving

$$
\boxed{dV=\cosh\rho\cos u(\sinh^2\rho+\sin^2u)\,d\rho\,du\,dv.}
$$

The ordered coordinate system is left handed: $\mathbf r_\rho\cdot(\mathbf r_u\times\mathbf r_v)=-h_\rho h_uh_v$. The volume measure uses the absolute value. The axis and the focal circle contain coordinate degeneracies, as expected for [oblate spheroidal coordinates](../../../../../oblate-spheroidal-coordinates.md). This is the [hyperbolic parametrization of oblate spheroidal coordinates](../../../../../hyperbolic-parametrization-of-oblate-spheroidal-coordinates.md). The local TeX has an OCR substitution $\sinh^2u$ in the volume formula; the original PDF correctly prints $\sin^2u$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
