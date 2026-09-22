<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

[Radiative diffusion in a star](../../../../../../radiative-diffusion-in-a-star.md) can be written

$$
\frac{dP_{\rm rad}}{dr}
=-\frac{\kappa\rho L_r}{4\pi cr^2}.
$$

Dividing by [hydrostatic equilibrium](../../../../../../hydrostatic-equilibrium.md) gives

$$
\frac{dP_{\rm rad}}{dP}
=\frac{\kappa L_r}{4\pi cGm_r}
=\frac{\nu L}{4\pi cGM},
$$

which is constant by assumption. Since both $P_{\rm rad}$ and $P$ vanish at the surface, integration gives $P_{\rm rad}=(1-\beta)P$ with constant $\beta$.

Eliminating $T$ between the gas and radiation equations of state now gives

$$
P=K\rho^{4/3},
\qquad
K=\left[\frac3a
\left(\frac{\mathcal R}{\mu}\right)^4
\frac{1-\beta}{\beta^4}\right]^{1/3}.
$$

Thus the star is an $n=3$ [stellar polytrope](../../../../../../stellar-polytrope.md). Put

$$
\rho=\rho_c\theta^3,
\qquad
r=\alpha\xi,
\qquad
\alpha^2=\frac K{\pi G}\rho_c^{-2/3}.
$$

The structure equations become the [Lane-Emden equation](../../../../../../lane-emden-equation.md)

$$
\boxed{\frac1{\xi^2}\frac d{d\xi}
\left(\xi^2\frac{d\theta}{d\xi}\right)=-\theta^3},
\qquad
\boxed{\theta(0)=1,\quad\theta'(0)=0}.
$$

The surface is the first zero $\xi_1\simeq6.89685$. Writing

$$
\omega_3=-\xi_1^2\theta'(\xi_1)\simeq2.01824,
$$

the [Lane-Emden mass formula](../../../../../../lane-emden-mass-formula.md) gives

$$
M=4\pi\alpha^3\rho_c\omega_3
=\frac{4\omega_3}{\sqrt\pi}
\left(\frac KG\right)^{3/2}.
$$

Therefore

$$
\boxed{M=\lambda\frac{(1-\beta)^{1/2}}{\beta^2}},
$$

where

$$
\boxed{\lambda=
\frac{4\omega_3}{\sqrt\pi}
\left(\frac3a\right)^{1/2}
\left(\frac{\mathcal R}{\mu}\right)^2G^{-3/2}}.
$$

The additional radiative-equilibrium relation is $1-\beta=\nu L/(4\pi cGM)$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 317](../../../paper-317-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
