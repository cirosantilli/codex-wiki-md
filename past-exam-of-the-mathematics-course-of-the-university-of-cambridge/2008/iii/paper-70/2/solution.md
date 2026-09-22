<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $\Omega=-\int_0^M Gm\,dm/r$ be the [gravitational energy](../../../../../gravitational-energy.md). Multiply the [stellar hydrostatic equation](../../../../../hydrostatic-pressure-support-equation.md) by $4\pi r^3$ and integrate through the star. Integration by parts and zero surface pressure give

$$
\int_0^R4\pi r^3\frac{dP}{dr}dr
=-3\int_0^R4\pi r^2Pdr
=-3\int_0^M\frac P\rho dm,
$$

while its hydrostatic right-hand side is $-\int_0^R4\pi Gmr\rho\,dr=\Omega$. Hence the [stellar virial theorem](../../../../../stellar-virial-theorem.md) is

$$
\boxed{3\int_0^M\frac P\rho dm+\Omega=0.}
$$

There is a genuine reference-sheet error to resolve. A monatomic [ideal gas](../../../../../ideal-gas.md) with adiabatic exponent $5/3$ has specific [internal energy of an ideal gas](../../../../../internal-energy-of-an-ideal-gas.md) $u=P/[\rho(5/3-1)]=3P/(2\rho)$, not the printed $3P/\rho$ on PDF page 2. The latter would give total internal energy $-\Omega$ and zero total energy, inconsistent with radiating contraction. The following derivation uses the consistent monatomic value.

A [fully convective star](../../../../../fully-convective-star.md) is approximately isentropic and has an [adiabatic stellar polytrope](../../../../../adiabatic-stellar-polytrope.md) with index $3/2$. The given polytropic gravitational-energy formula yields $\Omega=-6GM^2/(7R)$. The virial relation gives total internal energy $U=-\Omega/2$, so total energy is $U+\Omega=-3GM^2/(7R)$. At constant mass with no nuclear heating, [Kelvin-Helmholtz contraction](../../../../../kelvin-helmholtz-mechanism.md) obeys $d(U+\Omega)/ds=-L$, whence

$$
\boxed{\frac{dR}{ds}=-\frac{7LR^2}{3GM^2}.}
$$

Here $s$ denotes physical time.

In the plane-parallel atmosphere, the inward [optical depth](../../../../../optical-depth.md) satisfies $d\tau=-\kappa\rho\,dr$, so [hydrostatic equilibrium in optical depth](../../../../../hydrostatic-equilibrium-in-optical-depth.md) gives $dP/d\tau=g/\kappa$. Neglecting radiation pressure, $\rho=\mu P/(\mathcal RT)$ and the specified opacity becomes $\kappa=(\kappa_0\mu/\mathcal R)PT^{16}$. Therefore

$$
\frac{d(P^2)}{d\tau}=\frac{2\mathcal Rg}{\mu\kappa_0T^{16}}
=\frac{512\mathcal Rg}{\mu\kappa_0T_e^{16}}(2+3\tau)^{-4}.
$$

The [grey atmosphere](../../../../../grey-atmosphere.md) relation and the boundary $P(0)=0$ integrate to

$$
\boxed{P^2=\frac{512\mathcal Rg}{9\mu\kappa_0T_e^{16}}
\left[\frac18-\frac1{(2+3\tau)^3}\right].}
$$

To apply the [Schwarzschild criterion](../../../../../schwarzschild-criterion.md), put $w=2+3\tau$. Logarithmic differentiation gives

$$
\frac{d\log T}{d\tau}=\frac3{4w},\qquad
\frac{d\log P}{d\tau}=\frac9{2w(w^3/8-1)},\qquad
\nabla_{\rm rad}=\frac{d\log T}{d\log P}=\frac{w^3-8}{48}.
$$

This increases inward, starting from zero. Marginal convection has $\nabla_{\rm rad}=2/5$, so $w_b^3=136/5$. Since $T_b^{12}/T_e^{12}=w_b^3/64$, the [grey-atmosphere convection onset with seventeenth-power opacity](../../../../../grey-atmosphere-convection-onset-with-seventeenth-power-opacity.md) is

$$
\boxed{T_b=\left(\frac{17}{40}\right)^{1/12}T_e.}
$$

The purely radiative atmosphere is used only up to this boundary.

The convective relation $P=KT^{5/2}$ is spatially uniform in its entropy coefficient $K$ at each instant; $K$ can change as the star radiates and contracts. At the convection boundary $w_b$ is a fixed number, so $P_b\propto g^{1/2}T_e^{-8}$ at fixed composition and opacity normalization. Thus

$$
K=\frac{P_b}{T_b^{5/2}}\propto g^{1/2}T_e^{-21/2}
\propto M^{1/2}R^{-1}T_e^{-21/2}.
$$

On the other hand, the central scalings for the $n=3/2$ [stellar polytrope](../../../../../stellar-polytrope.md) give $P_c\propto GM^2/R^4$ and $T_c=\mu P_c/(\mathcal R\rho_c)\propto\mu GM/(\mathcal RR)$. Hence, at fixed composition,

$$
K=\frac{P_c}{T_c^{5/2}}\propto M^{-1/2}R^{-3/2}.
$$

Equating the interior and atmosphere expressions yields $T_e^{21/2}\propto MR^{1/2}$. Applying the [Stefan–Boltzmann law](../../../../../stefan-boltzmann-law.md) then proves the [Hayashi contraction with seventeenth-power opacity](../../../../../hayashi-contraction-with-seventeenth-power-opacity.md) relation

$$
\boxed{L\propto M^{8/21}R^{46/21}.}
$$

At fixed mass write $L=A M^{8/21}R^\alpha$, with constant $A$ and $\alpha=46/21$. The contraction equation is $\dot R=-C R^{\alpha+2}$, where $C=7AM^{8/21}/(3GM^2)$. Direct integration gives

$$
R^{-(\alpha+1)}-R_0^{-(\alpha+1)}=(\alpha+1)Cs,
\qquad \alpha+1=\frac{67}{21}.
$$

Multiplying through by $R^{\alpha+1}$ and substituting the current luminosity gives

$$
L=\frac{9GM^2}{67Rs}\left[1-\left(\frac R{R_0}\right)^{67/21}\right].
$$

For the stated very large initial radius, or after that initial-radius term becomes negligible,

$$
\boxed{L=\frac{9GM^2}{67Rs}.}
$$

This is the luminosity-age relation within the contraction model, rather than an assertion that a physical star begins at literally infinite radius.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 70](../../paper-70-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
