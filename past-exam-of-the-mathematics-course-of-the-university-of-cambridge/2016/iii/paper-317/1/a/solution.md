<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\mathcal R=k/(\mu m_H)$ for the specific gas constant, with the printed $m_H$ denoting the atomic mass unit, and $a_{\rm r}=4\sigma/c$ for the [radiation constant](../../../../../../radiation-constant.md). In the low-mass envelope the [enclosed mass](../../../../../../enclosed-mass.md) is approximately $M$ and the outward [luminosity](../../../../../../luminosity.md) is approximately $L$. The [stellar hydrostatic equation](../../../../../../hydrostatic-pressure-support-equation.md), [stellar radiative diffusion](../../../../../../radiative-diffusion-in-a-star.md), and [ideal gas](../../../../../../ideal-gas.md) equation give

$$
\frac{dP}{dr}=-\frac{GM\rho}{r^2},\qquad
\frac{dT}{dr}=-\frac{3\kappa\rho L}{16\pi a_{\rm r}c r^2T^3},\qquad
P=\mathcal R\rho T.
$$

The [Kramers' opacity law](../../../../../../kramers-opacity-law.md) becomes $\kappa=(\kappa_0/\mathcal R)PT^{-9/2}$. Dividing the two differential equations eliminates radius and [mass density](../../../../../../density.md):

$$
P\frac{dP}{dT}=\frac{16\pi a_{\rm r}cGM\mathcal R}{3\kappa_0L}T^{15/2}.
$$

Integrating from a surface matching point $(P_s,T_s)$ gives

$$
P^2=P_s^2+\frac{64\pi a_{\rm r}cGM\mathcal R}{51\kappa_0L}
\left(T^{17/2}-T_s^{17/2}\right).
$$

Deep compared with the [photosphere](../../../../../../photosphere.md), the surface terms are negligible. The [radiative-zero white-dwarf envelope](../../../../../../radiative-zero-white-dwarf-envelope.md) therefore has

$$
\boxed{P(T)=\left(\frac{64\pi a_{\rm r}cGM\mathcal R}{51\kappa_0L}\right)^{1/2}T^{17/4},\qquad
\rho\propto T^{13/4}.}
$$

This is the leading envelope approximation used in the later parts, rather than an exact atmospheric boundary condition at $T_{\rm eff}$.

At the base, [temperature](../../../../../../temperature.md), [mass density](../../../../../../density.md) and [pressure](../../../../../../pressure.md) match the isothermal degenerate core. Let $K_{\rm NR}=K_1\mu_e^{-5/3}$, where $\mu_e$ is the [mean molecular weight per electron](../../../../../../mean-molecular-weight-per-electron.md). Equating the gas and [electron degeneracy pressure](../../../../../../electron-degeneracy-pressure.md) gives

$$
\mathcal R\rho_bT_c=K_{\rm NR}\rho_b^{5/3},\qquad
\boxed{\rho_b=\left(\frac{\mathcal RT_c}{K_{\rm NR}}\right)^{3/2}
=\mu_e^{5/2}\left(\frac{\mathcal R}{K_1}\right)^{3/2}T_c^{3/2}.}
$$

Hence $P_b=\mu_e^{5/2}\mathcal R^{5/2}K_1^{-3/2}T_c^{5/2}$. Substituting this into the envelope relation at $T=T_c$ yields

$$
\boxed{\frac LM=\frac{64\pi a_{\rm r}cG}{51\kappa_0}
\frac{K_1^3}{\mu_e^5\mathcal R^4}T_c^{7/2}
=\frac{256\pi\sigma G}{51\kappa_0}\frac{K_1^3}{\mu_e^5}
\left(\frac{\mu m_H}{k}\right)^4T_c^{7/2}.}
$$

The [matching of a white-dwarf envelope to a degenerate core](../../../../../../matching-of-a-white-dwarf-envelope-to-a-degenerate-core.md) thus gives **$L/M\propto T_c^{7/2}$**, the envelope relation underlying [Mestel's cooling law](../../../../../../mestel-s-cooling-law.md). It depends on [pressure](../../../../../../pressure.md) as well as [mass density](../../../../../../density.md) continuity at the interface; otherwise the supplied core equation would not determine the matching [mass density](../../../../../../density.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 317](../../../paper-317-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
