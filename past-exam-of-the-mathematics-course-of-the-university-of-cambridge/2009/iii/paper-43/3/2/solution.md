<h1 id="3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Couple a real source through $H_J=H_0-\int d^Dx\,J(x)\phi(x)$. Its Fourier components obey $\widetilde J(-p)=\widetilde J(p)^*$, and the source term is $-\int_p\widetilde J(p)\widetilde\phi(p)^*$. Complete the square using the positive quadratic kernel from the previous part:

$$
H_J=\frac12\int_p\bigl(\widetilde\phi-\widetilde\Delta^{-1}\widetilde J\bigr)
\widetilde\Delta\bigl(\widetilde\phi-\widetilde\Delta^{-1}\widetilde J\bigr)^*
-\frac12\int_p\widetilde J\widetilde\Delta^{-1}\widetilde J^*.
$$

Translation of the integration variables in the regulated [Gaussian functional integral](../../../../../../gaussian-functional-integral.md) therefore gives

$$
\boxed{Z_0[J]=Z_G\exp\left[\frac12\int_p\frac{|\widetilde J(p)|^2}{\alpha^{-1}p^2+m^2}\right].}
$$

This also fixes the sign: a real linear source increases the Gaussian generating function by a positive quadratic exponent, unlike an imaginary Fourier-characteristic-function source.

To specify $Z_G$ rather than conceal an infinite normalization, first impose finite volume and an [ultraviolet cutoff](../../../../../../ultraviolet-cutoff.md), and choose orthonormal real coordinates for the independent field modes. If their number is $N_R$ and the eigenvalues of the quadratic form are $\Delta_j>0$, the measure $\prod_{j=1}^{N_R}d\phi_j$ gives

$$
\boxed{Z_G=\prod_{j=1}^{N_R}\left(\frac{2\pi}{\Delta_j}\right)^{1/2}
=(2\pi)^{N_R/2}(\det\Delta)^{-1/2}.}
$$

A measure $\prod_jd\phi_j/\sqrt{2\pi}$ removes the prefactor. In the continuum one may express this as $\log Z_G=-\tfrac12\operatorname{Tr}\log\Delta$ plus a source-independent measure constant, with the same regulator understood. The real-mode prescription prevents double counting the conjugate Fourier pairs. All normalized [correlation functions](../../../../../../correlation-function.md) follow from $Z_0[J]/Z_G$ and do not depend on that constant.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [3](../../3.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
