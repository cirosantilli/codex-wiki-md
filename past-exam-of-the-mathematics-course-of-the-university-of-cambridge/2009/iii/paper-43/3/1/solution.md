<h1 id="3/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Measure the [statistical Hamiltonian](../../../../../../statistical-hamiltonian.md) in units of $k_BT$ so that the weight is $e^{-H_0}$, and take $\alpha>0$, $m^2>0$ for convergence. Use the [Fourier transform](../../../../../../fourier-transform.md) convention

$$
\phi(x)=\int_p e^{ip\cdot x}\widetilde\phi(p),\qquad
\int_p=\int\frac{d^Dp}{(2\pi)^D},\qquad
\widetilde\phi(-p)=\widetilde\phi(p)^*.
$$

The last identity is the reality condition, so modes at $p$ and $-p$ are not independent complex fields. Orthogonality of the Fourier exponentials gives $\int d^Dx\,\phi^2=\int_p|\widetilde\phi(p)|^2$, while a derivative multiplies a Fourier mode by $ip$. Hence

$$
\boxed{H_0=\frac12\int_p\widetilde\phi(p)\widetilde\Delta(p)\widetilde\phi(p)^*,\qquad
\widetilde\Delta(p)=\alpha^{-1}p^2+m^2.}
$$

The kernel is positive for the stated parameters. Keeping an explicit inverse temperature instead would replace this kernel in the statistical weight by $\beta_{\rm th}\widetilde\Delta$; the following source convention absorbs that factor.

## ↑ Ancestors (11)

1. [1](../1.md)
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
