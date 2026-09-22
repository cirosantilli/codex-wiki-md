<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [radiative homology with proton-proton burning and inverse-fourth-power opacity](../../../../../radiative-homology-with-proton-proton-burning-and-inverse-fourth-power-opacity.md), retaining the composition factors throughout. To distinguish the stellar [radius](../../../../../radius.md) from the [stellar gas constant](../../../../../stellar-gas-constant.md), write them as $R$ and $\mathcal R$. With [gas pressure](../../../../../gas-pressure.md) alone, introduce the scale factors

$$
\rho_* =\frac{M}{4\pi R^3},\qquad P_* =\frac{GM^2}{4\pi R^4},\qquad T_* =\frac{\mu GM}{\mathcal RR}.
$$

The [ideal gas](../../../../../ideal-gas.md) equation gives $\rho=\rho_*b$, $P=P_*p$ and $T=T_*p/b$. Substitution into [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) and [mass conservation](../../../../../mass-conservation.md) gives

$$
\frac{P_*}{R}\frac{dp}{dx}=-\frac{GM\rho_*}{R^2}\frac{qb}{x^2},\qquad \frac{M}{R}\frac{dq}{dx}=4\pi R^2\rho_*x^2b,
$$

so **$p'=-bq/x^2$ and $q'=x^2b$**.

Set $\zeta=Z(1+X)$. The [radiative diffusion in a star](../../../../../radiative-diffusion-in-a-star.md) equation, with the stipulated [opacity](../../../../../opacity.md), becomes

$$
\frac{T_*}{R}\frac{d}{dx}\left(\frac pb\right)=-\frac{3\kappa_0\zeta\rho_*^2L}{16\pi acR^2T_*^7}\frac{b^9l}{x^2p^7}.
$$

Here $\rho^2T^{-7}=\rho_*^2T_*^{-7}b^9p^{-7}$. Thus

$$
\boxed{\frac{d}{dx}\left(\frac pb\right)=-D\frac{b^9l}{x^2p^7},\qquad D=\frac{3\kappa_0Z(1+X)\mathcal R^8LR}{256\pi^3ac\mu^8G^8M^6}.}
$$

The [luminosity](../../../../../luminosity.md) equation follows from the specific heating rate of the [Proton–proton chain](../../../../../proton-proton-chain.md):

$$
\frac{L}{R}\frac{dl}{dx}=4\pi R^2x^2\epsilon_0X^2\rho_*^2T_*^4p^4b^{-2}.
$$

Consequently

$$
\boxed{\frac{dl}{dx}=Ex^2p^4b^{-2},\qquad E=\frac{\epsilon_0X^2M^6}{4\pi R^7L}\left(\frac{\mu G}{\mathcal R}\right)^4.}
$$

These give all four dimensionless [stellar structure equations](../../../../../stellar-structure-equations.md) with their numerical coefficients.

The [stellar homology](../../../../../stellar-homology.md) assumption means the dimensionless profiles are shared across the models, not merely that an individual model can be written in dimensionless coordinates. The displayed equations then require $D$ and $E$ to be fixed. Holding the universal constants and $\kappa_0,\epsilon_0$ fixed gives

$$
L\propto\frac{\mu^8M^6}{\zeta R},\qquad L\propto\frac{X^2\mu^4M^6}{R^7}.
$$

Equating the two cancels $M^6$ and yields $R^6\propto X^2\zeta\mu^{-4}$. Therefore the [radius](../../../../../radius.md) and [mass-luminosity relation](../../../../../mass-luminosity-relation.md) are

$$
\boxed{R\propto X^{1/3}[Z(1+X)]^{1/6}\mu^{-2/3},\qquad L\propto\frac{M^6\mu^{26/3}}{X^{1/3}Z^{7/6}(1+X)^{7/6}}.}
$$

The mass-independent [radius](../../../../../radius.md) is a consequence of the particular heating and [opacity](../../../../../opacity.md) exponents in this model; it is not a general [radius](../../../../../radius.md) law for main-sequence [stars](../../../../../star.md).

Initially $X=X_0$ is the same for all [stars](../../../../../star.md). The adopted [mean molecular weight](../../../../../mean-molecular-weight.md) $\mu=4/(5X+3)$ also has the same initial value, neglecting its small direct dependence on $Z$. Thus $R\propto Z^{1/6}$. At fixed [luminosity](../../../../../luminosity.md), the [Stefan–Boltzmann law](../../../../../stefan-boltzmann-law.md) $L=4\pi R^2\sigma T_e^4$ gives

$$
\boxed{T_e\propto R^{-1/2}\propto Z^{-1/12}.}
$$

The [stars](../../../../../star.md) compared here can have different [masses](../../../../../mass.md); the [luminosity](../../../../../luminosity.md) law adjusts the [mass](../../../../../mass.md) to keep $L$ fixed.

For the evolution, take the stellar [mass](../../../../../mass.md) as constant and maintain homogeneous composition. The available energy in the remaining [hydrogen](../../../../../hydrogen.md) is $ME_HX$, so [conservation of energy](../../../../../conservation-of-energy.md) in the nuclear-powered model gives

$$
L=-\frac{d}{dt}(ME_HX),\qquad\boxed{\frac{dX}{dt}=-\frac{L}{ME_H}.}
$$

This includes the entire mixed [hydrogen](../../../../../hydrogen.md) reservoir, not just the [mass](../../../../../mass.md) in a central burning region.

To determine the [turnoff mass of a homogeneously mixed proton-proton-burning population](../../../../../turnoff-mass-of-a-homogeneously-mixed-proton-proton-burning-population.md), write the [luminosity](../../../../../luminosity.md) law as $L=C M^6 Z^{-7/6}H(X)$, where

$$
H(X)=\frac{\mu(X)^{26/3}}{X^{1/3}(1+X)^{7/6}},\qquad \mu(X)=\frac4{5X+3}.
$$

Separating variables, the time to evolve from $X_0$ to $fX_0$ is

$$
t=\frac{E_H}{C}M^{-5}Z^{7/6}\int_{fX_0}^{X_0}X^{1/3}(1+X)^{7/6}\left(\frac{5X+3}{4}\right)^{26/3}dX.
$$

For a common $X_0$ and $0\leq f<1$, this integral is a positive finite constant independent of $M,Z,t$. It follows that **the turning-off [stars](../../../../../star.md) satisfy**

$$
\boxed{M\propto Z^{7/30}t^{-1/5}.}
$$

The integration retains the evolving [luminosity](../../../../../luminosity.md) and [mean molecular weight](../../../../../mean-molecular-weight.md); replacing $L$ by its initial value is unnecessary.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 66](../../paper-66-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
