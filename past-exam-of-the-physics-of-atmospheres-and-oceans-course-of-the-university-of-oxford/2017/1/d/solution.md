<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take a weak line in the radiative sense: the integrated slant [optical depth](../../../../optical-depth.md) is small wherever [absorption](../../../../absorption-electromagnetic-radiation.md) materially contributes, not merely a small greenhouse-gas [mass mixing ratio](../../../../mass-mixing-ratio.md). Normalize every local [spectral line profile](../../../../spectral-line-profile.md) so that $\int\kappa_\nu(p)\,d\nu=S$, with the [line strength](../../../../spectral-line-strength.md) independent of [pressure](../../../../pressure-split.md) and, as stipulated, [temperature](../../../../temperature-split.md). Keep a finite Doppler or natural core, or a [Voigt profile](../../../../voigt-profile.md), so that a pressure-only zero-width core at the top does not invalidate a uniform optical-depth expansion. The line must also be narrow enough to use $B_{\nu_0}$ across it.

To first order,

$$
E(p,q)\simeq\frac q{g\mu_d}\int_0^p\int\kappa_\nu(p')\,d\nu\,dp'
=\frac{qSp}{g\mu_d}.
$$

Thus the detailed normalized [line shape](../../../../spectral-line-profile.md) drops out, even if its width varies with [pressure](../../../../pressure-split.md). Substituting in the deficit in [c](../c.md) gives

$$
\boxed{\sigma_{\rm SB}T_s^4\simeq F_*+
\frac{\pi qSp_s}{g\mu_d}\left[B_{\nu_0}(T_s)-
\int_0^1B_{\nu_0}(T_s r^\kappa)\,dr\right].}
$$

The neglected term is second order when the relevant squared optical depths are integrable and uniformly small. A very narrow saturated line need not be weak simply because $q\ll1$. More generally the displayed first-order integrated limit follows from the finite integrated [opacity](../../../../opacity.md) even if an idealized [line centre](../../../../spectral-line.md) makes a pointwise expansion nonuniform; a finite physical core is the straightforward sufficient assumption.

For an explicitly perturbative [temperature](../../../../temperature-split.md) estimate, evaluate the bracket at $T_{\rm bare}$:

$$
\boxed{T_s-T_{\rm bare}\simeq\frac{\pi qSp_s}{4g\mu_d\sigma_{\rm SB}T_{\rm bare}^3}
\left[B_{\nu_0}(T_{\rm bare})-\int_0^1B_{\nu_0}(T_{\rm bare}r^\kappa)\,dr\right]>0.}
$$

At fixed $p_s,g,q,S$ and radiative conditions, increasing $\kappa=R_b/c_{p,b}$ makes every level $0<r<1$ cooler relative to the surface, enlarging the bracket and the warming. Increasing $c_{p,b}$ at fixed $R_b$ has the opposite effect. The limit $\kappa\to0$ is [isothermal](../../../../isothermal-process.md) and gives zero line-induced deficit. A change of background [molecular mass](../../../../molecular-mass.md) alone need not change this leading result: for [ideal gases](../../../../ideal-gas-split.md) with the same active [degrees of freedom](../../../../degree-of-freedom.md), $R_b$ and $c_{p,b}$ scale together and their ratio is unchanged. Comparing only the height-coordinate lapse rate $g/c_{p,b}$ would miss that the absorber column is naturally a pressure-coordinate quantity.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
