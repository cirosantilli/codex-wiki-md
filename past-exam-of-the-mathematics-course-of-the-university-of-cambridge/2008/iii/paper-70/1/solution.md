<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Introduce the characteristic scales

$$
\rho_* =\frac{M}{4\pi R^3},\qquad
P_* =\frac{GM^2}{4\pi R^4},\qquad
T_* =\frac{\mu GM}{\mathcal R R}.
$$

Then $\rho=\rho_*b$, $P=P_*p$ and $T=T_*t$. The gas-only [equation of state](../../../../../equation-of-state.md) gives the important dimensionless identity **$p=bt$**. The PDF's [CNO cycle](../../../../../cno-cycle.md) approximation has temperature power 13; the converted TeX's power 1.3 is an OCR error.

Since $d/dr=R^{-1}d/dx$, the mass and [hydrostatic pressure support equation](../../../../../hydrostatic-pressure-support-equation.md) immediately become

$$
\frac MR\frac{dq}{dx}=4\pi R^2x^2\rho_*b,
\qquad
\frac{P_*}R\frac{dp}{dx}=-\frac{GM\rho_*bq}{R^2x^2}.
$$

Thus $dq/dx=x^2b$ and $dp/dx=-bq/x^2$. The [stellar structure equations](../../../../../stellar-structure-equations.md) for nuclear heating give

$$
\frac LR\frac{dl}{dx}
=4\pi R^2x^2\epsilon_0\rho_*^2b^2T_*^{13}t^{13},
$$

so

$$
\frac{dl}{dx}=E x^2b^2t^{13},\qquad
E=\frac{4\pi R^3\epsilon_0\rho_*^2T_*^{13}}L
=\frac{\epsilon_0M^{15}}{4\pi LR^{16}}
\left(\frac{\mu G}{\mathcal R}\right)^{13}.
$$

For [radiative diffusion in a star](../../../../../radiative-diffusion-in-a-star.md), $\kappa\rho=\kappa_0\rho^2T^{-3}$, and therefore

$$
\frac{T_*}R\frac{dt}{dx}
=-\frac{3\kappa_0\rho_*^2L}{16\pi acR^2T_*^6}
\frac{b^2l}{x^2t^6}.
$$

This gives the radiative gradient coefficient

$$
D=\frac{3\kappa_0\rho_*^2L}{16\pi acRT_*^7}
=\frac{3\kappa_0L}{256\pi^3acM^5}
\left(\frac{\mathcal R}{\mu G}\right)^7.
$$

In an efficiently convective region, the monatomic [adiabatic temperature gradient](../../../../../adiabatic-temperature-gradient.md) is $2/5$. Hence $dt/dx=(2/5)(t/p)(dp/dx)=-2q/(5x^2)$. If the radiative gradient is shallower, radiation suffices; if it is steeper than the adiabatic gradient, the [Schwarzschild criterion](../../../../../schwarzschild-criterion.md) selects convection and the shallower adiabatic profile. Thus

$$
\boxed{\frac{dq}{dx}=x^2b,\quad
\frac{dp}{dx}=-\frac{bq}{x^2},\quad
\frac{dt}{dx}=-\min\!\left(\frac{2q}{5x^2},\frac{Db^2l}{x^2t^6}\right),\quad
\frac{dl}{dx}=Ex^2b^2t^{13},\quad p=bt.}
$$

The regular central conditions are $q(0)=l(0)=0$ with finite positive $p(0),t(0)$. In particular $q\sim b(0)x^3/3$ and $l\sim E b(0)^2t(0)^{13}x^3/3$, so the pressure and temperature derivatives tend to zero at the centre. The normalized surface has $q(1)=l(1)=1$. In the idealized zero-pressure, zero-temperature surface used for [stellar homology](../../../../../stellar-homology.md), $p(1)=t(1)=0$; a physical photosphere supplies small nonzero surface values that are neglected in these bulk homology relations.

The common dimensionless profiles and boundary conditions keep $D,E$ constant. With fixed $\kappa_0,\epsilon_0$, $D$ constant yields $L\mu^{-7}M^{-5}=\mathrm{constant}$. Substitution into the nuclear coefficient then gives $R^{16}\propto\mu^6M^{10}$. Consequently the [CNO homology with density-dependent inverse-cubic opacity](../../../../../cno-homology-with-density-dependent-inverse-cubic-opacity.md) is

$$
\boxed{L\propto\mu^7M^5,\qquad R\propto\mu^{3/8}M^{5/8}.}
$$

The [Stefan–Boltzmann law](../../../../../stefan-boltzmann-law.md) gives $T_e^4\propto L/R^2\propto\mu^{25/4}M^{15/4}$. Eliminating mass, rather than dropping composition dependence, gives the [Hertzsprung-Russell diagram](../../../../../hertzsprung-russell-diagram.md) relation

$$
\boxed{L\propto\mu^{-4/3}T_e^{16/3},\qquad
\log L=\frac{16}{3}\log T_e-\frac43\log\mu+\mathrm{constant}.}
$$

The additive constant depends on the fixed physical and structural coefficients; logarithms refer to fixed choices of units.

For physical evolution time $s$, distinct from the dimensionless temperature $t(x)$, hold stellar mass fixed and put $u=3+5X$, $u_0=3+5X_0$. The [mean molecular weight](../../../../../mean-molecular-weight.md) approximation and the homology relation give $L=L_0(u_0/u)^7$. Converting hydrogen mass to helium releases energy at rate $L$, so fuel conservation is $ME_H\,dX/ds=-L$. Therefore

$$
\frac{du}{ds}=-\frac{5L_0u_0^7}{ME_Hu^7},\qquad
\frac d{ds}(u^8)=-\frac{40L_0u_0^7}{ME_H}.
$$

Integration with the initial composition proves the [homogeneous fuel-depletion luminosity feedback](../../../../../homogeneous-fuel-depletion-luminosity-feedback.md) law

$$
\boxed{L(s)=L_0\left(1-\frac{40L_0s}{ME_H(3+5X_0)}\right)^{-7/8}.}
$$

It is valid while hydrogen remains and the homology assumptions hold. Fuel exhaustion occurs when $u=3$, before the formal denominator vanishes; the apparent infinite luminosity is not a physical endpoint of this stellar model.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
