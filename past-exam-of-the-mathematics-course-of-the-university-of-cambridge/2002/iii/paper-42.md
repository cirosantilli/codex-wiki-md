# Paper 42

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper42.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper42.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

A [stellar polytrope](../../../stellar-structure.md#stellar-polytrope) has a spatially constant coefficient $K$ in the relation $P=K\rho^{1+1/n}$; $n$ is its [polytropic index](../../../stellar-structure.md#polytropic-index). This relates [pressure](../../../thermodynamics.md#pressure) to [mass density](../../../fluid-mechanics.md#density) and need not describe an adiabatic gas. Combining [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) with [mass conservation](../../../continuum-mechanics.md#mass-conservation) eliminates the enclosed [mass](../../../classical-mechanics.md#mass):

$$
\frac{1}{r^2}\frac{d}{dr}\left(\frac{r^2}{\rho}\frac{dP}{dr}\right)=-4\pi G\rho.
$$

For $\rho=\rho_c\theta^n$, the [polytropic equation of state](../../../astrophysical-fluid-dynamics.md#polytropic-equation-of-state) gives $(1/\rho)dP/dr=(n+1)K\rho_c^{1/n}d\theta/dr$. Choose the [Lane-Emden variables for a stellar polytrope](../../../stellar-structure.md#lane-emden-variables-for-a-stellar-polytrope) with

$$
\alpha^2=\frac{(n+1)K}{4\pi G}\rho_c^{1/n-1},\qquad r=\alpha\xi.
$$

Substitution then gives the dimensionless [Lane-Emden equation](../../../nonlinear-analysis.md#lane-emden-equation):

$$
\boxed{\frac{1}{\xi^2}(\xi^2\theta')'=-\theta^n.}
$$

A regular stellar centre has $\theta(0)=1$, $\theta'(0)=0$ and $m(0)=0$. In particular the regular central expansion is $\theta=1-\xi^2/6+O(\xi^4)$. For an isolated finite-radius [stellar polytrope](../../../stellar-structure.md#stellar-polytrope) with negligible external [pressure](../../../thermodynamics.md#pressure), the surface is the first zero $\xi_1$ of $\theta$, and $R=\alpha\xi_1$. A core embedded in an envelope can instead end at a positive matching [pressure](../../../thermodynamics.md#pressure), before this zero.

The integrated [Lane-Emden equation](../../../nonlinear-analysis.md#lane-emden-equation) is $\xi^2\theta'=-\int_0^\xi s^2\theta(s)^n ds$. Thus [mass conservation](../../../continuum-mechanics.md#mass-conservation) gives the [Lane-Emden mass formula](../../../stellar-structure.md#lane-emden-mass-formula) directly:

$$
\boxed{m(\xi)=-4\pi\rho_c\alpha^3\xi^2\theta'(\xi).}
$$

For the proposed functional form, differentiation gives

$$
\theta''+\frac{2}{\xi}\theta'=2\beta\gamma(1+\beta\xi^2)^{\gamma-2}\bigl[3+(2\gamma+1)\beta\xi^2\bigr].
$$

Choosing $\gamma=-1/2$ removes the extra polynomial factor; equality to $-\theta^5$ then requires $3\beta=1$. The regular [polytrope of index five](../../../stellar-structure.md#polytrope-of-index-five) is therefore

$$
\boxed{\beta=\frac13,\quad\gamma=-\frac12,\quad\theta=(1+\xi^2/3)^{-1/2}.}
$$

Its enclosed [mass](../../../classical-mechanics.md#mass) and enclosed mean [mass density](../../../fluid-mechanics.md#density) are

$$
m(\xi)=\frac{4\pi\rho_c\alpha^3\xi^3}{3(1+\xi^2/3)^{3/2}},\qquad
\overline\rho(\xi)=\frac{3m}{4\pi r^3}=\rho_c(1+\xi^2/3)^{-3/2}.
$$

There is no finite zero: its isolated radius is infinite. Nevertheless its total [mass](../../../classical-mechanics.md#mass) converges, since the outer [mass density](../../../fluid-mechanics.md#density) falls as $r^{-5}$:

$$
\boxed{M=4\pi\sqrt3\rho_c\alpha^3,\qquad R=\infty,\qquad\lim_{r\to\infty}\overline\rho(r)=0.}
$$

The zero mean [mass density](../../../fluid-mechanics.md#density) is a limiting volume average, not a statement that the material has zero [mass density](../../../fluid-mechanics.md#density) at finite radius.

To turn this density model into a [CNO cycle](../../../stellar-astrophysics.md#cno-cycle) burning model, use gas-dominated [pressure](../../../thermodynamics.md#pressure) and uniform [mean molecular weight](../../../thermodynamics.md#mean-molecular-weight). The [ideal gas law](../../../thermodynamics.md#ideal-gas-law) and the [polytropic equation of state](../../../astrophysical-fluid-dynamics.md#polytropic-equation-of-state) then imply $T/T_c=\theta$. Without this thermal assumption a [polytropic equation of state](../../../astrophysical-fluid-dynamics.md#polytropic-equation-of-state) for total [pressure](../../../thermodynamics.md#pressure) does not alone fix the [temperature](../../../thermodynamics.md#temperature) profile. Since the [stellar energy-generation rate](../../../stellar-astrophysics.md#stellar-energy-generation-rate) is power per unit [mass](../../../classical-mechanics.md#mass), its contribution to [luminosity](../../../astrophysics.md#luminosity) is $\epsilon\,dm$, giving the [luminosity integral of an index-five polytrope](../../../stellar-structure.md#luminosity-integral-of-an-index-five-polytrope):

$$
L=4\pi\epsilon_0\alpha^3\rho_c^2T_c^{11}\int_0^\infty\xi^2(1+\xi^2/3)^{-21/2}\,d\xi.
$$

Put $u=\xi/\sqrt{3+\xi^2}$. Then $\xi=\sqrt3u/\sqrt{1-u^2}$ and the dimensionless integral becomes $3\sqrt3\int_0^1u^2(1-u^2)^8du$. Evaluation gives

$$
A=12\pi\sqrt3\frac{8!\,9!\,2^{17}}{19!}=1.029415\ldots,\qquad
\boxed{L=A\epsilon_0\alpha^3\rho_c^2T_c^{11},\quad A\sim1.}
$$

The PDF's power of $\alpha$ in the proposed [luminosity](../../../astrophysics.md#luminosity) scaling is a genuine dimensional error: it must be three, rather than two. The volume element supplies $\alpha^3$; replacing it by $\alpha^2$ would give power divided by length, and could not be repaired by a dimensionless numerical constant.

The [polytrope of index five](../../../stellar-structure.md#polytrope-of-index-five) is unlikely to model a real burning [stellar core](../../../stellar-structure.md#stellar-core) well. An embedded core has a finite boundary, and a complete isolated star cannot have this infinite radius. More importantly, strongly [temperature](../../../thermodynamics.md#temperature)-sensitive [CNO cycle](../../../stellar-astrophysics.md#cno-cycle) heating concentrates the [luminosity](../../../astrophysics.md#luminosity) centrally and tends to produce a [convection zone](../../../fluid-mechanics.md#convection-zone) there. A well-mixed gas-pressure-dominated convective core is closer to an [adiabatic stellar polytrope](../../../stellar-structure.md#adiabatic-stellar-polytrope) of index $3/2$ than to index five. A finite truncation would also change the integral defining $A$; its value above pertains to the full mathematical model.

## 2

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

In [stellar homology](../../../stellar-structure.md#stellar-homology), write $r=Rx$, $m=Mf(x)$ and $\rho=\rho_c h(x)$, with common dimensionless profiles. Integrating [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) from the surface, where the [pressure](../../../thermodynamics.md#pressure) is negligible, gives

$$
P_c=\frac{GM\rho_c}{R}\int_0^1\frac{f(x)h(x)}{x^2}\,dx.
$$

The profile integral is common to the sequence. Similarly, [mass conservation](../../../continuum-mechanics.md#mass-conservation) gives $M=4\pi\rho_cR^3\int_0^1x^2h(x)dx$. These prove the [homology scaling of central stellar pressure](../../../stellar-structure.md#homology-scaling-of-central-stellar-pressure):

$$
\rho_c\propto\frac{M}{R^3},\qquad P_c\propto\frac{GM\rho_c}{R}\propto\frac{GM^2}{R^4}.
$$

The [ideal gas law](../../../thermodynamics.md#ideal-gas-law) consequently gives $T_c\propto\mu M/R$, with the gravitational and gas constants absorbed into the coefficient.

The [radiative diffusion in a star](../../../stellar-structure.md#radiative-diffusion-in-a-star) equation has a characteristic gradient $T_c/R$. Hence $L\propto RT_c^4/(\kappa_c\rho_c)$. Using [Kramers' opacity law](../../../stellar-structure.md#kramers-opacity-law), and comparing fixed-composition homologous models, this becomes

$$
L_{\rm rad}\propto\frac{RT_c^{15/2}}{\kappa_0\rho_c^2}
\propto\kappa_0^{-1}\mu^{15/2}M^{11/2}R^{-1/2}.
$$

The volume integral of the [stellar energy-generation rate](../../../stellar-astrophysics.md#stellar-energy-generation-rate) $\epsilon=\epsilon_0\rho T^\nu$ instead gives

$$
L_{\rm nuc}\propto M\epsilon_0\rho_cT_c^\nu
\propto\epsilon_0\mu^\nu M^{\nu+2}R^{-\nu-3}.
$$

The dimensionless integrals behind these relations do not depend on $M$ along a homologous sequence. In [stellar thermal equilibrium](../../../stellar-structure.md#stellar-thermal-equilibrium) the two [luminosities](../../../astrophysics.md#luminosity) agree, proving [Kramers homology with a variable nuclear exponent](../../../stellar-structure.md#kramers-homology-with-a-variable-nuclear-exponent):

$$
R^{\nu+5/2}\propto\epsilon_0\kappa_0\mu^{\nu-15/2}M^{\nu-7/2}.
$$

For the specified [proton–proton chain](../../../stellar-astrophysics.md#proton-proton-chain) exponent $\nu=7/2$, the mass factor cancels. Thus

$$
\boxed{R=\text{constant},\qquad L\propto M^{11/2}.}
$$

The model captures two important features of the [lower main sequence](../../../stellar-astrophysics.md#lower-main-sequence): [hydrogen burning](../../../stellar-astrophysics.md#hydrogen-burning) primarily uses the [proton–proton chain](../../../stellar-astrophysics.md#proton-proton-chain), and gas rather than [radiation pressure](../../../thermodynamics.md#radiation-pressure) supplies the principal support. A radiative interior and a [Kramers' opacity law](../../../stellar-structure.md#kramers-opacity-law) approximation are useful near the Sun. It is a simplified local model: the Sun has a convective envelope, the coolest [main sequence](../../../stellar-astrophysics.md#main-sequence) stars become fully convective, and real [opacities](../../../stellar-structure.md#opacity) and burning exponents vary. In particular a literally constant radius is not a realistic law over the entire [lower main sequence](../../../stellar-astrophysics.md#lower-main-sequence).

On this [proton–proton chain](../../../stellar-astrophysics.md#proton-proton-chain) branch $T_c\propto M$, because $R$ and [mean molecular weight](../../../thermodynamics.md#mean-molecular-weight) are fixed. Normalizing to the Sun gives the upper mass estimate

$$
\boxed{M_*\simeq\frac{2\times10^7}{1.5\times10^7}M_\odot=\frac43M_\odot.}
$$

For the specified [CNO cycle](../../../stellar-astrophysics.md#cno-cycle) exponent $\nu=23/2$, the homology relation instead reads $R^{14}\propto M^8$. Substituting into the radiative [luminosity](../../../astrophysics.md#luminosity) relation gives

$$
\boxed{R\propto M^{4/7},\qquad L\propto M^{73/14},\qquad T_c\propto M^{3/7}.}
$$

This branch retains the deliberately idealized fully radiative assumptions, even though real [CNO cycle](../../../stellar-astrophysics.md#cno-cycle) cores are often convective.

For a [Hertzsprung-Russell diagram](../../../stellar-astrophysics.md#hertzsprung-russell-diagram), use the [Stefan–Boltzmann law](../../../thermodynamics.md#stefan-boltzmann-law), $L=4\pi R^2\sigma T_{\rm eff}^4$. On the [proton–proton chain](../../../stellar-astrophysics.md#proton-proton-chain) branch $T_{\rm eff}\propto M^{11/8}$, so $L\propto T_{\rm eff}^4$. On the [CNO cycle](../../../stellar-astrophysics.md#cno-cycle) branch $T_{\rm eff}\propto M^{57/56}$, giving $L\propto T_{\rm eff}^{292/57}$. Thus the upper branch rises slightly more steeply toward the hot, luminous upper left in a logarithmic [Hertzsprung-Russell diagram](../../../stellar-astrophysics.md#hertzsprung-russell-diagram). The sketch below matches the approximate branches continuously at their respective burning crossovers; the true crossover has both heating terms and is smooth.

The [proton–proton chain](../../../stellar-astrophysics.md#proton-proton-chain) begins with reactions between [hydrogen](../../../chemistry.md#hydrogen) nuclei, so its specific heating scales as $X_H^2\rho T^{7/2}$ in this approximation. The catalytic [CNO cycle](../../../stellar-astrophysics.md#cno-cycle) involves [hydrogen](../../../chemistry.md#hydrogen) and CNO nuclei, and scales as $X_HZ_{\rm CNO}\rho T^{23/2}$. Here $X_H$ is the [hydrogen mass fraction](../../../stellar-astrophysics.md#hydrogen-mass-fraction) and $Z_{\rm CNO}$ the [CNO mass fraction](../../../stellar-astrophysics.md#cno-mass-fraction), not the total abundance of every metal. Consequently

$$
\frac{\epsilon_{\rm CNO}}{\epsilon_{pp}}\propto\frac{Z_{\rm CNO}}{X_H}T^8.
$$

Keeping $X_H$ fixed while dividing $Z_{\rm CNO}$ by 256 gives the [CNO crossover temperature](../../../stellar-astrophysics.md#cno-crossover-temperature)

$$
\boxed{T_{*,\rm poor}=256^{1/8}(2\times10^7\,\mathrm K)=4\times10^7\,\mathrm K,\qquad
M_{*,\rm poor}\simeq\frac83M_\odot.}
$$

The mass estimate uses the unchanged [proton–proton chain](../../../stellar-astrophysics.md#proton-proton-chain) branch below crossover, together with the stipulated unchanged [opacity](../../../stellar-structure.md#opacity) and [mean molecular weight](../../../thermodynamics.md#mean-molecular-weight).

The low-CNO [proton–proton chain](../../../stellar-astrophysics.md#proton-proton-chain) sequence therefore lies on the same locus, but extends to twice the transition mass. Beyond its later crossover the low-CNO [CNO cycle](../../../stellar-astrophysics.md#cno-cycle) sequence has the same logarithmic slope $292/57$ but a different normalization. At a fixed mass where both sequences are CNO-dominated, lowering the nuclear coefficient by 256 gives

$$
\frac{R_{\rm poor}}{R_{\rm solar}}=256^{-1/14}=2^{-4/7},\qquad
\frac{L_{\rm poor}}{L_{\rm solar}}=2^{2/7},\qquad
\frac{T_{{\rm eff},\rm poor}}{T_{{\rm eff},\rm solar}}=2^{5/14}.
$$

Thus those low-CNO models are smaller, hotter and modestly more luminous at the same mass. At the same [effective temperature](../../../stellar-structure.md#effective-temperature), their CNO branch is lower in [luminosity](../../../astrophysics.md#luminosity) than the solar-composition CNO branch; these comparisons hold different quantities fixed.

<a id="2/image-radiative-homology-sequences-for-solar-cno-abundance-and-a-cno-abundance-reduced-by-256-with-their-different-burning-crossovers"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-42-homology-sequences.png)

**[Figure 1](#2/image-radiative-homology-sequences-for-solar-cno-abundance-and-a-cno-abundance-reduced-by-256-with-their-different-burning-crossovers). Radiative homology sequences for solar CNO abundance and a CNO abundance reduced by 256, with their different burning crossovers**.

## 3

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

A constant number [star formation rate](../../../galaxy.md#star-formation-rate) over $10\,\mathrm{Gyr}$ produces a uniform present-age distribution. The [birth-age distribution under constant star formation](../../../stellar-astrophysics.md#birth-age-distribution-under-constant-star-formation) therefore gives

$$
\boxed{Y(t)=\frac{t}{10\,\mathrm{Gyr}}=0.1\frac{t}{\mathrm{Gyr}}\quad(0\le t\le10\,\mathrm{Gyr}).}
$$

Outside this age interval the [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function) is zero or one. The census here retains stellar remnants as objects, as required by the population model.

Write $m=M/M_\odot$. The [initial mass function](../../../stellar-astrophysics.md#initial-mass-function) is proportional to $m^{-3}$ on $m\ge0.2$. Normalizing the tail integral gives the [power-law initial-mass-function tail coordinate](../../../stellar-astrophysics.md#power-law-initial-mass-function-tail-coordinate):

$$
\boxed{X(m)=\frac{\int_m^\infty s^{-3}ds}{\int_{0.2}^\infty s^{-3}ds}
=\frac{0.04}{m^2}\quad(m\ge0.2).}
$$

For lower thresholds $X=1$. Because the birth [mass](../../../classical-mechanics.md#mass) and formation time have [independence](../../../random-variable.md#independent-random-variables), the [probability integral transform](../../../probability-theory.md#probability-integral-transform) makes $(X,Y)$ uniform on the unit square. $X$ is an upper-tail coordinate, so larger masses have smaller $X$.

A [red giant](../../../stellar-astrophysics.md#red-giant) of current age $t$ lies in the [stellar lifetime regions in a mass-age diagram](../../../stellar-astrophysics.md#stellar-lifetime-regions-in-a-mass-age-diagram)

$$
\frac{8}{m^2}\le\frac{t}{\mathrm{Gyr}}<\frac{10}{m^2},\qquad 0\le\frac{t}{\mathrm{Gyr}}\le10.
$$

There are no [red giants](../../../stellar-astrophysics.md#red-giant) below $m=\sqrt{0.8}$ in this model. For $\sqrt{0.8}<m<1$ the upper boundary is the population's age limit, while for $m\ge1$ both lifetime boundaries are present. A [white dwarf](../../../stellar-astrophysics.md#white-dwarf) lies above $t/\mathrm{Gyr}=10/m^2$.

In uniform [probability](../../../probability-theory.md#probability) coordinates the main-sequence boundary is $Y=20X$ and the end of the giant phase is $Y=25X$. The giant region is therefore $20X\le Y<25X$, clipped to the unit square: it is the triangle with vertices $(0,0),(1/25,1),(1/20,1)$. Its area, and hence the individual giant fraction, is

$$
\boxed{\Pr(G)=\frac12\left(\frac1{20}-\frac1{25}\right)=\frac1{200}=0.5\%.}
$$

The [white dwarf](../../../stellar-astrophysics.md#white-dwarf) region $Y\ge25X$ is the triangle with vertices $(0,0),(0,1),(1/25,1)$, giving

$$
\boxed{\Pr(W)=\frac12\frac1{25}=\frac1{50}=2\%.}
$$

The remaining $97.5\%$ are on the [main sequence](../../../stellar-astrophysics.md#main-sequence). Boundaries have zero [probability](../../../probability-theory.md#probability) and do not affect these counts. Treating every post-giant object as a [white dwarf](../../../stellar-astrophysics.md#white-dwarf) is a stipulated toy-model assumption; real high-mass stars have other [stellar remnants](../../../stellar-astrophysics.md#stellar-remnant).

<a id="3/image-red-giant-and-white-dwarf-regions-in-mass-age-coordinates-and-their-triangular-images-in-uniform-tail-mass-and-age-coordinates"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-42-population-regions.png)

**[Figure 2](#3/image-red-giant-and-white-dwarf-regions-in-mass-age-coordinates-and-their-triangular-images-in-uniform-tail-mass-and-age-coordinates). Red-giant and white-dwarf regions in mass-age coordinates and their triangular images in uniform tail-mass and age coordinates**.

For the binary calculations, use a [coeval binary population](../../../stellar-astrophysics.md#coeval-binary-population): components share their birth time even though their birth masses are independently drawn and their subsequent evolution is independent. Hence $(X_1,X_2,Y)$ is uniform in the unit cube. At a fixed age coordinate $Y=y$, a component is a giant when $y/25<X<y/20$, and a [white dwarf](../../../stellar-astrophysics.md#white-dwarf) when $0<X<y/25$. Define the conditional state fractions

$$
g(y)=\frac{y}{100},\qquad w(y)=\frac{y}{25},\qquad e(y)=g(y)+w(y)=\frac{y}{20}.
$$

Components have [conditional independence](../../../random-variable.md#conditional-independence) given $y$; averaging over the common age must be done after forming the conditional pair [probabilities](../../../probability-theory.md#probability). The [continuous-birth binary state fractions](../../../stellar-astrophysics.md#continuous-birth-binary-state-fractions) below are consequently volumes in this cube, not products of the marginal single-star fractions.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Condition on the common age $Y=y$ of the [coeval binary population](../../../stellar-astrophysics.md#coeval-binary-population). Each component is a [red giant](../../../stellar-astrophysics.md#red-giant) with conditional [probability](../../../probability-theory.md#probability) $g(y)=y/100$, independently of the other component at that age. The conditional [probability](../../../probability-theory.md#probability) of at least one giant is $1-(1-g)^2=2g-g^2$. Integrating over the uniform age distribution gives

$$
\Pr(\text{at least one giant})=\int_0^1\left(\frac{2y}{100}-\frac{y^2}{10000}\right)dy
=\frac1{100}-\frac1{30000}.
$$

Thus **the fraction is $299/30000=0.996\overline6\%$, just below $1\%$**. The subtracted term removes the systems counted twice because both components are [red giants](../../../stellar-astrophysics.md#red-giant). Using the square of the marginal giant fraction would incorrectly ignore their shared age.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

A system containing a [red giant](../../../stellar-astrophysics.md#red-giant) and another evolved component is either a giant–giant pair or an unordered giant–[white dwarf](../../../stellar-astrophysics.md#white-dwarf) pair. At common age $y$, these disjoint possibilities have conditional [probabilities](../../../probability-theory.md#probability) $g(y)^2$ and $2g(y)w(y)$. The [conditional evolved-companion fraction in a coeval binary population](../../../stellar-astrophysics.md#conditional-evolved-companion-fraction-in-a-coeval-binary-population) therefore has numerator

$$
\Pr(GG\text{ or }GW)=\int_0^1\left(\frac{y^2}{10000}+\frac{2y^2}{2500}\right)dy
=\frac9{30000}.
$$

Divide by the fraction $299/30000$ of systems containing at least one giant:

$$
\boxed{\Pr(\text{another evolved component}\mid\text{at least one giant})=\frac9{299}=0.0301003\ldots.}
$$

Thus **just over $3\%$ of giant-containing binaries have an evolved companion**. The $0.03\%$ numerator is a fraction of all binaries; it is not itself the requested conditional fraction.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

For [continuous-birth binary state fractions](../../../stellar-astrophysics.md#continuous-birth-binary-state-fractions), conditional mass [independence](../../../random-variable.md#independent-random-variables) and the common age give

$$
\begin{aligned}
\Pr(GG)&=\int_0^1\frac{y^2}{10000}dy=\frac1{30000},\\
\Pr(GW)&=\int_0^1\frac{2y^2}{2500}dy=\frac8{30000},\\
\Pr(WW)&=\int_0^1\frac{y^2}{625}dy=\frac{16}{30000}.
\end{aligned}
$$

The factor two in the middle expression allows either component to be the [red giant](../../../stellar-astrophysics.md#red-giant). Thus

$$
\boxed{\Pr(GG):\Pr(GW):\Pr(WW)=1:8:16.}
$$

Geometrically, the corresponding sections of the unit cube have areas proportional to $y^2$, so their volumes equal one third of their $y=1$ base areas. This is exactly the pyramid-volume calculation: the equal height and common factor $1/3$ leave the base-area ratio $1:8:16$ unchanged.

## 4

↑ **Parent:** [Paper 42](paper-42.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

**The elements have several complementary origins: primordial light nuclei, stellar and explosive fusion products, and nuclei built by neutron capture. Chemical enrichment also requires their ejection, rather than merely their production inside a star.** [Nucleosynthesis](../../../physics.md#nucleosynthesis) and transport into the [interstellar medium](../../../galaxy.md#interstellar-medium) must therefore be considered together.

[Hydrogen](../../../chemistry.md#hydrogen) and much of the [helium](../../../chemistry.md#helium) are primordial. During [Big Bang nucleosynthesis](../../../cosmology.md#big-bang-nucleosynthesis), a cooling, expanding plasma assembled surviving [neutrons](../../../physics.md#neutron) and [protons](../../../physics.md#proton) into [deuterium](../../../chemistry.md#deuterium), helium-3 and especially helium-4, with small abundances of lithium-7 or its beryllium-7 progenitor. Unstable nuclei at mass numbers five and eight, together with the rapidly falling density and short available time, obstructed sustained production of heavier nuclei. The [carbon](../../../chemistry.md#carbon), [oxygen](../../../chemistry.md#oxygen) and heavier material in later generations consequently require other sites. [Cosmic rays](../../../galaxy.md#cosmic-ray) fragment heavier interstellar nuclei and contribute importantly to the light elements lithium, beryllium and boron, which ordinary stellar burning tends to destroy.

**Burning stages depend on initial stellar mass.** [Stellar nuclear fusion](../../../stellar-astrophysics.md#stellar-nuclear-fusion) can release energy when the products have greater [nuclear binding energy](../../../physics.md#nuclear-binding-energy) than the reactants. The resulting [stellar thermostat](../../../stellar-astrophysics.md#stellar-thermostat) links nuclear burning to [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium): when fuel exhaustion lowers heating, contraction raises the central [temperature](../../../thermodynamics.md#temperature) until another fuel can ignite, if the core becomes hot enough. Higher nuclear charges bring larger [Coulomb barriers](../../../physics.md#coulomb-barrier), so later charged-particle burning generally requires progressively higher [temperatures](../../../thermodynamics.md#temperature). Whether the core reaches them depends on its mass, [electron degeneracy pressure](../../../statistical-physics.md#electron-degeneracy-pressure), mixing and envelope loss.

An approximately solar-composition $1M_\odot$ star first spends most of its life on the [main sequence](../../../stellar-astrophysics.md#main-sequence), converting [hydrogen](../../../chemistry.md#hydrogen) into [helium](../../../chemistry.md#helium) mainly through the [proton–proton chain](../../../stellar-astrophysics.md#proton-proton-chain). The net conversion is four protons into one helium-4 nucleus, with positrons and [neutrinos](../../../standard-model.md#neutrino); the small [CNO cycle](../../../stellar-astrophysics.md#cno-cycle) contribution redistributes CNO catalyst abundances but is not a net source of carbon at this stage. Exhaustion of central [hydrogen](../../../chemistry.md#hydrogen) leaves a helium-rich core. A surrounding [hydrogen-burning shell](../../../stellar-astrophysics.md#hydrogen-burning-shell) continues to add [helium](../../../chemistry.md#helium), while the core contracts and the envelope expands into a [red giant](../../../stellar-astrophysics.md#red-giant).

The low-mass helium core becomes supported substantially by [electron degeneracy pressure](../../../statistical-physics.md#electron-degeneracy-pressure). At roughly $10^8\,\mathrm K$, the [Triple-alpha process](../../../stellar-astrophysics.md#triple-alpha-process) ignites, first making transient beryllium-8 and then carbon-12 through the [Hoyle state](../../../stellar-astrophysics.md#hoyle-state). Because degeneracy initially weakens the usual expansion response, this ignition is a [helium flash](../../../stellar-astrophysics.md#helium-flash). It heats and lifts the degeneracy of the core, leading to a stable phase of [core helium burning](../../../stellar-astrophysics.md#core-helium-burning). The [Triple-alpha process](../../../stellar-astrophysics.md#triple-alpha-process) makes [carbon](../../../chemistry.md#carbon); competing [carbon-12 alpha capture](../../../physics.md#carbon-12-alpha-capture) makes [oxygen](../../../chemistry.md#oxygen):

$$
3\,{}^4\mathrm{He}\longrightarrow{}^{12}\mathrm C,\qquad
{}^{12}\mathrm C(\alpha,\gamma){}^{16}\mathrm O.
$$

After central [helium](../../../chemistry.md#helium) exhaustion, the star develops a carbon-oxygen core, a [helium-burning shell](../../../stellar-astrophysics.md#helium-burning-shell) and a more external [hydrogen-burning shell](../../../stellar-astrophysics.md#hydrogen-burning-shell). On the [Asymptotic giant branch](../../../stellar-astrophysics.md#asymptotic-giant-branch), recurrent [thermal pulses of an asymptotic-giant-branch star](../../../stellar-astrophysics.md#thermal-pulse-of-an-asymptotic-giant-branch-star) arise from unstable helium-shell burning. [Stellar dredge-up](../../../stellar-astrophysics.md#stellar-dredge-up) can bring processed material toward the surface, with its efficiency depending on mass and composition. The eventual [stellar wind](../../../stellar-astrophysics.md#stellar-wind) removes the envelope; the hot exposed core can illuminate a [planetary nebula](../../../stellar-astrophysics.md#planetary-nebula), and the remnant becomes a [carbon-oxygen white dwarf](../../../stellar-astrophysics.md#carbon-oxygen-white-dwarf). A usual isolated $1M_\odot$ star does not ignite [carbon burning](../../../stellar-astrophysics.md#carbon-burning). In particular, an element synthesized in its core need not all escape: much of the carbon and oxygen remains locked in the [white dwarf](../../../stellar-astrophysics.md#white-dwarf).

An approximately $5M_\odot$ star burns central [hydrogen](../../../chemistry.md#hydrogen) predominantly through the [CNO cycle](../../../stellar-astrophysics.md#cno-cycle), usually in a convective core. The CNO nuclei act as catalysts; the slow nitrogen-14 proton-capture step tends to accumulate nitrogen-14 while converting [hydrogen](../../../chemistry.md#hydrogen) into [helium](../../../chemistry.md#helium). After central fuel exhaustion, a [hydrogen-burning shell](../../../stellar-astrophysics.md#hydrogen-burning-shell) surrounds the contracting helium core. Unlike the $1M_\odot$ case, [core helium burning](../../../stellar-astrophysics.md#core-helium-burning) normally begins before strong electron degeneracy, without a classical [helium flash](../../../stellar-astrophysics.md#helium-flash). The same [Triple-alpha process](../../../stellar-astrophysics.md#triple-alpha-process) and [carbon-12 alpha capture](../../../physics.md#carbon-12-alpha-capture) create a carbon-oxygen core.

The $5M_\odot$ star then enters the [Asymptotic giant branch](../../../stellar-astrophysics.md#asymptotic-giant-branch), with hydrogen and helium burning in shells. Repeated thermal pulses and [stellar dredge-up](../../../stellar-astrophysics.md#stellar-dredge-up) can enrich its envelope with freshly made [carbon](../../../chemistry.md#carbon) and [s-process](../../../stellar-astrophysics.md#s-process) nuclei. [Hot-bottom burning](../../../stellar-astrophysics.md#hot-bottom-burning) can occur when the base of the convective envelope is sufficiently hot: the [CNO cycle](../../../stellar-astrophysics.md#cno-cycle) processes dredged-up carbon into [nitrogen](../../../chemistry.md#nitrogen), so a massive AGB star need not become carbon-rich despite making carbon below its envelope. Helium-shell reactions on neon-22 can also provide neutrons for the [s-process](../../../stellar-astrophysics.md#s-process). For an ordinary $5M_\odot$ model, strong envelope loss generally precedes carbon ignition, leaving a [carbon-oxygen white dwarf](../../../stellar-astrophysics.md#carbon-oxygen-white-dwarf). The exact threshold for carbon ignition and the size of these yields depend on [metallicity](../../../stellar-astrophysics.md#metallicity), mass loss and mixing; they are not universal integers fixed solely by initial mass.

A $20M_\odot$ star reaches much more advanced stages. It starts with convective-core [CNO cycle](../../../stellar-astrophysics.md#cno-cycle) [hydrogen burning](../../../stellar-astrophysics.md#hydrogen-burning), followed by [core helium burning](../../../stellar-astrophysics.md#core-helium-burning). After central [helium](../../../chemistry.md#helium) exhaustion, contraction can ignite [carbon burning](../../../stellar-astrophysics.md#carbon-burning) at temperatures approaching $10^9\,\mathrm K$. Carbon-fusion channels make products including [neon](../../../chemistry.md#neon), [sodium](../../../chemistry.md#sodium) and [magnesium](../../../chemistry.md#magnesium). [Neon burning](../../../stellar-astrophysics.md#neon-burning) then uses [photodisintegration](../../../physics.md#nuclear-photodisintegration) of neon-20 to release oxygen-16 and an [alpha particle](../../../physics.md#alpha-particle), followed by capture of that alpha particle on another neon-20 nucleus; the combined network releases energy and produces magnesium-24. [Oxygen burning](../../../stellar-astrophysics.md#oxygen-burning) makes silicon-group nuclei through channels such as

$$
{}^{16}\mathrm O+{}^{16}\mathrm O\longrightarrow{}^{28}\mathrm{Si}+\alpha.
$$

At still higher [temperature](../../../thermodynamics.md#temperature), [silicon burning](../../../stellar-astrophysics.md#silicon-burning) rearranges nuclei by [photodisintegration](../../../physics.md#nuclear-photodisintegration) and captures of protons, neutrons and [alpha particles](../../../physics.md#alpha-particle). It is not principally direct fusion of two silicon nuclei. Networks approach quasi-equilibrium and then [nuclear statistical equilibrium](../../../physics.md#nuclear-statistical-equilibrium), producing an iron-group core whose precise mixture depends on the [electron fraction in stellar matter](../../../physics.md#electron-fraction-in-stellar-matter). Outer shells retain different stages of burning, giving an approximately layered structure. Increasing [stellar neutrino energy loss](../../../stellar-structure.md#stellar-neutrino-energy-loss) makes advanced burning stages much shorter than [hydrogen burning](../../../stellar-astrophysics.md#hydrogen-burning).

Near the iron group, [nuclear binding energy](../../../physics.md#nuclear-binding-energy) per nucleon is close to its maximum. Further fusion cannot provide the sustained energy source required to support the core. As the core grows, [electron capture](../../../physics.md#electron-capture) reduces electron-pressure support and [photodisintegration](../../../physics.md#nuclear-photodisintegration) absorbs energy, assisting gravitational collapse. A successful [core-collapse supernova](../../../stellar-astrophysics.md#core-collapse-supernova) ejects some of the envelope and processed shells, and leaves a [neutron star](../../../stellar-astrophysics.md#neutron-star) or [black hole](../../../general-relativity.md#black-hole). The shock also causes explosive burning, changing the pre-existing abundances. A $20M_\odot$ initial mass does not uniquely fix the explosion or remnant: envelope loss, rotation, composition and fallback all matter, and some collapses fail to eject much material.

**Ejection determines the enrichment of the interstellar medium.** Low- and intermediate-mass stars return [helium](../../../chemistry.md#helium), CNO-processed matter, dredged-up [carbon](../../../chemistry.md#carbon) and [s-process](../../../stellar-astrophysics.md#s-process) products through [stellar winds](../../../stellar-astrophysics.md#stellar-wind) and envelope expulsion. Massive-star winds can expose hydrogen- or helium-burning products before collapse. Successful [core-collapse supernovae](../../../stellar-astrophysics.md#core-collapse-supernova) eject substantial oxygen and other alpha-capture products, together with some iron-group matter formed in hydrostatic and explosive burning. Material that falls back or remains in a [stellar remnant](../../../stellar-astrophysics.md#stellar-remnant) is withheld from the [interstellar medium](../../../galaxy.md#interstellar-medium). Subsequent mixing, cooling and star formation distribute the escaped material into new stars. The distinction between production and ejection is why an internal burning inventory alone is not a stellar yield.

[Binary stars](../../../stellar-astrophysics.md#binary-star) provide an additional major iron-group source. In a [Type Ia supernova](../../../stellar-astrophysics.md#type-ia-supernova), a carbon-oxygen [white dwarf](../../../stellar-astrophysics.md#white-dwarf) in a binary undergoes thermonuclear disruption after an appropriate accretion or merger history. Explosive carbon and oxygen burning makes intermediate-mass and iron-group nuclei. Much initially synthesized nickel-56 decays through cobalt-56 into iron-56; this [radioactive decay](../../../physics.md#radioactive-decay) also powers the [supernova](../../../stellar-astrophysics.md#supernova) light curve. Such explosions have delay times and yields different from those of massive-star collapse, and help explain why iron enrichment need not track oxygen enrichment exactly.

**Neutron capture builds much of the material beyond iron.** Charged-particle reactions encounter increasing [Coulomb barriers](../../../physics.md#coulomb-barrier) as nuclear charge grows, but a neutral [neutron](../../../physics.md#neutron) does not encounter that barrier. [Neutron capture](../../../physics.md#neutron-capture) raises mass number, and subsequent [beta-minus decay](../../../physics.md#beta-minus-decay) can turn a neutron into a proton and raise atomic number. The relative capture and decay times select different paths through the nuclear chart.

In the [slow neutron-capture process](../../../stellar-astrophysics.md#s-process), most unstable intermediates decay before the next capture, so the path stays near stable nuclei. In [Asymptotic giant branch](../../../stellar-astrophysics.md#asymptotic-giant-branch) stars, important neutron sources are

$$
{}^{13}\mathrm C(\alpha,n){}^{16}\mathrm O,\qquad
{}^{22}\mathrm{Ne}(\alpha,n){}^{25}\mathrm{Mg}.
$$

The carbon-13 source operates in suitable partially mixed layers, while the hotter helium-shell pulses can activate the neon-22 source. Captures on pre-existing seed nuclei produce elements such as strontium and barium and, under suitable conditions, lead. [Stellar dredge-up](../../../stellar-astrophysics.md#stellar-dredge-up) and [stellar winds](../../../stellar-astrophysics.md#stellar-wind) return these products to the [interstellar medium](../../../galaxy.md#interstellar-medium). Massive stars also have a weak [s-process](../../../stellar-astrophysics.md#s-process), notably using neon-22 during helium- and carbon-burning phases; it need not produce the same abundance range as the main AGB contribution.

In the [rapid neutron-capture process](../../../physics.md#r-process), very high neutron densities permit many captures before typical [beta-minus decays](../../../physics.md#beta-minus-decay). The path moves to neutron-rich nuclei, which later decay toward stability, producing heavy nuclei including lanthanides and actinides. Neutron-rich ejecta from [neutron star mergers](../../../stellar-astrophysics.md#neutron-star-merger) provide an established site: a merger can eject dynamical material and disk outflows, and [radioactive decay](../../../physics.md#radioactive-decay) of the newly made nuclei powers a [kilonova](../../../stellar-astrophysics.md#kilonova). Special neutron-rich outflows associated with some massive-star collapses are additional candidate sites. It would be unjustified to assume that every ordinary [core-collapse supernova](../../../stellar-astrophysics.md#core-collapse-supernova) produces the full heavy [r-process](../../../physics.md#r-process) pattern; the required neutron richness and expansion history are restrictive.

The two neutron-capture processes do not make every isotope beyond iron. Some proton-rich isotopes bypass their main paths. [Gamma-process nucleosynthesis](../../../physics.md#gamma-process-nucleosynthesis), for example, uses [photodisintegration](../../../physics.md#nuclear-photodisintegration) of pre-existing heavy seed nuclei in hot explosive material. Other proton-rich reaction paths can matter in suitable environments. Thus “heavier than iron” describes a family of production mechanisms rather than a single further ordinary fusion stage.

**Binaries change both stellar evolution and the delivery of elements.** [Roche-lobe overflow](../../../stellar-astrophysics.md#roche-lobe-overflow), wind transfer and mergers can strip a donor, rejuvenate a [mass-gaining star](../../../stellar-astrophysics.md#mass-gaining-star), alter core and envelope masses, and change the timing and character of an eventual explosion. Binary stripping can remove the hydrogen envelope of a massive [core-collapse supernova](../../../stellar-astrophysics.md#core-collapse-supernova) progenitor. Accretion onto a [white dwarf](../../../stellar-astrophysics.md#white-dwarf) can cause a [classical nova](../../../stellar-astrophysics.md#classical-nova), ejecting hydrogen-burning products and particular isotopes while ordinarily leaving the [white dwarf](../../../stellar-astrophysics.md#white-dwarf) intact; this differs from the destructive [Type Ia supernova](../../../stellar-astrophysics.md#type-ia-supernova). Compact [binary stars](../../../stellar-astrophysics.md#binary-star) can lose orbital energy through [gravitational radiation](../../../general-relativity.md#gravitational-wave) and merge, providing the [neutron star merger](../../../stellar-astrophysics.md#neutron-star-merger) route to heavy [r-process](../../../physics.md#r-process) material. Consequently chemical enrichment cannot be inferred entirely from isolated-star tracks, even when a simplified population calculation treats binary components as evolving independently.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
