<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $\rho_g(r)$ be the gas density and $M(<r)$ the total gravitating mass. For a spherically symmetric gas in [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md), radial force balance is

$$
\frac{dP}{dr}=-\rho_g\frac{GM(<r)}{r^2}.
$$

Using the [ideal gas law](../../../../../../ideal-gas-law.md) $P=\rho_gk_BT/(\mu m_p)$, with constant [mean molecular weight](../../../../../../mean-molecular-weight.md) $\mu$, differentiate the product rather than setting $T$ constant:

$$
\frac{dP}{dr}=\frac{k_BT\rho_g}{\mu m_pr}
\left(\frac{d\log\rho_g}{d\log r}+\frac{d\log T}{d\log r}\right).
$$

Substitution and cancellation of $\rho_g$ give the [cluster hydrostatic mass estimator](../../../../../../cluster-hydrostatic-mass-estimator.md)

$$
\boxed{M(<r)=-\frac{k_BT(r)r}{\mu m_pG}
\left[\frac{d\log\rho_g}{d\log r}+\frac{d\log T}{d\log r}\right].}
$$

Here $k_B$ is the [Boltzmann constant](../../../../../../boltzmann-constant.md), denoted $K$ in the question. The prefactor has units of mass; a pressure decreasing outward makes the bracket negative and the inferred mass positive. For an isothermal gas with $\rho_g\propto r^{-\beta}$, this reduces to $M(<r)=\beta k_BTr/(\mu m_pG)$. The density in the logarithmic derivative is the gas density, not the total density. A varying $\mu$ or nonthermal pressure would require the corresponding extra terms.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
