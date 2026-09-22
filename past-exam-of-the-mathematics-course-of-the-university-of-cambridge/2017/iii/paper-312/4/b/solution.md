<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $R=\Delta\tau>0$, $L=\ell_1+\ell_2+\ell_3$ and $D=\prod_{r=1}^3(2\ell_r+1)$. Use exactly the given [constant primordial bispectrum](../../../../../../constant-primordial-bispectrum.md) normalization, without an additional local-template convention factor. Combining it with the large-angle [Sachs-Wolfe effect](../../../../../../sachs-wolfe-effect.md) [cosmological transfer function](../../../../../../cosmological-transfer-function.md) gives the [reduced CMB bispectrum](../../../../../../reduced-cmb-bispectrum.md)

$$
b_{\ell_1\ell_2\ell_3}=\left(\frac2\pi\right)^3\frac{4\pi^4f_{\rm NL}\Delta_\zeta^4}{125}\int_0^\infty x^2\,dx\prod_{r=1}^3I_{\ell_r}(x,R),
$$

where $I_\ell(x,R)=\int_0^\infty j_\ell(kR)j_\ell(kx)\,dk$. Each $1/5$ transfer factor has been retained; their product is $1/125$.

Apply the supplied [spherical Bessel product integral](../../../../../../spherical-bessel-product-integral.md) after rescaling $q=kR$:

$$
I_\ell(x,R)=\frac{\pi}{2R(2\ell+1)}\begin{cases}(x/R)^\ell,&0<x<R,\\(x/R)^{-\ell-1},&x>R.\end{cases}
$$

The two branches agree at $x=R$. In the radial integral put $r=x/R$. The factor $R^3$ from $x^2dx$ cancels the $R^{-3}$ from the three kernels. The remaining integral is

$$
\int_0^\infty x^2\prod_r I_{\ell_r}(x,R)\,dx=\frac{\pi^3}{8D}\left[\int_0^1r^{L+2}\,dr+\int_1^\infty r^{-L-1}\,dr\right]=\frac{\pi^3}{8D}\left(\frac1{L+3}+\frac1L\right),
$$

provided $L>0$. This evaluation uses the momentum integrals at fixed radial parameter in the projection, then the radial integral; it does not require an unjustified global exchange of all oscillatory integrals.

The factors $(2/\pi)^3$ and $\pi^3/8$ cancel exactly. Hence the [Sachs-Wolfe projection of a constant bispectrum](../../../../../../sachs-wolfe-projection-of-a-constant-bispectrum.md) is

$$
\boxed{b_{\ell_1\ell_2\ell_3}=\frac{4\pi^4f_{\rm NL}\Delta_\zeta^4}{125(2\ell_1+1)(2\ell_2+1)(2\ell_3+1)}\left[\frac1{\ell_1+\ell_2+\ell_3+3}+\frac1{\ell_1+\ell_2+\ell_3}\right],\qquad \mathcal A=\frac{4\pi^4\Delta_\zeta^4}{125}.}
$$

The all-monopole case $L=0$ has a logarithmically divergent outer radial integral and is not covered by the printed finite formula. Observable CMB analyses remove the monopole and dipole, normally using $\ell_i\geq2$, so this issue is absent there. Angular triangle and parity selection are carried by the triple-[spherical harmonic](../../../../../../spherical-harmonic.md) geometric factor multiplying the reduced bispectrum.

There is no dependence on the last-scattering distance $R$, and no extra physical scale appears when $\Delta_\zeta^2$ is held constant. At fixed triangle shape and in the range $1\ll\ell_i\ll200$, common rescaling of all multipoles gives

$$
\boxed{b_{\lambda\ell_1,\lambda\ell_2,\lambda\ell_3}\sim\lambda^{-4}b_{\ell_1,\ell_2,\ell_3}.}
$$

This is angular scale invariance in the usual weighted sense; a constant primordial shape does not make the unweighted [reduced CMB bispectrum](../../../../../../reduced-cmb-bispectrum.md) independent of angular scale. The exact finite-multipole expression retains the $+1$ and $+3$ terms shown above.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
