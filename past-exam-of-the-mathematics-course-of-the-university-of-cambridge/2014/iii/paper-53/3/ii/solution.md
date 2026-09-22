<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Insert the [primordial bispectrum](../../../../../../primordial-bispectrum.md) into the product of the three linear transfer integrals. Write $L=\ell_1+\ell_2+\ell_3$ and abbreviate $g_{\ell_i}(\eta_0,k_i)$ by $g_i$. The observer-position phase is one because the momentum delta function imposes $\sum\boldsymbol k_i=0$. Represent that delta function by

$$
(2\pi)^3\delta^{(3)}(\boldsymbol k_1+\boldsymbol k_2+\boldsymbol k_3)
=\int d^3x\,e^{i(\boldsymbol k_1+\boldsymbol k_2+\boldsymbol k_3)\cdot\boldsymbol x}.
$$

The [Rayleigh plane-wave expansion](../../../../../../rayleigh-plane-wave-expansion.md) and angular orthogonality give, for each momentum,

$$
\int d\hat k\,Y_{\ell m}^*(\hat k)e^{i\boldsymbol k\cdot\boldsymbol x}
=4\pi i^\ell j_\ell(kx)Y_{\ell m}^*(\hat x).
$$

The three $i^\ell$ factors cancel the $(-i)^L$ in the temperature multipoles. Angular integration over $\hat x$ leaves the complex conjugate [Gaunt integral](../../../../../../gaunt-integral.md). In the conventional complex [spherical harmonics](../../../../../../spherical-harmonic.md), this integral is real, and it vanishes unless the angular momentum triangle, even-parity and $m_1+m_2+m_3=0$ selection rules hold. Therefore its conjugate equals itself.

The radial measure is $x^2dx$, and the momentum radial measures are $k_i^2dk_i$. The combined numerical prefactor is $(4\pi)^6/(2\pi)^9=8/\pi^3=64/(2\pi)^3$. Hence the [reduced CMB bispectrum](../../../../../../reduced-cmb-bispectrum.md) is

$$
\boxed{b_{\ell_1\ell_2\ell_3}=\left(\frac2\pi\right)^3
\int_0^\infty x^2dx\int_0^\infty\prod_{i=1}^3
\left[k_i^2dk_i\,j_{\ell_i}(k_ix)g_{\ell_i}(\eta_0,k_i)\right]B(k_1,k_2,k_3),}
$$

and the angular three-point function factorizes as

$$
\boxed{\langle\Theta_{\ell_1m_1}\Theta_{\ell_2m_2}\Theta_{\ell_3m_3}\rangle
=b_{\ell_1\ell_2\ell_3}\mathcal G^{\ell_1\ell_2\ell_3}_{m_1m_2m_3}.}
$$

This [primordial-to-angular bispectrum projection](../../../../../../primordial-to-angular-bispectrum-projection.md) separates dynamics and radial transfer from purely angular geometry. The spatial integration variable is auxiliary, not the observer position. Linear transfer is justified at leading order in the primordial signal; it does not require a large amplitude mathematically, although a signal must exceed measurement uncertainty to be detectable.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
