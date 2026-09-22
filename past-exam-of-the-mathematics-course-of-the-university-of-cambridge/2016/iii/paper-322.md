# Paper 322

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_322.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_322.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 322](paper-322.md)

Let $T=10\,\mathrm{Gyr}$ and let $t$ denote present [stellar age](../../../stellar-astrophysics.md#stellar-age), rather than time measured from the galaxy's birth. With a fixed [initial mass function](../../../stellar-astrophysics.md#initial-mass-function), constant [star formation rate](../../../galaxy.md#star-formation-rate) also gives a constant number of births per unit time, as in the [birth-age distribution under constant star formation](../../../stellar-astrophysics.md#birth-age-distribution-under-constant-star-formation). Counting the supplied [stellar evolution](../../../stellar-astrophysics.md#stellar-evolution) model's remnants as part of the population, ages have a [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) on $[0,T]$. Integrating the constant birth rate therefore gives

$$
\boxed{Y(t)=\frac tT=0.1\frac{t}{\mathrm{Gyr}}\quad(0\le t\le T).}
$$

Outside this interval the cumulative fraction is zero or one as appropriate.

Write $m=M/M_\odot$ for the birth-mass parameter and $M_{\min}=0.2M_\odot$. The normalization cancels when integrating the [initial mass function](../../../stellar-astrophysics.md#initial-mass-function):

$$
X(M)=\frac{\int_M^\infty kM_\odot^3M'^{-3}\,dM'}{\int_{M_{\min}}^\infty kM_\odot^3M'^{-3}\,dM'}=\frac{M_{\min}^2}{M^2}.
$$

Thus **the mass-tail fraction** is

$$
\boxed{X(M)=\frac{0.04}{m^2}\quad(m>0.2).}
$$

It is one at and below the lower cutoff. The normalization constant has no effect on any number fraction.

For [evolutionary-state selection by stellar lifetimes](../../../stellar-astrophysics.md#evolutionary-state-selection-by-stellar-lifetimes), a [red giant](../../../stellar-astrophysics.md#red-giant) has completed its [main sequence](../../../stellar-astrophysics.md#main-sequence) lifetime but not its giant lifetime. Its [stellar lifetime regions in a mass-age diagram](../../../stellar-astrophysics.md#stellar-lifetime-regions-in-a-mass-age-diagram) are bounded by

$$
\boxed{\frac{8\,\mathrm{Gyr}}{m^2}<t<\frac{10\,\mathrm{Gyr}}{m^2},\qquad 0<t<T,\qquad m\ge0.2.}
$$

The lower boundary meets $t=T$ at $m=\sqrt{0.8}$ and the upper boundary meets it at $m=1$. A [white dwarf](../../../stellar-astrophysics.md#white-dwarf) lies above the upper lifetime curve, within the same age interval.

<a id="1/image-red-giant-and-white-dwarf-regions-in-the-birth-mass-age-plane-and-their-triangular-images-in-uniform-mass-tail-age-coordinates"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-322-population-regions.png)

**[Figure 1](#1/image-red-giant-and-white-dwarf-regions-in-the-birth-mass-age-plane-and-their-triangular-images-in-uniform-mass-tail-age-coordinates). Red-giant and white-dwarf regions in the birth-mass–age plane and their triangular images in uniform mass-tail–age coordinates**.

The [probability integral transform](../../../probability-theory.md#probability-integral-transform), applied to the decreasing mass-tail coordinate, makes $X$ uniform on $(0,1)$: $\Pr(X<x)=x$. The independent birth age gives $Y=t/T$ uniform on $(0,1)$, so number fractions are areas in a unit square. Since $m^{-2}=25X$, the [red giant](../../../stellar-astrophysics.md#red-giant) region becomes $20X<Y<25X$, a triangle with vertices $(0,0)$, $(1/25,1)$ and $(1/20,1)$. Its area is $\tfrac12(1/20-1/25)=1/200$. The [white dwarf](../../../stellar-astrophysics.md#white-dwarf) region $Y>25X$ is a triangle of area $\tfrac12(1/25)=1/50$. Hence **the present individual-star fractions** are

$$
\boxed{\Pr(G)=0.005=0.5\%,\qquad\Pr(W)=0.02=2\%.}
$$

The rest are on the [main sequence](../../../stellar-astrophysics.md#main-sequence) under the given toy lifetime model.

For the [binary stars](../../../stellar-astrophysics.md#binary-star), draw two independent mass-tail coordinates $X_1,X_2$, but only one shared age coordinate $Y$: components born together are coeval. The [coeval binary population](../../../stellar-astrophysics.md#coeval-binary-population) therefore occupies a uniform unit cube $(X_1,X_2,Y)$. At a fixed age $Y=y$, the state [probabilities](../../../probability-theory.md#probability) for either component are

$$
g(y)=\Pr(G\mid y)=\frac y{100},\qquad w(y)=\Pr(W\mid y)=\frac y{25}=4g(y),\qquad s(y)=1-\frac y{20}.
$$

Their evolutionary states have [conditional independence](../../../random-variable.md#conditional-independence) given $y$. They generally do not have unconditional independence, because sharing an age correlates their states. The binary fractions below are slice areas averaged over $0<y<1$.

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

At a fixed age, the [probability](../../../probability-theory.md#probability) that at least one component is a [red giant](../../../stellar-astrophysics.md#red-giant) is $1-(1-g)^2=2g-g^2$. Integrating over the common age in the [coeval binary population](../../../stellar-astrophysics.md#coeval-binary-population) gives

$$
\boxed{\Pr(\text{at least one }G)=\int_0^1\left(\frac{2y}{100}-\frac{y^2}{10000}\right)dy=\frac{299}{30000}=0.996\overline6\%.}
$$

This is **just under one percent of systems**. Squaring the marginal single-star fraction would incorrectly give two independently sampled component ages.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

For the [evolved-companion fraction](../../../stellar-astrophysics.md#conditional-evolved-companion-fraction-in-a-coeval-binary-population), a [red giant](../../../stellar-astrophysics.md#red-giant) has another evolved component precisely for unordered $GG$ or $GW$ pairs. By [conditional independence](../../../random-variable.md#conditional-independence) at fixed age, their combined slice [probability](../../../probability-theory.md#probability) is $g^2+2gw=9g^2$. Therefore

$$
\Pr(GG\text{ or }GW)=\int_0^1\frac{9y^2}{10000}\,dy=\frac9{30000}.
$$

Divide by the system fraction containing at least one [red giant](../../../stellar-astrophysics.md#red-giant) to obtain **the requested conditional fraction**:

$$
\boxed{\Pr(\text{another evolved component}\mid\text{at least one }G)=\frac9{299}\simeq3.01003\%.}
$$

A double-giant system is counted once in this denominator, and the factor two for a giant–[white dwarf](../../../stellar-astrophysics.md#white-dwarf) pair represents its two possible component orderings.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

For the three unordered evolved pairs, [conditional independence](../../../random-variable.md#conditional-independence) gives the slice [probabilities](../../../probability-theory.md#probability) $g^2$, $2gw=8g^2$ and $w^2=16g^2$. Averaging over the shared age in the [coeval binary population](../../../stellar-astrophysics.md#coeval-binary-population) yields

$$
\boxed{\Pr(GG)=\frac1{30000},\qquad\Pr(GW)=\frac8{30000},\qquad\Pr(WW)=\frac{16}{30000}.}
$$

Thus **their system-number ratio is $1:8:16$**, as required.

For the unheaded instantaneous-burst continuation, put $\tau=t/\mathrm{Gyr}$, with $0<\tau<10$. All [binary stars](../../../stellar-astrophysics.md#binary-star) now have the same age, so the individual [red giant](../../../stellar-astrophysics.md#red-giant) fraction is $g=\tau/1000$. Independent component masses give the [giant-pair fraction in an instantaneous stellar burst](../../../stellar-astrophysics.md#giant-pair-fraction-in-an-instantaneous-stellar-burst), **the two-giant system fraction**

$$
\boxed{\Pr_{\mathrm{burst}}(GG)=\left(\frac\tau{1000}\right)^2=10^{-6}\tau^2.}
$$

The final comparison has an ambiguity about which population is being counted. Taken literally as a comparison with the first galaxy's individual-star giant fraction $0.005$, it would require $\tau>\sqrt{5000}\simeq70.71$. **There is no allowed burst age**: throughout $0<\tau<10$, the two-giant fraction is less than $10^{-4}$, well below $0.005$.

If the intended comparison instead concerns two-giant systems in both galaxies, the comparison fraction is $1/30000$. Then $\tau^2/10^6>1/30000$ gives

$$
\boxed{\frac{10}{\sqrt3}\,\mathrm{Gyr}<t<10\,\mathrm{Gyr},\qquad\frac{10}{\sqrt3}\simeq5.7735.}
$$

For completeness, a comparison of individual [red giant](../../../stellar-astrophysics.md#red-giant) fractions in both galaxies would give $5\,\mathrm{Gyr}<t<10\,\mathrm{Gyr}$. These three comparisons have different denominators and should not be conflated.

## 2

↑ **Parent:** [Paper 322](paper-322.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use a [circular orbit](../../../classical-mechanics.md#circular-orbit), as in the stated [Roche lobe](../../../stellar-astrophysics.md#roche-lobe) approximation, with orbital angular speed $\Omega$ and negligible stellar spin. The [center of mass](../../../classical-mechanics.md#center-of-mass) distances are $a_1=aM_2/M$ and $a_2=aM_1/M$. Summing the two orbital [angular momenta](../../../classical-mechanics.md#angular-momentum) gives

$$
\boxed{J=(M_1a_1^2+M_2a_2^2)\Omega=\frac{M_1M_2}{M}a^2\Omega.}
$$

[Kepler's third law](../../../physics.md#kepler-s-third-law), $\Omega^2a^3=GM$, makes this $J=M_1M_2\sqrt{Ga/M}$. In [conservative mass transfer](../../../stellar-astrophysics.md#conservative-binary-mass-transfer), both $M$ and $J$ are fixed, while $dM_2=-dM_1$. Thus

$$
\frac{d\ln M_2}{d\ln M_1}=-q,\qquad \frac{d\ln a}{d\ln M_1}=2(q-1).
$$

The [Roche-lobe radius response exponent](../../../stellar-astrophysics.md#roche-lobe-radius-response-exponent) is consequently

$$
\zeta_L=\frac{d\ln R_L}{d\ln M_1}=2(q-1)+\frac13=2q-\frac53.
$$

During a dynamical mass-loss perturbation, the deep interior and [luminosity](../../../astrophysics.md#luminosity) do not have time to change. The supplied giant structure therefore has [stellar radius response exponent](../../../stellar-astrophysics.md#stellar-radius-response-exponent) $\zeta_*=-0.27$. Its fractional overfill changes by $d\ln(R/R_L)=(\zeta_*-\zeta_L)d\ln M_1$. The [binary mass ratio](../../../stellar-astrophysics.md#binary-mass-ratio) uses donor mass divided by accretor mass. Since $d\ln M_1<0$, self-limiting [Roche-lobe overflow](../../../stellar-astrophysics.md#roche-lobe-overflow) requires $\zeta_*>\zeta_L$. Hence **the dynamical stability condition** is

$$
\boxed{q<q_{\mathrm{crit}}=\frac{5/3-0.27}{2}=0.698\overline3\simeq0.7.}
$$

At equality the linear restoring response vanishes. This [conservative mass-transfer critical mass ratio](../../../stellar-astrophysics.md#conservative-mass-transfer-critical-mass-ratio) uses the given radius exponent, rather than imposing the different fully convective $-1/3$ approximation.

The initially more massive component normally evolves first. If it first overflowed only after acquiring the given giant response, it would have $q>1$ and the mass loss would be dynamically unstable: its radius grows while its [Roche lobe](../../../stellar-astrophysics.md#roche-lobe) initially contracts. Starting overflow earlier can avoid this outcome. A [main sequence](../../../stellar-astrophysics.md#main-sequence) or early post-main-sequence [donor star](../../../stellar-astrophysics.md#donor-star) can have a radiative envelope with a stabilizing contraction response. Transfer then reverses the [binary mass ratio](../../../stellar-astrophysics.md#binary-mass-ratio) before the donor develops the giant structure. This is the route to an [Algol binary](../../../stellar-astrophysics.md#algol-binary) through [Case A mass transfer](../../../stellar-astrophysics.md#case-a-mass-transfer) during core hydrogen burning, or [early case B mass transfer](../../../stellar-astrophysics.md#early-case-b-mass-transfer) after core hydrogen exhaustion but before a deep giant envelope develops.

For the initial [Roche-lobe overflow](../../../stellar-astrophysics.md#roche-lobe-overflow) to occur before the base of the giant branch, its lobe must be smaller than the base-of-branch stellar radius. Combining $R_L=0.462a(M_1/M)^{1/3}$ with [Kepler's third law](../../../physics.md#kepler-s-third-law) cancels the companion dependence:

$$
P_i<2\pi\left[\frac{R_{\mathrm{BGB}}^3}{0.462^3GM_1}\right]^{1/2}.
$$

Writing $m_1=M_1/M_\odot$, substitute the [mass-radius relation](../../../exoplanet.md#mass-radius-relation) to obtain **the pre-giant period limit**:

$$
\boxed{P_i<P_0m_1^2,\qquad P_0=2\pi\left[\frac{(1.68/0.462)^3R_\odot^3}{GM_\odot}\right]^{1/2}\simeq0.803\,\mathrm{days}.}
$$

We use the specified $0.8\,\mathrm{days}$ below. This is a [pre-giant Roche-lobe-filling period limit](../../../stellar-astrophysics.md#pre-giant-roche-lobe-filling-period-limit), not a condition on the current stripped donor's radius.

At fixed total mass, [Kepler's third law](../../../physics.md#kepler-s-third-law) gives $P\propto a^{3/2}$, while fixed orbital [angular momentum](../../../classical-mechanics.md#angular-momentum) gives $a\propto(M_1M_2)^{-2}$. Therefore **the conservative period invariant** is

$$
\boxed{P(M_1M_2)^3=\text{constant}.}
$$

To find the smallest possible pre-giant period ratio, use solar-unit masses $m_1,m_2$ and fixed $m=m_1+m_2$. Let $K=P(m_1m_2)^3$. Along this [period-product invariant for conservative mass transfer](../../../stellar-astrophysics.md#period-product-invariant-for-conservative-mass-transfer),

$$
F(m_1)=\frac{P}{m_1^2}=\frac K{m_1^5(m-m_1)^3}.
$$

The denominator has logarithmic derivative $5/m_1-3/(m-m_1)$, with a strictly negative derivative of its own. Its unique maximum, hence the unique minimum of $F$, occurs at

$$
\boxed{m_1=\frac58m,\qquad m_2=\frac38m.}
$$

Since $F$ diverges at either endpoint, this is the global [minimum period-to-donor-mass ratio for conservative evolution](../../../stellar-astrophysics.md#minimum-period-to-donor-mass-ratio-for-conservative-evolution).

For the quoted [Algol binary](../../../stellar-astrophysics.md#algol-binary), $K=3(1\times3)^3=81\,\mathrm{days}$ and $m=4$. Choosing the minimizing progenitor gives $m_{1,i}=2.5$, $m_{2,i}=1.5$ and

$$
P_i=\frac{81}{(2.5\times1.5)^3}=1.536\,\mathrm{days},\qquad F_{\min}=0.24576\,\mathrm{days}<0.8\,\mathrm{days}.
$$

Its pre-giant upper limit is $0.8(2.5)^2=5\,\mathrm{days}$, comfortably above this initial period. Subsequent [conservative mass transfer](../../../stellar-astrophysics.md#conservative-binary-mass-transfer) of $1.5M_\odot$ produces the stated masses and period. Thus **the data permit the proposed early-overflow formation route**.

For [RT Lac](../../../stellar-astrophysics.md#rt-lac), instead $K=5(0.5\times1.5)^3=2.109375\,\mathrm{days}$ and $m=2$. At its most favorable conservative progenitor, $m_{1,i}=1.25$, $m_{2,i}=0.75$ and

$$
P_i=2.56\,\mathrm{days},\qquad F_{\min}=1.6384\,\mathrm{days}>0.8\,\mathrm{days}.
$$

**No conservative progenitor meets the pre-giant overflow condition.** An initially more massive giant donor also fails the dynamical-stability condition derived above. Within this stable Algol-type formation model, the current RT Lac system therefore requires [nonconservative mass transfer](../../../stellar-astrophysics.md#nonconservative-binary-mass-transfer).

A plausible history is substantial envelope loss from the system, through a [stellar wind](../../../stellar-astrophysics.md#stellar-wind) or escaping overflow, possibly with a [common envelope](../../../stellar-astrophysics.md#common-envelope) episode. Escaping matter also carries orbital [angular momentum](../../../classical-mechanics.md#angular-momentum), so the total-mass and period-product invariants no longer constrain its initial orbit. A more massive progenitor can then shed its envelope and reach the present low donor mass without requiring the excluded conservative sequence. The supplied final data do not determine a unique mass-loss or angular-momentum-loss history.

## 3

↑ **Parent:** [Paper 322](paper-322.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For constant component masses, the [center of mass](../../../classical-mechanics.md#center-of-mass) frame has $\mathbf r_1=(M_2/M)\mathbf r$ and $\mathbf r_2=-(M_1/M)\mathbf r$. [Newton's law of universal gravitation](../../../classical-mechanics.md#newton-s-law-of-universal-gravitation) gives the relative equation $\ddot{\mathbf r}=-GM\mathbf r/r^3$. Substitution in the component [angular momenta](../../../classical-mechanics.md#angular-momentum) yields

$$
\boxed{\mathbf J=\mu\mathbf h=\mu\mathbf r\times\dot{\mathbf r},\qquad\dot{\mathbf h}=\mathbf r\times\ddot{\mathbf r}=0.}
$$

Here $\mu=M_1M_2/M$ is the [reduced mass](../../../classical-mechanics.md#reduced-mass), while $\mathbf h$ is [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum).

The printed total-energy expression lacks a factor of $\mu$ in its kinetic term. With the stated physical separation coordinate, the dimensionally consistent total [two-body orbital energy](../../../classical-mechanics.md#two-body-orbital-energy) is

$$
\boxed{E=\frac\mu2|\dot{\mathbf r}|^2-\frac{GM\mu}{r}=\mu\varepsilon,\qquad\varepsilon=\frac12|\dot{\mathbf r}|^2-\frac{GM}{r}.}
$$

The second expression is [specific orbital energy](../../../classical-mechanics.md#specific-orbital-energy); these two conventions must not be mixed. Its conservation follows directly:

$$
\dot E=\mu\dot{\mathbf r}\cdot\left(\ddot{\mathbf r}+\frac{GM\mathbf r}{r^3}\right)=0.
$$

For the [eccentricity vector](../../../classical-mechanics.md#eccentricity-vector), differentiate $GM\mathbf e=\dot{\mathbf r}\times\mathbf h-GM\widehat{\mathbf r}$. Since $\mathbf h$ is constant,

$$
GM\dot{\mathbf e}=-\frac{GM}{r^3}\mathbf r\times(\mathbf r\times\dot{\mathbf r})-GM\left[\frac{\dot{\mathbf r}}r-\frac{\mathbf r(\mathbf r\cdot\dot{\mathbf r})}{r^3}\right]=0.
$$

The cancellation is the [vector triple product identity](../../../calculus.md#vector-triple-product). Thus **all three corrected Kepler integrals are conserved**. Dotting the eccentricity relation with $\mathbf r$ also gives the useful orbit identity

$$
\boxed{\mathbf e\cdot\mathbf r=\frac{h^2}{GM}-r.}
$$

For [ballistic streamline focusing by a moving star](../../../astrophysics.md#ballistic-streamline-focusing-by-a-moving-star), work in the star's rest frame and take the incoming gas to have velocity $v\mathbf e_x$, with downstream behind the star at $x>0$. A streamline with [impact parameter](../../../classical-mechanics.md#impact-parameter) $d>0$ approaches from $(-\infty,d,0)$. Its upstream [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum) and [eccentricity vector](../../../classical-mechanics.md#eccentricity-vector) are

$$
\mathbf h=-dv\mathbf e_z,\qquad\mathbf e=\mathbf e_x+\frac{dv^2}{GM}\mathbf e_y.
$$

At its downstream axis crossing, $\mathbf r=b\mathbf e_x$. The orbit identity gives $b=d^2v^2/(GM)-b$, hence **the collision distance** is

$$
\boxed{b=\frac{d^2v^2}{2GM}.}
$$

At that point, $h_z=b u_y=-dv$, while the $y$ component of $GM\mathbf e=\mathbf u\times\mathbf h-GM\widehat{\mathbf r}$ gives $dv\,u_x=dv^2$. Therefore

$$
\mathbf u=v\mathbf e_x-\frac{2GM}{dv}\mathbf e_y.
$$

A symmetric streamline with opposite impact parameter has the opposite transverse velocity. Their [shock wave](../../../partial-differential-equation.md#shock-wave) removes the opposing transverse motion while preserving the common downstream component. Thus **the remaining velocity is $v\mathbf e_x$ in the star frame**. In the frame where the undisturbed medium is stationary, adding the star's velocity gives zero velocity immediately after this idealized collision.

After transverse [kinetic energy](../../../classical-mechanics.md#kinetic-energy) is dissipated, the remaining [specific orbital energy](../../../classical-mechanics.md#specific-orbital-energy) is $\varepsilon_{\rm after}=v^2/2-GM/b$. It is negative if $b<2GM/v^2$, or equivalently if the upstream [impact parameter](../../../classical-mechanics.md#impact-parameter) satisfies $d<d_{\rm cap}=2GM/v^2$. This is the [post-shock capture criterion in ballistic accretion](../../../astrophysics.md#post-shock-capture-criterion-in-ballistic-accretion); bound axial streams can return to the star. The captured incident [mass flux](../../../physics.md#mass-flux) through the corresponding disk gives the ballistic [Bondi--Hoyle--Lyttleton accretion rate](../../../astrophysics.md#bondi-hoyle-lyttleton-accretion-rate):

$$
\boxed{\dot M=\pi d_{\rm cap}^2\rho v=\frac{4\pi(GM)^2\rho}{v^3}.}
$$

This is the pressureless, dissipative capture model, with the shock's transverse energy unavailable to unbind the wake.

For [wind mass transfer in a binary star](../../../stellar-astrophysics.md#wind-mass-transfer-in-a-binary-star), steady isotropic donor mass loss gives the local wind [mass density](../../../fluid-mechanics.md#density) at the companion:

$$
\rho_w(a)=\frac{-\dot M_1}{4\pi a^2v_w}.
$$

A fast wind has $v_w\gg2\pi a/P$ and a capture scale small compared with $a$, so its relative incident speed is $v_w$ to leading order. Apply the same [Bondi--Hoyle--Lyttleton accretion rate](../../../astrophysics.md#bondi-hoyle-lyttleton-accretion-rate) with accretor mass $M_2$ to obtain

$$
\boxed{\dot M_{2,\rm acc}=(-\dot M_1)\frac{G^2M_2^2}{a^2v_w^4}.}
$$

Finally, [Kepler's third law](../../../physics.md#kepler-s-third-law) eliminates the unquoted separation, $a=[G(M_1+M_2)P^2/(4\pi^2)]^{1/3}$, giving **the rate in terms of the stated [orbital period](../../../classical-mechanics.md#orbital-period)**:

$$
\boxed{\dot M_{2,\rm acc}=(-\dot M_1)\frac{(2\pi G/P)^{4/3}M_2^2}{(M_1+M_2)^{2/3}v_w^4}.}
$$

Equivalently, the [fast-wind accretion fraction in a circular binary](../../../stellar-astrophysics.md#fast-wind-accretion-fraction-in-a-circular-binary) is $[M_2/(M_1+M_2)]^2(v_{\rm orb}/v_w)^4$, with $v_{\rm orb}=2\pi a/P$ the relative circular orbital speed. Its smallness is consistent with using an almost undisturbed isotropic [stellar wind](../../../stellar-astrophysics.md#stellar-wind).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
