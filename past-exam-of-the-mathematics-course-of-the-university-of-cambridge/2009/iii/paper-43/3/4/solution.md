<h1 id="3/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Split the Fourier modes into $|p|<\Lambda/b$ and the shell $\Lambda/b<|p|<\Lambda$. The source is uniform, so it couples only to the zero mode, which belongs to the retained part. The [Gaussian field theory](../../../../../../gaussian-field-theory.md) has no couplings between the shell and retained modes. Integrating out the shell therefore contributes only a source-independent determinant to the [free energy](../../../../../../thermodynamic-free-energy.md), without changing the quadratic coefficients of the retained Hamiltonian.

Restore the cutoff by $x=bx'$ and choose the field normalization $\phi_<(bx')=b^{-(D-2)/2}\phi'(x')$. Counting the measure, derivative and field factors explicitly gives

$$
\int d^Dx\,\frac1{2\alpha}|\nabla\phi_<|^2
=\int d^Dx'\,\frac1{2\alpha}|\nabla'\phi'|^2,
$$



$$
\int d^Dx\,\frac{m^2}{2}\phi_<^2
=\int d^Dx'\,\frac{b^2m^2}{2}\phi'^2,\qquad
\int d^Dx\,h\phi_<
=\int d^Dx'\,b^{(D+2)/2}h\phi'.
$$

Thus in the convention that preserves the kinetic normalization, the [Gaussian momentum-shell scaling](../../../../../../gaussian-momentum-shell-scaling.md) is

$$
\boxed{\alpha'=\alpha,\qquad (m^2)'=b^2m^2,\qquad h'=b^{(D+2)/2}h.}
$$

The field has [engineering dimension](../../../../../../engineering-dimension.md) $(D-2)/2$ and zero [anomalous dimension](../../../../../../anomalous-dimension.md). The measure Jacobian and shell determinant supply the additive constant described in Q2. A different choice of field rescaling can redistribute factors into $\alpha$, but must give the same physical transformed [correlation length](../../../../../../correlation-length.md) $\xi'=\xi/b$.

## ↑ Ancestors (11)

1. [4](../4.md)
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
