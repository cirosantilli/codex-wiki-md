<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [stellar homology](../../../../../../stellar-homology.md): dimensionless profiles and composition are fixed, so proportionality constants do not change along the model sequence. Scaling mass conservation and the [stellar hydrostatic equation](../../../../../../hydrostatic-pressure-support-equation.md) gives

$$
\rho_*\propto\frac M{R^3},\qquad P_*\propto\frac{GM^2}{R^4},\qquad
T_*\propto\frac{P_*}{\rho_*}\propto\frac MR,
$$

where the last relation uses the [ideal gas](../../../../../../ideal-gas.md) equation of state with fixed [mean molecular weight](../../../../../../mean-molecular-weight.md). The specific [stellar energy-generation rate](../../../../../../stellar-energy-generation-rate.md) is $\epsilon\propto\rho T^\eta$, so

$$
L_{\rm nuc}\sim M\epsilon_*\propto M^{\eta+2}R^{-(\eta+3)}.
$$

By [stellar radiative diffusion](../../../../../../radiative-diffusion-in-a-star.md), $T_*/R\sim\kappa_*\rho_*L/R^2T_*^3$, hence

$$
L_{\rm rad}\propto\frac{RT_*^4}{\kappa_*\rho_*}
\propto M^{3-\lambda-\nu}R^{3\lambda+\nu}.
$$

Equate the generated and transported [luminosity](../../../../../../luminosity.md) in thermal equilibrium. The [homology relations for radiative stars](../../../../../../homology-relations-for-radiative-stars.md) give

$$
R^{3+\eta+\nu+3\lambda}\propto M^{\eta+\nu+\lambda-1},\qquad
\boxed{R\propto M^X,\quad
X=\frac{\eta+\nu+\lambda-1}{3+\eta+\nu+3\lambda}.}
$$

This division presumes a nonzero denominator. If it vanishes, the scaling balance instead imposes a condition on $M$ or leaves the radius scaling undetermined, depending on the numerator. For later use, the corresponding [mass-luminosity relation](../../../../../../mass-luminosity-relation.md) exponent is

$$
Y=\eta+2-(\eta+3)X
=3-\lambda-\nu+(3\lambda+\nu)X.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 317](../../../paper-317-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
