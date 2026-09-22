# Paper 66

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper66.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper66.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use [radiative homology with proton-proton burning and inverse-fourth-power opacity](../../../stellar-structure.md#radiative-homology-with-proton-proton-burning-and-inverse-fourth-power-opacity), retaining the composition factors throughout. To distinguish the stellar [radius](../../../topology.md#radius) from the [stellar gas constant](../../../thermodynamics.md#stellar-gas-constant), write them as $R$ and $\mathcal R$. With [gas pressure](../../../thermodynamics.md#gas-pressure) alone, introduce the scale factors

$$
\rho_* =\frac{M}{4\pi R^3},\qquad P_* =\frac{GM^2}{4\pi R^4},\qquad T_* =\frac{\mu GM}{\mathcal RR}.
$$

The [ideal gas](../../../thermodynamics.md#ideal-gas) equation gives $\rho=\rho_*b$, $P=P_*p$ and $T=T_*p/b$. Substitution into [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) and [mass conservation](../../../continuum-mechanics.md#mass-conservation) gives

$$
\frac{P_*}{R}\frac{dp}{dx}=-\frac{GM\rho_*}{R^2}\frac{qb}{x^2},\qquad \frac{M}{R}\frac{dq}{dx}=4\pi R^2\rho_*x^2b,
$$

so **$p'=-bq/x^2$ and $q'=x^2b$**.

Set $\zeta=Z(1+X)$. The [radiative diffusion in a star](../../../stellar-structure.md#radiative-diffusion-in-a-star) equation, with the stipulated [opacity](../../../stellar-structure.md#opacity), becomes

$$
\frac{T_*}{R}\frac{d}{dx}\left(\frac pb\right)=-\frac{3\kappa_0\zeta\rho_*^2L}{16\pi acR^2T_*^7}\frac{b^9l}{x^2p^7}.
$$

Here $\rho^2T^{-7}=\rho_*^2T_*^{-7}b^9p^{-7}$. Thus

$$
\boxed{\frac{d}{dx}\left(\frac pb\right)=-D\frac{b^9l}{x^2p^7},\qquad D=\frac{3\kappa_0Z(1+X)\mathcal R^8LR}{256\pi^3ac\mu^8G^8M^6}.}
$$

The [luminosity](../../../astrophysics.md#luminosity) equation follows from the specific heating rate of the [Proton–proton chain](../../../stellar-astrophysics.md#proton-proton-chain):

$$
\frac{L}{R}\frac{dl}{dx}=4\pi R^2x^2\epsilon_0X^2\rho_*^2T_*^4p^4b^{-2}.
$$

Consequently

$$
\boxed{\frac{dl}{dx}=Ex^2p^4b^{-2},\qquad E=\frac{\epsilon_0X^2M^6}{4\pi R^7L}\left(\frac{\mu G}{\mathcal R}\right)^4.}
$$

These give all four dimensionless [stellar structure equations](../../../stellar-structure.md#stellar-structure-equations) with their numerical coefficients.

The [stellar homology](../../../stellar-structure.md#stellar-homology) assumption means the dimensionless profiles are shared across the models, not merely that an individual model can be written in dimensionless coordinates. The displayed equations then require $D$ and $E$ to be fixed. Holding the universal constants and $\kappa_0,\epsilon_0$ fixed gives

$$
L\propto\frac{\mu^8M^6}{\zeta R},\qquad L\propto\frac{X^2\mu^4M^6}{R^7}.
$$

Equating the two cancels $M^6$ and yields $R^6\propto X^2\zeta\mu^{-4}$. Therefore the [radius](../../../topology.md#radius) and [mass-luminosity relation](../../../stellar-structure.md#mass-luminosity-relation) are

$$
\boxed{R\propto X^{1/3}[Z(1+X)]^{1/6}\mu^{-2/3},\qquad L\propto\frac{M^6\mu^{26/3}}{X^{1/3}Z^{7/6}(1+X)^{7/6}}.}
$$

The mass-independent [radius](../../../topology.md#radius) is a consequence of the particular heating and [opacity](../../../stellar-structure.md#opacity) exponents in this model; it is not a general [radius](../../../topology.md#radius) law for main-sequence [stars](../../../stellar-astrophysics.md#star).

Initially $X=X_0$ is the same for all [stars](../../../stellar-astrophysics.md#star). The adopted [mean molecular weight](../../../thermodynamics.md#mean-molecular-weight) $\mu=4/(5X+3)$ also has the same initial value, neglecting its small direct dependence on $Z$. Thus $R\propto Z^{1/6}$. At fixed [luminosity](../../../astrophysics.md#luminosity), the [Stefan–Boltzmann law](../../../thermodynamics.md#stefan-boltzmann-law) $L=4\pi R^2\sigma T_e^4$ gives

$$
\boxed{T_e\propto R^{-1/2}\propto Z^{-1/12}.}
$$

The [stars](../../../stellar-astrophysics.md#star) compared here can have different [masses](../../../classical-mechanics.md#mass); the [luminosity](../../../astrophysics.md#luminosity) law adjusts the [mass](../../../classical-mechanics.md#mass) to keep $L$ fixed.

For the evolution, take the stellar [mass](../../../classical-mechanics.md#mass) as constant and maintain homogeneous composition. The available energy in the remaining [hydrogen](../../../chemistry.md#hydrogen) is $ME_HX$, so [conservation of energy](../../../physics.md#conservation-of-energy) in the nuclear-powered model gives

$$
L=-\frac{d}{dt}(ME_HX),\qquad\boxed{\frac{dX}{dt}=-\frac{L}{ME_H}.}
$$

This includes the entire mixed [hydrogen](../../../chemistry.md#hydrogen) reservoir, not just the [mass](../../../classical-mechanics.md#mass) in a central burning region.

To determine the [turnoff mass of a homogeneously mixed proton-proton-burning population](../../../stellar-structure.md#turnoff-mass-of-a-homogeneously-mixed-proton-proton-burning-population), write the [luminosity](../../../astrophysics.md#luminosity) law as $L=C M^6 Z^{-7/6}H(X)$, where

$$
H(X)=\frac{\mu(X)^{26/3}}{X^{1/3}(1+X)^{7/6}},\qquad \mu(X)=\frac4{5X+3}.
$$

Separating variables, the time to evolve from $X_0$ to $fX_0$ is

$$
t=\frac{E_H}{C}M^{-5}Z^{7/6}\int_{fX_0}^{X_0}X^{1/3}(1+X)^{7/6}\left(\frac{5X+3}{4}\right)^{26/3}dX.
$$

For a common $X_0$ and $0\leq f<1$, this integral is a positive finite constant independent of $M,Z,t$. It follows that **the turning-off [stars](../../../stellar-astrophysics.md#star) satisfy**

$$
\boxed{M\propto Z^{7/30}t^{-1/5}.}
$$

The integration retains the evolving [luminosity](../../../astrophysics.md#luminosity) and [mean molecular weight](../../../thermodynamics.md#mean-molecular-weight); replacing $L$ by its initial value is unnecessary.

## 2

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For the [Schwarzschild criterion](../../../stellar-structure.md#schwarzschild-criterion), displace a small gas parcel upwards. Assume its composition is unchanged, it remains in [pressure](../../../thermodynamics.md#pressure) balance with its surroundings, and it moves quickly enough that heat exchange is negligible. The parcel obeys the [adiabatic equation of state](../../../thermodynamics.md#adiabatic-equation-of-state) $P\rho^{-\gamma}=\mathrm{constant}$. Combining this with the [ideal gas](../../../thermodynamics.md#ideal-gas) equation gives $T\propto P^{(\gamma-1)/\gamma}$, so its [adiabatic temperature gradient](../../../exoplanet.md#adiabatic-temperature-gradient) is $\nabla_{\mathrm{ad}}=(\gamma-1)/\gamma=2/5$.

Let the surrounding [temperature gradient](../../../thermodynamics.md#temperature-gradient) be $\nabla=d\log T/d\log P$. For an upward displacement $\delta\log P<0$, the parcel's [temperature](../../../thermodynamics.md#temperature) relative to its new surroundings is

$$
\delta\log T_{\mathrm{parcel}}-\delta\log T_{\mathrm{environment}}=(\nabla_{\mathrm{ad}}-\nabla)\delta\log P.
$$

If $\nabla<\nabla_{\mathrm{ad}}$, this is negative: the parcel is cooler and, at equal [pressure](../../../thermodynamics.md#pressure) and composition, denser than its surroundings. It therefore sinks back; a downward displacement likewise gives a restoring [buoyancy](../../../fluid-mechanics.md#buoyancy) force. If the inequality is reversed, the displaced parcel continues to rise. The stability condition is thus

$$
\boxed{\nabla=\frac PT\frac{dT}{dP}<\frac25.}
$$

Equality is the neutral boundary. There is no composition-gradient term because the ideal-gas parcel and the background have the same [mean molecular weight](../../../thermodynamics.md#mean-molecular-weight).

In the thin upper [stellar atmosphere](../../../stellar-astrophysics.md#stellar-atmosphere), take a plane-parallel approximation with constant $g$, optical depth increasing inward, and zero overlying [pressure](../../../thermodynamics.md#pressure) $P(0)=0$. [Hydrostatic equilibrium in optical depth](../../../stellar-structure.md#hydrostatic-equilibrium-in-optical-depth) gives $dP/d\tau=g/\kappa$. The [ideal gas](../../../thermodynamics.md#ideal-gas) equation converts the stipulated [opacity](../../../stellar-structure.md#opacity) into

$$
\kappa=\frac{\kappa_0\mu P}{\mathcal R}T^{4\beta},\qquad \frac{dP^2}{d\tau}=\frac{2\mathcal Rg}{\kappa_0\mu}T^{-4\beta}.
$$

Define $u=1+3\tau/2$, so the given [grey atmosphere](../../../astrophysics.md#grey-atmosphere) relation is $T^4=T_e^4u/2$. Integrating from the surface gives

$$
\begin{aligned}
P^2&=\frac{2^{\beta+1}\mathcal Rg}{\kappa_0\mu T_e^{4\beta}}\int_0^\tau(1+3t/2)^{-\beta}dt\\
&=\frac{2^{\beta+2}\mathcal Rg}{3\kappa_0(\beta-1)\mu T_e^{4\beta}}\left(1-u^{1-\beta}\right).
\end{aligned}
$$

This proves the required [pressure](../../../thermodynamics.md#pressure) law. In particular $P^2\propto gT_e^{-4\beta}$ times a function only of $u$ and $\beta$.

For the [grey-atmosphere convection onset with density-linear opacity](../../../stellar-structure.md#grey-atmosphere-convection-onset-with-density-linear-opacity), differentiate the two profiles to obtain the radiative [temperature gradient](../../../thermodynamics.md#temperature-gradient):

$$
\frac{d\log T}{d\tau}=\frac3{8u},\qquad \frac{d\log P}{d\tau}=\frac{3(\beta-1)u^{-\beta}}{4(1-u^{1-\beta})},\qquad \nabla_{\mathrm{rad}}=\frac{u^{\beta-1}-1}{2(\beta-1)}.
$$

It increases monotonically from zero, since $\beta>1$, and first reaches the [adiabatic temperature gradient](../../../exoplanet.md#adiabatic-temperature-gradient) at $u_b^{\beta-1}=(4\beta+1)/5$. Therefore

$$
\boxed{\tau_b=\frac23\left[\left(\frac{4\beta+1}{5}\right)^{1/(\beta-1)}-1\right].}
$$

Below this point the radiative stratification is unstable and [convection](../../../fluid-mechanics.md#convection) must transport some of the outward energy flux.

At the outer [convection](../../../fluid-mechanics.md#convection) boundary, $u_b$ depends only on $\beta$, so $T_b=T_e(u_b/2)^{1/4}\propto T_e$ and $P_b\propto g^{1/2}T_e^{-2\beta}$ for fixed $\mu,\kappa_0,\beta$. The matching constant in $P=KT^{5/2}$ is $K=P_b/T_b^{5/2}$. Consequently

$$
\boxed{K\propto g^{1/2}T_e^{-2\beta-5/2}.}
$$

This [temperature](../../../thermodynamics.md#temperature) form of the polytropic relation follows from an ideal monatomic adiabat; its $K$ is not the density-polytrope coefficient in Question 3.

For the [deep radiative boundary beneath a power-law-opacity convective envelope](../../../stellar-structure.md#deep-radiative-boundary-beneath-a-power-law-opacity-convective-envelope), negligible envelope [mass](../../../classical-mechanics.md#mass) and absent local energy generation give $m\simeq M$ and $L_r\simeq L$. Divide the radiative [temperature](../../../thermodynamics.md#temperature) equation by the [pressure](../../../thermodynamics.md#pressure) equation to get the [stellar radiative temperature gradient](../../../stellar-structure.md#stellar-radiative-temperature-gradient)

$$
\nabla_{\mathrm{rad}}=\frac{3\kappa L P}{16\pi acGM T^4}.
$$

This is the gradient that would be needed if radiation alone carried $L$, and it is the quantity to compare with $2/5$ even while the actual region is convective. The deeper [Kramers' opacity law](../../../stellar-structure.md#kramers-opacity-law) gives $\kappa=\kappa_1\mu PT^{-9/2}/\mathcal R$. Substituting $P=KT^{5/2}$ yields

$$
\nabla_{\mathrm{rad}}=\frac{3\kappa_1\mu K^2L}{16\pi ac\mathcal RGM T^{7/2}}.
$$

As $T$ rises inward this decreases, so the transition back to a stable radiative interior is at

$$
\boxed{\frac{3\kappa_1\mu K^2L}{16\pi ac\mathcal RGM T_{\mathrm{in}}^{7/2}}=\frac25.}
$$

Thus $T_{\mathrm{in}}^{7/2}\propto K^2L/M$. Using the outer matching and the [Stefan–Boltzmann law](../../../thermodynamics.md#stefan-boltzmann-law),

$$
K^2\frac LM\propto gT_e^{-4\beta-5}\frac LM,\qquad g\frac LM=\frac{GM}{R^2}\frac{4\pi R^2\sigma T_e^4}{M}=4\pi G\sigma T_e^4.
$$

The [mass](../../../classical-mechanics.md#mass) and [radius](../../../topology.md#radius) cancel. Hence, at fixed [opacity](../../../stellar-structure.md#opacity) coefficients and composition,

$$
\boxed{T_{\mathrm{in}}\propto T_e^{-(8\beta+2)/7}.}
$$

This uses the same adiabat through the [convection](../../../fluid-mechanics.md#convection) zone and distinguishes its inner transition [temperature](../../../thermodynamics.md#temperature) from its outer onset [temperature](../../../thermodynamics.md#temperature).

## 3

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a regular, spherical [star](../../../stellar-astrophysics.md#star), [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) gives $dP/dr=-Gm(r)\rho(r)/r^2$. Multiply by $4\pi r^3$ and integrate to the surface. [Integration by parts](../../../calculus.md#integration-by-parts) gives

$$
\int_0^R4\pi r^3\frac{dP}{dr}dr=4\pi R^3P(R)-3\int_0^R4\pi r^2P\,dr.
$$

The central boundary term vanishes for finite central [pressure](../../../thermodynamics.md#pressure). Since $dm=4\pi r^2\rho\,dr$, the right-hand side of the integrated hydrostatic equation is

$$
-\int_0^R4\pi Gm\rho r\,dr=-\int_0^M\frac{Gm}{r(m)}dm=\Omega.
$$

The last expression is the [gravitational energy](../../../classical-mechanics.md#gravitational-energy): adding a thin [mass](../../../classical-mechanics.md#mass) shell $dm$ to the interior [mass](../../../classical-mechanics.md#mass) $m$ contributes $-Gm\,dm/r$, counting each interacting pair once. Hence

$$
3\int_0^M\frac P\rho dm+\Omega=4\pi R^3P(R).
$$

With the specified zero surface [pressure](../../../thermodynamics.md#pressure) this proves the [stellar virial theorem](../../../stellar-structure.md#stellar-virial-theorem) in the required form,

$$
\boxed{3\int_0^M\frac P\rho dm+\Omega=0.}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

To derive the [nonrelativistic electron-degeneracy pressure in a hydrogen-helium mixture](../../../statistical-physics.md#nonrelativistic-electron-degeneracy-pressure-in-a-hydrogen-helium-mixture), take fully ionized [hydrogen](../../../chemistry.md#hydrogen) and [helium](../../../chemistry.md#helium) with [hydrogen mass fraction](../../../stellar-astrophysics.md#hydrogen-mass-fraction) $X$, the [Electron](../../../physics.md#electron) [number density](../../../statistical-physics.md#number-density) is

$$
n_e=\frac{X\rho}{m_p}+2\frac{(1-X)\rho}{4m_p}=\frac{(1+X)\rho}{2m_p}.
$$

Here [helium](../../../chemistry.md#helium) nuclei have [mass](../../../classical-mechanics.md#mass) $4m_p$ in the approximation used in the question. Filling the two spin states of each [momentum](../../../classical-mechanics.md#momentum) mode up to the [Fermi momentum](../../../statistical-physics.md#fermi-momentum) $p_0$ gives

$$
n_e=\int_0^{p_0}\frac{8\pi p^2}{h^3}dp=\frac{8\pi p_0^3}{3h^3},\qquad p_0=h\left(\frac{3n_e}{8\pi}\right)^{1/3}.
$$

The isotropic [momentum](../../../classical-mechanics.md#momentum) flux gives [pressure](../../../thermodynamics.md#pressure) $\frac13\int pv\,dn$. For nonrelativistic [Electrons](../../../physics.md#electron) $v=p/m_e$, so the [electron degeneracy pressure](../../../statistical-physics.md#electron-degeneracy-pressure) is

$$
\begin{aligned}
P_e&=\frac13\int_0^{p_0}\frac{p^2}{m_e}\frac{8\pi p^2}{h^3}dp=\frac{8\pi p_0^5}{15m_eh^3}\\
&=\frac{h^2}{5m_e}\left(\frac3{8\pi}\right)^{2/3}n_e^{5/3}.
\end{aligned}
$$

Substitute the composition-dependent $n_e$ and simplify powers of two:

$$
\boxed{P_e=K\rho^{5/3},\qquad K=\left(\frac3{2\pi}\right)^{2/3}\frac{h^2(1+X)^{5/3}}{40m_em_p^{5/3}}.}
$$

Comparing $5/3=1+1/n$ gives **the [polytropic index](../../../stellar-structure.md#polytropic-index) $n=3/2$**. The result assumes complete [Electron](../../../physics.md#electron) degeneracy, $p_0\ll m_ec$, and negligible nuclear [mass](../../../classical-mechanics.md#mass) corrections.

Now adopt the stated approximate partially degenerate [equation of state](../../../thermodynamics.md#equation-of-state), keeping composition and hence $K,\mu$ fixed during contraction. Set $q=m/M$ and define the mass-averaged [temperature](../../../thermodynamics.md#temperature) $\overline T_M=\int_0^1T\,dq$. The [stellar virial theorem](../../../stellar-structure.md#stellar-virial-theorem) from part (a) gives

$$
3K\int_0^1\rho^{2/3}dq+\frac{3\mathcal R}{\mu}\overline T_M=-\frac{\Omega}{M}.
$$

For an index-$3/2$ [stellar polytrope](../../../stellar-structure.md#stellar-polytrope), the permitted gravitational-energy formula is $\Omega=-6GM^2/(7R)$. Also, using $\bar\rho=3M/(4\pi R^3)$,

$$
\rho^{2/3}=\frac{M^{2/3}}{R^2}\left(\frac{3\rho}{4\pi\bar\rho}\right)^{2/3}.
$$

Thus, with $A=3K\int_0^1[3\rho/(4\pi\bar\rho)]^{2/3}dq$,

$$
\boxed{\overline T_M=\frac{2\mu GM}{7\mathcal RR}-\frac{\mu A M^{2/3}}{3\mathcal RR^2}.}
$$

The normalized [density](../../../fluid-mechanics.md#density) $\rho/\bar\rho$ is a fixed function of $q$ for this homologous polytropic structure. Therefore its integral and $K$ fix $A$, which is independent of $M$ and $R$ for a common composition. The mean here is mass-weighted, rather than a volume average.

For the [mass-averaged temperature maximum in a partially degenerate polytrope](../../../stellar-astrophysics.md#mass-averaged-temperature-maximum-in-a-partially-degenerate-polytrope), put $\alpha=2\mu GM/(7\mathcal R)$ and $\delta=\mu A M^{2/3}/(3\mathcal R)$, both positive. As a function of $s=1/R$ the [temperature](../../../thermodynamics.md#temperature) is the concave quadratic

$$
\overline T_M=\alpha s-\delta s^2=\frac{\alpha^2}{4\delta}-\delta\left(s-\frac\alpha{2\delta}\right)^2.
$$

It reaches its maximum when $R=2\delta/\alpha=7A M^{-1/3}/(3G)$, with

$$
\boxed{\overline T_{M,\max}=\frac{\alpha^2}{4\delta}=\frac{3\mu G^2M^{4/3}}{49\mathcal RA}.}
$$

At large [radius](../../../topology.md#radius), contraction increases the [temperature](../../../thermodynamics.md#temperature) as in a thermally supported [star](../../../stellar-astrophysics.md#star). Once [Electron](../../../physics.md#electron) degeneracy provides a sufficiently large fraction of the support, further contraction can lower the thermal [temperature](../../../thermodynamics.md#temperature). The formal zero-temperature [radius](../../../topology.md#radius) is $R_{\mathrm{deg}}=\delta/\alpha=R_{\max}/2$, with $R_{\mathrm{deg}}\propto M^{-1/3}$. The continuation to negative temperatures would be unphysical; the adopted sequence only describes its positive-temperature part.

The [contraction-limited central temperature](../../../stellar-astrophysics.md#contraction-limited-central-temperature) has the same [mass](../../../classical-mechanics.md#mass) scaling. Indeed, if the total polytropic [pressure](../../../thermodynamics.md#pressure) is $P=K_{\mathrm{tot}}\rho^{5/3}$, the approximate [equation of state](../../../thermodynamics.md#equation-of-state) gives $T=(\mu/\mathcal R)(K_{\mathrm{tot}}-K)\rho^{2/3}$. The fixed [density](../../../fluid-mechanics.md#density) profile therefore fixes $T_c/\overline T_M$. A sufficiently small [mass](../../../classical-mechanics.md#mass) never reaches the central [temperature](../../../thermodynamics.md#temperature) required for sustained [hydrogen burning](../../../stellar-astrophysics.md#hydrogen-burning), producing a [hydrogen-burning minimum mass](../../../stellar-astrophysics.md#hydrogen-burning-minimum-mass). Such an object becomes a cooling, degeneracy-supported [brown dwarf](../../../stellar-astrophysics.md#brown-dwarf) instead of settling onto the [main sequence](../../../stellar-astrophysics.md#main-sequence). More massive contracting objects can ignite [hydrogen](../../../chemistry.md#hydrogen) before reaching this degeneracy-limited maximum. This conclusion uses the nonrelativistic, fixed-composition model; it does not require extrapolation into the relativistic regime.

## 4

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Treat the [stars](../../../stellar-astrophysics.md#star) as [point masses](../../../classical-mechanics.md#point-mass) for the orbital motion, neglecting their spin [angular momenta](../../../classical-mechanics.md#angular-momentum). Let $M=M_1+M_2$. Their distances from the [centre of mass](../../../classical-mechanics.md#center-of-mass) are $a_1=aM_2/M$ and $a_2=aM_1/M$. The sum of their orbital [angular momenta](../../../classical-mechanics.md#angular-momentum) is

$$
\begin{aligned}
J&=(M_1a_1^2+M_2a_2^2)\Omega\\
&=\frac{M_1M_2}{M}a^2\left(\frac{GM}{a^3}\right)^{1/2}.
\end{aligned}
$$

Thus the [circular-binary orbital angular momentum](../../../stellar-astrophysics.md#circular-binary-orbital-angular-momentum) is

$$
\boxed{J=\frac{M_1M_2}{M_1+M_2}\sqrt{G(M_1+M_2)a}.}
$$

For [conservative binary mass transfer](../../../stellar-astrophysics.md#conservative-binary-mass-transfer), both $M$ and $J$ are fixed. In terms of the [binary mass ratio](../../../stellar-astrophysics.md#binary-mass-ratio) $q=M_1/M_2$, $M_1=Mq/(1+q)$ and $M_2=M/(1+q)$, hence

$$
J^2=GM^3a\frac{q^2}{(1+q)^4},\qquad\boxed{a(1+q)^{-4}q^2=C,\quad C=\frac{J^2}{GM^3}.}
$$

[Mass conservation](../../../continuum-mechanics.md#mass-conservation) also gives $dM_2=-dM_1$, so

$$
\frac{d\log M_2}{d\log M_1}=-q,\qquad\frac{d\log q}{d\log M_1}=1+q.
$$

Differentiating $J\propto M_1M_2a^{1/2}$ at fixed $M,J$ gives $d\log a/d\log M_1=2(q-1)$. Therefore the stipulated [Roche lobe](../../../stellar-astrophysics.md#roche-lobe) law has the [Roche-lobe radius response exponent](../../../stellar-astrophysics.md#roche-lobe-radius-response-exponent)

$$
\zeta_L=\frac{d\log R_L}{d\log M_1}=\frac3{10}(1+q)+2(q-1)=\frac{23q-17}{10}.
$$

Define the overfill by $\Delta=\log(R_1/R_L)$. On a time scale short compared with the slow change of $K$, the donor's response is $d\log R_1=\beta\,d\log M_1$. Thus

$$
d\Delta=(\beta-\zeta_L)d\log M_1.
$$

During [mass](../../../classical-mechanics.md#mass) loss $d\log M_1<0$. If $\zeta_L>\beta$, [mass](../../../classical-mechanics.md#mass) loss increases the overfill and therefore drives more [mass](../../../classical-mechanics.md#mass) loss: this is positive feedback, giving more rapid [Roche-lobe overflow](../../../stellar-astrophysics.md#roche-lobe-overflow). If $\zeta_L<\beta$, [mass](../../../classical-mechanics.md#mass) loss decreases the overfill and can balance the slow expansion due to [stellar evolution](../../../stellar-astrophysics.md#stellar-evolution). More explicitly, with $k_{\mathrm{ev}}=d\log K/dt>0$, contact requires

$$
0=\dot\Delta=k_{\mathrm{ev}}+(\beta-\zeta_L)\frac{\dot M_1}{M_1}.
$$

A slow negative transfer rate can satisfy this only on the stable side $\beta>\zeta_L$. The rapid-transfer condition is therefore

$$
\boxed{q>\frac{17+10\beta}{23}.}
$$

Its time scale depends on the physical donor response represented by $\beta$; it need not be a dynamical time scale if $\beta$ is a thermal-equilibrium mass-radius exponent.

For [Roche-lobe overflow feedback with a constant wind torque factor](../../../stellar-astrophysics.md#roche-lobe-overflow-feedback-with-a-constant-wind-torque-factor), retain [mass conservation](../../../continuum-mechanics.md#mass-conservation) to the stated approximation but allow the prescribed angular-momentum loss. Since $d\log J=f\,d\log M_1$, differentiation gives

$$
f=1-q+\frac12\frac{d\log a}{d\log M_1},\qquad\frac{d\log a}{d\log M_1}=2(q-1+f).
$$

The new [Roche-lobe radius response exponent](../../../stellar-astrophysics.md#roche-lobe-radius-response-exponent) is

$$
\zeta_L=\frac3{10}(1+q)+2(q-1+f)=\frac{23q-17+20f}{10}.
$$

The same overfill calculation gives

$$
\boxed{q>\frac{17-20f+10\beta}{23}.}
$$

A loss of [angular momentum](../../../classical-mechanics.md#angular-momentum) has $f>0$ because $\dot M_1<0$, and it lowers the critical ratio by making the orbit contract more strongly.

For the specified solar-mass donor exponent $\beta=1/2$, the answer is

$$
\boxed{q>\frac{22-20f}{23},\qquad q>0.}
$$

Without the wind torque this becomes **$q>22/23\simeq0.957$**, so donors slightly less massive than their companions can already lie on the rapid-transfer side of this model. For $0<f<11/10$ the lower threshold is $(22-20f)/23$, and for $f\geq11/10$ every positive $q$ satisfies the strict inequality. There is no finite upper bound on $q$ from this criterion. Since the paper does not specify $f$, the wind case has a conditional range rather than a unique numerical cutoff.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
