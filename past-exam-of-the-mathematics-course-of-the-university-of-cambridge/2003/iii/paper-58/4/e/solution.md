<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $\langle\Phi_{\mathbf k}\Phi_{\mathbf k'}^*\rangle=(2\pi)^3\delta^3(\mathbf k-\mathbf k')P_\Phi(k)$. Statistical isotropy and $\int|Y_{\ell m}|^2d\Omega=1$ applied to the preceding expression give the [CMB angular power spectrum](../../../../../../cosmic-microwave-background-power-spectrum.md)

$$
C_\ell=\frac{2}{9\pi}\int_0^\infty k^2P_\Phi(k)j_\ell(k\chi_*)^2\,dk.
$$

For $n=1$, define the constant dimensionless potential power $\mathcal A_\Phi=k^3P_\Phi(k)/(2\pi^2)$. Then

$$
C_\ell=\frac{4\pi\mathcal A_\Phi}{9}\int_0^\infty j_\ell(x)^2\frac{dx}{x}.
$$

The needed [logarithmic spherical Bessel square integral](../../../../../../logarithmic-spherical-bessel-square-integral.md) can be proved directly. Put $I_\ell=\int_0^\infty j_\ell^2\,dx/x$ and $J_\ell=\int_0^\infty j_\ell j_{\ell-1}\,dx$. From the [Spherical Bessel function](../../../../../../spherical-bessel-function.md) recurrences,

$$
j_\ell'=j_{\ell-1}-\frac{\ell+1}{x}j_\ell,\qquad
j_{\ell-1}'=\frac{\ell-1}{x}j_{\ell-1}-j_\ell,
$$

integration of the squares' derivatives gives $J_\ell=(\ell+1)I_\ell$, and for $\ell>1$ also $J_\ell=(\ell-1)I_{\ell-1}$. At $\ell=1$, $j_0(0)=1$ and $j_0(\infty)=0$ give $J_1=1/2$, hence $I_1=1/4$. Induction now proves $I_\ell=1/[2\ell(\ell+1)]$. Consequently

$$
\boxed{C_\ell=\frac{2\pi\mathcal A_\Phi}{9\ell(\ell+1)},\qquad
\ell(\ell+1)C_\ell=\frac{2\pi\mathcal A_\Phi}{9}\quad(\ell\geq2).}
$$

This is the flat large-angle [Sachs-Wolfe plateau](../../../../../../sachs-wolfe-plateau.md). The useful integral printed in the PDF is missing the square on $j_\ell$: without that square the formula is false, since at $\ell=1$ its left-hand side is $\pi/4$, whereas its asserted value would be $1/4$. The squared identity above is the one required by the variance calculation. The plateau describes the matter-era large-angle approximation, not acoustic peaks or late integrated-potential corrections.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
