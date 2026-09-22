<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Change independent variable from [proper time](../../../../../../proper-time.md) to the [scale factor](../../../../../../scale-factor-cosmology.md). Then $\dot\delta=\dot a\delta_a$ and $\ddot\delta=\dot a^2\delta_{aa}+\ddot a\delta_a$. Under [radiation domination](../../../../../../radiation-domination.md), $\ddot a=-\dot a^2/a$ and $H^2\simeq8\pi G\bar\rho_r/3$. Since $\bar\rho_m/\bar\rho_r=a/a_{\rm eq}$, the [linear matter perturbation growth equation](../../../../../../linear-matter-perturbation-growth-equation.md) becomes

$$
\delta_{aa}+\frac1a\delta_a-\frac{3}{2aa_{\rm eq}}\delta=0.
$$

Putting $\delta=au$ gives

$$
\boxed{u_{aa}+\frac3a u_a+\frac1{a^2}\left(1-\frac32\frac a{a_{\rm eq}}\right)u=0}.
$$

This keeps the matter self-gravity term in a radiation-dominated background. It is not an exact background equation through radiation-matter equality.

At $a/a_{\rm eq}\ll1$, neglecting that small term gives $\delta_{aa}+\delta_a/a=0$. Integration yields

$$
\boxed{\delta_m=C_1+C_2\ln(a/a_*),\qquad u=[C_1+C_2\ln(a/a_*)]/a}.
$$

Thus matter has at most logarithmic growth during this leading radiation approximation, together with a constant independent mode. The constant is non-growing, not a mode that literally falls as $a^{-1}$; that power belongs to $u$ rather than $\delta_m$.

For an increasing/decreasing basis of the displayed equation with matter self-gravity retained, put $x=\sqrt{6a/a_{\rm eq}}$. Its equation becomes $x^2\delta_{xx}+x\delta_x-x^2\delta=0$. Hence

$$
\boxed{\delta_+=I_0(x),\qquad\delta_-=K_0(x)}.
$$

The [Modified Bessel function of the first kind](../../../../../../modified-bessel-function-of-the-first-kind.md) gives $I_0(x)=1+3a/(2a_{\rm eq})+O((a/a_{\rm eq})^2)$, which increases slowly. The [Modified Bessel function of the second kind](../../../../../../modified-bessel-function-of-the-second-kind.md) gives $K_0(x)=-\tfrac12\ln(a/a_{\rm eq})+\tfrac12\ln(2/3)-\gamma_E+O((a/a_{\rm eq})|\ln(a/a_{\rm eq})|)$, where $\gamma_E$ is [Euler's constant](../../../../../../euler-s-constant.md); this mode decreases as $a$ increases. Their leading span is precisely the constant/logarithmic pair above. Mode labels depend on the chosen basis and normalization; no rapid matter-era growth $\delta\propto a$ occurs here. Neglected background corrections can change subleading terms, so the Bessel basis should not be extrapolated through equality.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
