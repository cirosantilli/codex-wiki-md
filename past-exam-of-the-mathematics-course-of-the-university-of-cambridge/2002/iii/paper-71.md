# Paper 71

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper71.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper71.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
- [7](#7)
  - [a](#7/a)
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)

## 1

↑ **Parent:** [Paper 71](paper-71.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A [photon](../../../quantum-mechanics.md#photon) loses [energy](../../../classical-mechanics.md#energy) by $1+z=a_0/a_e$ between emission and reception. The interval between successive [photon](../../../quantum-mechanics.md#photon) arrivals is also longer by $1+z$, so the received [energy](../../../classical-mechanics.md#energy) per unit time is reduced by $(1+z)^2$. An isotropic wavefront at reception has area $4\pi(a_0r)^2$: the astronomical radial coordinate is an areal coordinate, even in curved space. Hence

$$
F=\frac{L}{4\pi(a_0r)^2(1+z)^2},\qquad\boxed{d_L\equiv\sqrt{\frac{L}{4\pi F}}=a_0r(1+z).}
$$

This defines the [luminosity distance](../../../cosmology.md#luminosity-distance). [Photon](../../../quantum-mechanics.md#photon) absorption or conversion would require a further transmission factor; the relation assumes freely propagating conserved [photons](../../../quantum-mechanics.md#photon) and bolometric [luminosity](../../../astrophysics.md#luminosity). The radial [cosmological proper distance](../../../cosmology.md#proper-distance-in-cosmology) is generally different from the areal distance $a_0r$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Take zero [cosmological constant](../../../cosmology.md#cosmological-constant) and an open geometry, which means $k<0$ in the metric convention. Evaluating the [Friedmann equations](../../../cosmology.md#friedmann-equations) today gives $H_0^2=H_0^2\Omega_0-k/a_0^2$, so

$$
\boxed{-k=a_0^2H_0^2(1-\Omega_0)},\qquad 0<\Omega_0<1.
$$

On a constant-time slice the radial line element is $d\ell=a_0dr/\sqrt{1-kr^2}$. Therefore

$$
d_S=a_0\int_0^r\frac{dr'}{\sqrt{1+(-k)r'^2}}=\boxed{\frac{\operatorname{arsinh}[a_0H_0\sqrt{1-\Omega_0}\,r]}{H_0\sqrt{1-\Omega_0}}}.
$$

This is a [cosmological proper distance](../../../cosmology.md#proper-distance-in-cosmology) on today's slice, not the distance traveled during the [photon](../../../quantum-mechanics.md#photon) flight. The printed condition $k<1$ is insufficient to specify an open model; the derivation uses its intended $k<0$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For radial null propagation, $dr/\sqrt{1-kr^2}=|dt|/a$. Since $dz/dt=-(1+z)H(z)$ and $a=a_0/(1+z)$, its present-distance integral is

$$
\boxed{d_S=a_0\int_{t_e}^{t_0}\frac{dt}{a(t)}=\int_0^z\frac{dz'}{H(z')}}.
$$

Thus the printed extra $a_0$ before the [redshift](../../../optics.md#redshift) integral is inappropriate when $H$ is the physical [Hubble parameter](../../../cosmology.md#hubble-parameter); it disappears only if $a_0$ has been set to one.

Dust conservation and the [curvature](../../../differential-geometry.md#curvature) relation give

$$
H^2(z)=H_0^2[\Omega_0(1+z)^3+(1-\Omega_0)(1+z)^2],\qquad d_S=\frac1{H_0}\int_0^z\frac{dz'}{(1+z')\sqrt{1+\Omega_0z'}}.
$$

To evaluate it, put $s=\sqrt{1-\Omega_0}$ and $v=\sqrt{1+\Omega_0z}$. The dimensionless integral $I=H_0d_S$ is

$$
I=2\int_1^v\frac{dv'}{v'^2-s^2}=\frac1s\log\left[\frac{v-s}{v+s}\frac{1+s}{1-s}\right].
$$

Inverting the proper-distance expression in part b gives $r=\sinh(sI)/(a_0H_0s)$. Substituting the logarithm, writing the [hyperbolic sine](../../../calculus.md#hyperbolic-sine) as half the difference of its exponential and inverse, and using $v^2-s^2=\Omega_0(1+z)$ yields

$$
\boxed{r(z)=\frac2{a_0H_0}\frac{\Omega_0z+(2-\Omega_0)[1-\sqrt{1+\Omega_0z}]}{\Omega_0^2(1+z)}}.
$$

This is the [open dust distance-redshift relation](../../../cosmology.md#open-dust-distance-redshift-relation). The printed square root lacks the factor $z$; its literal form would give a negative, nonzero coordinate at $z=0$. The corrected expression has $r\sim z/(a_0H_0)$ near zero. At fixed positive $\Omega_0$ and $z\gg\Omega_0^{-1}$, the term linear in $z$ dominates, giving

$$
\boxed{r\longrightarrow\frac2{a_0H_0\Omega_0}}.
$$

The zero-density limit is nonuniform: a pure Milne model has no such finite limiting radial coordinate.

## 2

↑ **Parent:** [Paper 71](paper-71.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use radiation-era $H=C_*T^2/m_{\rm pl}$, with $C_*=1.66\sqrt{g_*}$. The stipulated interaction rate is $\alpha_Y^4T^5/m_Y^4$, not $\alpha_Y^2T^5/m_Y^4$. Decoupling therefore gives

$$
T_D^3=\frac{C_*m_Y^4}{\alpha_Y^4m_{\rm pl}},\quad\boxed{m_{Y\rm nr}=\frac{\alpha_Y^4m_{\rm pl}}{C_*}\simeq7\times10^5\ {\rm GeV}},\quad T_D=m_Y\left(\frac{m_Y}{m_{Y\rm nr}}\right)^{1/3}.
$$

At the threshold $T_D=m_{Y\rm nr}$, the assumed $g_*\simeq100$ is self-consistent with the stated high-temperature condition. Smaller masses decouple nonrelativistically, with $x_D=m_Y/T_D=(m_{Y\rm nr}/m_Y)^{1/3}\gg1$.

For an [thermal equilibrium](../../../thermodynamics.md#thermal-equilibrium) species with zero [chemical potential](../../../thermodynamics.md#chemical-potential), $n_Y=2(m_YT_D/2\pi)^{3/2}e^{-x_D}$, while $s=2\pi^2g_{*s}T_D^3/45$. Thus

$$
\frac{n_Y}{s}=\frac{45g_Y}{2\pi^2g_{*s}(2\pi)^{3/2}}x_D^{3/2}e^{-x_D}\simeq\boxed{10^{-3}\left(\frac{m_{Y\rm nr}}{m_Y}\right)^{1/2}e^{-(m_{Y\rm nr}/m_Y)^{1/3}}}.
$$

The numerical coefficient before rounding is about $2.9\times10^{-3}$ for $g_Y=2$ and $g_{*s}=100$. This is [mass-dependent fermion freeze-out](../../../cosmology.md#mass-dependent-fermion-freeze-out). It assumes the rate maintains [chemical equilibrium](../../../thermodynamics.md#chemical-equilibrium) until sudden [cosmological particle freeze-out](../../../cosmology.md#cosmological-particle-freeze-out) and that entropy is conserved afterwards. Elastic scattering alone would not justify the [thermal equilibrium](../../../thermodynamics.md#thermal-equilibrium) number-density estimate. For decoupling below the high-temperature range, changes in effective degrees of freedom modify the numerical estimate; the requested formula treats them as roughly constant.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

In the specified dust model $H_0=2/(3t_0)$, so $\rho_{\rm crit}=m_{\rm pl}^2/(6\pi t_0^2)$ and $n_B=\Omega_{B0}\rho_{\rm crit}/m_B$. [Photons](../../../quantum-mechanics.md#photon) and the six [neutrino](../../../standard-model.md#neutrino)/[antineutrino](../../../standard-model.md#antineutrino) helicity states give

$$
g_{*s,0}=2+\frac78\,6\left(\frac{T_\nu}{T_\gamma}\right)^3=\frac{43}{11},\qquad s_0=\frac{2\pi^2}{45}\frac{43}{11}T_\gamma^3.
$$

Using the supplied GeV estimates literally gives

$$
\boxed{Y_B\equiv\frac{n_B}{s}\simeq4.5\times10^{-12}}.
$$

The rounded time/[temperature](../../../thermodynamics.md#temperature) conversions are unusually crude: converting $10$ Gyr to $4.8\times10^{41}\ {\rm GeV}^{-1}$ and $3$ K to $2.6\times10^{-13}$ GeV instead gives $Y_B\sim10^{-10}$. Either set gives the same order-of-magnitude [mass](../../../classical-mechanics.md#mass) conclusion below, but the numerical abundance should identify which supplied units are used.

For a stable relic, the relevant comparison is [energy](../../../classical-mechanics.md#energy) [density](../../../fluid-mechanics.md#density), not merely particle number. The matter [density](../../../fluid-mechanics.md#density) left over after the [baryons](../../../physics.md#baryon) is at most nine times the [baryon](../../../physics.md#baryon) [density](../../../fluid-mechanics.md#density) here. Consequently

$$
\boxed{m_YY_Y\lesssim9m_BY_B},\qquad Y_Y=n_Y/s.
$$

Put $x=(m_{Y\rm nr}/m_Y)^{1/3}$ and use $Y_Y\simeq C_Yx^{3/2}e^{-x}$ with $C_Y\simeq10^{-3}$. The condition becomes

$$
x+\frac32\log x\gtrsim\log\left(\frac{C_Ym_{Y\rm nr}}{9m_BY_B}\right).
$$

For the literal supplied numbers the right side is about $30.5$, giving $x\gtrsim25.6$ and $m_Y\lesssim40$–$50$ GeV. With the physically consistent conversions the estimate is about $60$ GeV. The intended rough conclusion is therefore **a sufficiently suppressed branch with $m_Y$ no larger than order $10^2$ GeV**, within the toy [cosmological particle freeze-out](../../../cosmology.md#cosmological-particle-freeze-out) law. Comparing the two number yields alone gives a similar rough scale but misses the [mass](../../../classical-mechanics.md#mass) weighting. This is a [thermal relic density bound for a tunable fermion](../../../cosmology.md#thermal-relic-density-bound-for-a-tunable-fermion).

For $m_Y\gtrsim m_{Y\rm nr}$, relativistic decoupling would instead leave $Y_Y\simeq135\zeta(3)g_Y/(8\pi^4g_{*s})\simeq4\times10^{-3}$, incompatible with the matter-density bound for such heavy stable particles. These are conditional bounds on a populated, stable [thermal relic](../../../cosmology.md#thermal-relic). A short lifetime or an initially suppressed nonthermal population can change the conclusion; the supplied information alone does not constrain every possible production and decay history.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Above the transition,

$$
\frac{\Gamma_{\rm int}}H=\frac{\alpha_Y^2m_{\rm pl}}{1.66\sqrt{g_*}\,T}=\frac{T_{\rm eq}}T,\qquad\boxed{T_{\rm eq}\sim7\times10^{11}\ {\rm GeV}}
$$

for $g_*\sim100$. The ratio increases during cooling, rather than at higher [temperature](../../../thermodynamics.md#temperature). A GUT transition at $T_c\sim10^{15}$–$10^{16}$ GeV occurs well above this scale, so the interaction is too slow to establish or maintain [thermal equilibrium](../../../thermodynamics.md#thermal-equilibrium) throughout $T>T_c$. In fact its integrated interaction probability from an arbitrarily high [temperature](../../../thermodynamics.md#temperature) down to $T_c$ is at most of order $T_{\rm eq}/T_c\ll1$, since $dt=-dT/(HT)$.

An initial [Fermi-Dirac distribution](../../../statistical-physics.md#fermi-dirac-distribution) with zero [chemical potential](../../../thermodynamics.md#chemical-potential) therefore cannot be assumed from this high-temperature rate alone. If imposed initially and collisionlessly redshifted while the particles are massless, its thermal-looking form can persist, but this is not dynamically maintained [thermal equilibrium](../../../thermodynamics.md#thermal-equilibrium). Other initial states can remain nonthermal. This is the [thermalization temperature for a massless gauge mediator](../../../cosmology.md#thermalization-temperature-for-a-massless-gauge-mediator).

The below-transition rate stipulated in the model has $\Gamma/H=(T/T_D)^3$. If $T_c\gg T_D$ and it includes efficient number-changing reactions, it can restore [chemical equilibrium](../../../thermodynamics.md#chemical-equilibrium) after the transition and erase the initial-state memory, making the estimates in a and b applicable. If it only equilibrates momenta, or if [reheating](../../../cosmic-inflation.md#reheating) never populates the relevant range, the [thermal relic](../../../cosmology.md#thermal-relic) calculation must be reconsidered.

## 3

↑ **Parent:** [Paper 71](paper-71.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Separate conservation of a fluid with fixed $w=P/\rho$ gives $\dot\rho+3H(1+w)\rho=0$, hence $\rho\propto a^{-3(1+w)}$. The $w=-1/3$ component therefore has $\rho_Q\propto a^{-2}$. Flatness today fixes its normalization to $\rho_{Q0}=3H_0^2(1-\Omega_{M0})/(8\pi G)$, so

$$
\boxed{\rho_Q(a)=\frac{3H_0^2(1-\Omega_{M0})}{8\pi Ga^2}}.
$$

This is a [coasting fluid](../../../cosmology.md#coasting-fluid): its contribution to $\rho+3P$ is zero, so it does not itself drive accelerated expansion. Its background Friedmann contribution resembles [curvature](../../../differential-geometry.md#curvature), although the actual spatial geometry remains flat.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write $\Omega=\Omega_{M0}$, $\beta^2=H_0^2(1-\Omega)$ and $\mathcal H=a'/a=\dot a$. The Friedmann equation is

$$
\mathcal H^2=H_0^2\left(\frac\Omega a+1-\Omega\right).
$$

The [Raychaudhuri equation](../../../cosmology.md#friedmann-acceleration-equation) has only the matter component on its active-gravity side, so

$$
\mathcal H'=a\ddot a=-\frac{4\pi G}{3}a^2\rho_M=-\frac{H_0^2\Omega}{2a}.
$$

Combining these expressions proves

$$
\boxed{2\mathcal H'+\mathcal H^2-\beta^2=0}.
$$

This is the [conformal Riccati equation for matter and a coasting fluid](../../../cosmology.md#conformal-riccati-equation-for-matter-and-a-coasting-fluid). The prime denotes [conformal time](../../../cosmology.md#conformal-time), whereas $H_0$ is the physical present [Hubble parameter](../../../cosmology.md#hubble-parameter).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Choose the [Big Bang](../../../cosmology.md#big-bang) at $\tau=t=0$. For $0<\Omega<1$, the expanding singular solution of the Riccati equation is $\mathcal H=\beta\coth(\beta\tau/2)$. Integrating $a'/a=\mathcal H$ gives $a=C\sinh^2(\beta\tau/2)$. The Friedmann constraint fixes $C=\Omega/(1-\Omega)$, rather than leaving an independent amplitude. Thus

$$
\boxed{a(\tau)=\frac\Omega{2(1-\Omega)}[\cosh(\beta\tau)-1]}.
$$

Now $dt=a\,d\tau$. Integrating from the singular origin gives

$$
\boxed{t(\tau)=\frac{H_0^{-1}\Omega}{2(1-\Omega)^{3/2}}[\sinh(\beta\tau)-\beta\tau]}.
$$

This derives the [flat matter-coasting-fluid Friedmann solution](../../../cosmology.md#flat-matter-coasting-fluid-friedmann-solution). For small $\tau$, $a\propto\tau^2$ and $t\propto\tau^3$, hence $a\propto t^{2/3}$. At late time $a\propto t$, as expected when the [coasting fluid](../../../cosmology.md#coasting-fluid) dominates.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Set $a=1$ in the parametric solution. With $b=1-\Omega$,

$$
\beta\tau_0=2\operatorname{arsinh}\sqrt{\frac b\Omega},\qquad\sinh(\beta\tau_0)=\frac{2\sqrt b}{\Omega}.
$$

Consequently

$$
\boxed{H_0t_0=\frac1b-\frac\Omega{b^{3/2}}\operatorname{arsinh}\sqrt{\frac b\Omega}}.
$$

The endpoint values are obtained by limits. A particularly direct proof of the age bound avoids subtracting nearly equal terms: from the Friedmann equation,

$$
H_0t_0=\int_0^1\frac{\sqrt a\,da}{\sqrt{\Omega+(1-\Omega)a}}.
$$

For nonnegative component densities, $0\le\Omega\le1$ and $a\le\Omega+(1-\Omega)a\le1$. The integrand lies between $\sqrt a$ and $1$. Integrating therefore gives

$$
\boxed{\frac23H_0^{-1}\le t_0\le H_0^{-1}}.
$$

Equality holds for pure matter and pure [coasting fluid](../../../cosmology.md#coasting-fluid), respectively. These are the [age of a flat matter-coasting-fluid universe](../../../cosmology.md#age-of-a-flat-matter-coasting-fluid-universe) and the [coasting-fluid age bound](../../../cosmology.md#coasting-fluid-age-bound); the positivity range is necessary for the stated universal inequality.

## 4

↑ **Parent:** [Paper 71](paper-71.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For a homogeneous canonical scalar, $\rho_\phi=\dot\phi^2/2+V$ and $P_\phi=\dot\phi^2/2-V$. The acceleration equation requires $V>\dot\phi^2$ for [cosmic inflation](../../../cosmic-inflation.md), equivalently $\epsilon_H=-\dot H/H^2<1$ in the flat scalar-dominated limit. Inflation need not be exactly de Sitter.

A standard sufficient regime for a long period is positive [potential energy](../../../classical-mechanics.md#potential-energy) dominating the [kinetic energy](../../../classical-mechanics.md#kinetic-energy), physical [gradient](../../../calculus.md#gradient) [energy](../../../classical-mechanics.md#energy) and [curvature](../../../differential-geometry.md#curvature). Homogeneity over an expanding approximately Hubble-sized patch allows the [gradient](../../../calculus.md#gradient) term to [redshift](../../../optics.md#redshift) away. In comoving coordinates the [gradient](../../../calculus.md#gradient) [energy](../../../classical-mechanics.md#energy) is $|\nabla_{\rm com}\phi|^2/(2a^2)$; the [gradient](../../../calculus.md#gradient) in the displayed [energy](../../../classical-mechanics.md#energy) formula must be interpreted physically if no $a^{-2}$ is written there. Require

$$
\frac{\dot\phi^2}{2}\ll V,\quad\frac{|\nabla_{\rm com}\phi|^2}{2a^2}\ll V,\quad\frac{|k|}{a^2}\ll\frac{8\pi V}{3m_{\rm pl}^2},\quad|\ddot\phi|\ll3H|\dot\phi|.
$$

The slow-roll equations are then $3H\dot\phi\simeq-V'$ and $H^2\simeq8\pi V/(3m_{\rm pl}^2)$. Sufficient potential conditions are

$$
\epsilon_V=\frac{m_{\rm pl}^2}{16\pi}\left(\frac{V'}V\right)^2\ll1,\qquad |\eta_V|=\left|\frac{m_{\rm pl}^2}{8\pi}\frac{V''}V\right|\ll1.
$$

The potential must remain sufficiently flat over a large enough field interval to produce the required expansion. These slow-roll conditions are stronger than the bare necessary condition for acceleration.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Write $V=V_0e^{-A\phi/m_{\rm pl}}$, where the stated model has $V_0=m_{\rm pl}^4$, and take $A>0$. Slow roll gives

$$
H=\sqrt{\frac{8\pi V_0}{3m_{\rm pl}^2}}e^{-A\phi/(2m_{\rm pl})},\qquad\dot\phi=\frac{A\sqrt{V_0}}{\sqrt{24\pi}}e^{-A\phi/(2m_{\rm pl})}.
$$

Thus $d[e^{A\phi/(2m_{\rm pl})}]/dt=A^2\sqrt{V_0}/(\sqrt{96\pi}m_{\rm pl})$. Absorb the integration constant into $b$ to obtain

$$
\boxed{\phi(t)=\frac{2m_{\rm pl}}A\log[C(t+b)],\qquad C^2=\frac{A^4V_0}{96\pi m_{\rm pl}^2}}.
$$

It follows that $H=16\pi/[A^2(t+b)]$, so

$$
\boxed{\frac{a(t)}{a(t_i)}=\left(\frac{t+b}{t_i+b}\right)^p=\exp\left[\frac{8\pi}{Am_{\rm pl}}(\phi-\phi_i)\right],\qquad p=\frac{16\pi}{A^2}}.
$$

The exponential potential has constant $\epsilon_V=A^2/(16\pi)$ and $\eta_V=A^2/(8\pi)$. Inflation requires $p>1$, whereas reliable [slow-roll approximation](../../../cosmic-inflation.md#slow-roll-approximation) requires $A^2/(8\pi)\ll1$. This is the [slow-roll normalization for exponential inflation](../../../cosmic-inflation.md#slow-roll-normalization-for-exponential-inflation).

The stated field normalization is a slow-roll result, not an exact solution of the original full equations. Keeping the acceleration and kinetic terms yields the same $p$ but $C^2=A^4V_0/[2m_{\rm pl}^2(48\pi-A^2)]$, as follows by substituting $\dot\phi=2m_{\rm pl}/[A(t+b)]$ into both full equations. It agrees to leading order for small slope and is the [exponential-potential power-law inflation](../../../cosmic-inflation.md#exponential-potential-power-law-inflation) solution.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

There is no minimum about which this scalar can undergo the damped oscillations normally used for [reheating](../../../cosmic-inflation.md#reheating). Its slow-roll parameters are constant, so an inflating exponential solution has no automatic exit. An independent stopping and energy-transfer mechanism is needed.

At the assumed exit, $V_R=m_{\rm pl}^4e^{-30}$. Equating this to the thermal radiation [density](../../../fluid-mechanics.md#density) gives

$$
\boxed{T_R\simeq\left(\frac{30}{\pi^2g_*}\right)^{1/4}m_{\rm pl}e^{-30/4}\simeq1.5\times10^{15}\ {\rm GeV}}
$$

for $g_*=10^3$. Corrections from the small kinetic fraction do not change this rough estimate.

[Curvature](../../../differential-geometry.md#curvature) obeys $|\Omega-1|\propto(aH)^{-2}$. For constant $\epsilon_H=A^2/(16\pi)$ and $N=\log(a_R/a_i)$, its suppression during [cosmic inflation](../../../cosmic-inflation.md) is $e^{-2(1-\epsilon_H)N}$. Starting from order-one [curvature](../../../differential-geometry.md#curvature) and requiring present [curvature](../../../differential-geometry.md#curvature) no larger than order one gives

$$
N\gtrsim\frac{\log(a_RH_R/a_0H_0)}{1-\epsilon_H}.
$$

After instantaneous [reheating](../../../cosmic-inflation.md#reheating), entropy conservation implies $a_R/a_0=(T_0/T_R)(g_{*s,0}/g_{*s,R})^{1/3}$, with $H_R\simeq1.66\sqrt{g_*}T_R^2/m_{\rm pl}$. Present scales make the numerator roughly $60$; using the literal approximate units from question2 gives about $63$. A tighter present [curvature](../../../differential-geometry.md#curvature) tolerance adds its corresponding half-logarithm. In [slow-roll approximation](../../../cosmic-inflation.md#slow-roll-approximation) this is the conventional requirement of roughly sixty e-folds.

Because the field increases toward $\phi_R$, enough expansion requires

$$
\boxed{\phi_i\lesssim\frac{30m_{\rm pl}}A-\frac{Am_{\rm pl}}{8\pi}\frac{60}{1-A^2/(16\pi)}}.
$$

This is the [flatness bound on the initial field in exponential inflation](../../../cosmology.md#flatness-bound-on-the-initial-field-in-exponential-inflation). It is an **upper bound on the initial field**, not a nonzero minimum: starting earlier at a smaller field produces more expansion. If one additionally restricts the initial potential below $m_{\rm pl}^4$, then $\phi_i\ge0$ supplies a lower bound, but that is a separate restriction. Without initial-curvature and final-tolerance choices there is no unique numerical initial-field value.

## 5

↑ **Parent:** [Paper 71](paper-71.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Put $\mathcal H=a'/a$ and choose the residual synchronous frame comoving with [cold dark matter](../../../cosmology.md#cold-dark-matter), so $\mathbf v_C=0$. Its Euler equation preserves this choice. The continuity equation then gives $\delta_C'=h'/2$. Neglect background [baryon](../../../physics.md#baryon) [pressure](../../../thermodynamics.md#pressure) and all unenhanced corrections of order $c_s^2$, but retain $c_s^2k^2$ because a short wavelength can make it important. The trace equation becomes

$$
h''+\mathcal Hh'=3\mathcal H^2(\Omega_C\delta_C+\Omega_B\delta_B).
$$

Using $h'=2\delta_C'$ proves

$$
\boxed{\delta_C''+\mathcal H\delta_C'-\frac32\mathcal H^2(\Omega_C\delta_C+\Omega_B\delta_B)=0}.
$$

For [baryons](../../../physics.md#baryon) let $\theta_B=i\mathbf k\cdot\mathbf v_B$. The retained continuity and Euler terms are $\delta_B'=-\theta_B+h'/2$ and $\theta_B'+\mathcal H\theta_B-c_s^2k^2\delta_B=0$. Differentiate the first and substitute the second:

$$
\delta_B''+\mathcal H\delta_B'+c_s^2k^2\delta_B=\frac12(h''+\mathcal Hh').
$$

Hence

$$
\boxed{\delta_B''+\mathcal H\delta_B'-\frac32\mathcal H^2(\Omega_C\delta_C+\Omega_B\delta_B)+c_s^2k^2\delta_B=0}.
$$

The [pressure](../../../thermodynamics.md#pressure) sign is stabilizing. The drag terms contain first derivatives of the [density](../../../fluid-mechanics.md#density) perturbations, as printed in the PDF; those primes are lost in the converted TeX. The approximation assumes slowly varying nonrelativistic background [baryon](../../../physics.md#baryon) [pressure](../../../thermodynamics.md#pressure) and the growing physical mode, not a residual [synchronous gauge](../../../linear-cosmological-perturbation-theory.md#synchronous-gauge-in-cosmology) mode.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For small [baryon](../../../physics.md#baryon) fraction the CDM growing mode is $\delta_C\propto a$, and its gravity forces

$$
\delta_B''+\mathcal H\delta_B'+c_s^2k^2\delta_B\simeq4\pi Ga^2\bar\rho_C\delta_C.
$$

For an [adiabatic cosmological perturbation](../../../cosmic-microwave-background-anisotropy.md#adiabatic-initial-conditions) to follow the unsuppressed growing mode, [pressure](../../../thermodynamics.md#pressure) must be below the gravitational forcing frequency: $c_s^2k^2\lesssim4\pi Ga^2\bar\rho_C$. With physical wavelength $\lambda=2\pi a/k$, this becomes

$$
\boxed{\lambda\gtrsim\lambda_J=c_s\sqrt{\frac\pi{G\bar\rho_C}}}.
$$

This is [Jeans support versus forced baryon response](../../../linear-cosmological-density-perturbation.md#jeans-support-versus-forced-baryon-response). The wording “only grow” must refer to unsuppressed gravitational structure growth; it is not a theorem that all shorter-wavelength [baryon](../../../physics.md#baryon) perturbations are absent or constant. In the pressure-dominated regime a forced response $\delta_B\simeq(k_J/k)^2\delta_C$ remains. In particular, a falling [sound speed](../../../compressible-flow.md#speed-of-sound) can make this small response grow even before it catches up to CDM.

Before [photon decoupling](../../../cosmology.md#photon-decoupling), the [photon-baryon fluid](../../../cosmic-microwave-background-anisotropy.md#photon-baryon-fluid) has [sound speed](../../../compressible-flow.md#speed-of-sound) of order $c/\sqrt3$. Its Jeans scale is roughly a horizon scale, so smaller perturbations oscillate acoustically instead of freely following the growing CDM structures. After decoupling the [baryon](../../../physics.md#baryon) [sound speed](../../../compressible-flow.md#speed-of-sound) drops sharply. Above the new Jeans scale, [pressure](../../../thermodynamics.md#pressure) is negligible and subtraction of the CDM equation gives $(\delta_B-\delta_C)''+\mathcal H(\delta_B-\delta_C)'=0$. For $a\propto\tau^2$, the difference is a constant plus a decaying $1/\tau$ term; its ratio to the growing CDM contrast tends to zero. [Baryons](../../../physics.md#baryon) therefore catch up. Under the stipulated post-decoupling $c_s\propto T\propto a^{-1}$, the physical [Jeans length](../../../linear-cosmological-density-perturbation.md#jeans-length) scales as $a^{1/2}$, the comoving scale as $a^{-1/2}$ and the corresponding [Jeans mass](../../../stellar-astrophysics.md#jeans-mass) as $a^{-3/2}$.

For the requested instantaneous [mass](../../../classical-mechanics.md#mass) estimates, define the baryonic [Jeans mass](../../../stellar-astrophysics.md#jeans-mass) as the [baryon](../../../physics.md#baryon) content of a sphere of radius $\lambda_J/2$:

$$
M_{JB}=\frac\pi6\bar\rho_B\lambda_J^3,\qquad\bar\rho_B\simeq0.1\bar\rho_C.
$$

Using the supplied matter-era age gives $t_{\rm dec}=t_0(1+z_{\rm dec})^{-3/2}\simeq9.5\times10^{13}$ s and $\bar\rho_C\simeq1/(6\pi Gt_{\rm dec}^2)\simeq6\times10^{-23}\ {\rm g\,cm^{-3}}$. Then

$$
\boxed{M_{JB}^{\rm before}\sim6\times10^{18}M_\odot\quad(c_s=c/\sqrt3),\qquad M_{JB}^{\rm after}\sim3\times10^4M_\odot\quad(c_s=10^{-5}c)}.
$$

The drop is by $(\sqrt3\times10^{-5})^3$. A definition using the total gravitating [mass](../../../classical-mechanics.md#mass) instead of [baryon](../../../physics.md#baryon) content gives values about ten times larger. The pre-decoupling number is an acoustic Jeans order estimate, not an accurate application of the nonrelativistic equations from part a when $c_s\sim c$.

## 6

↑ **Parent:** [Paper 71](paper-71.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Holding the background metric fixed, the linearized homogeneous-field equation is

$$
\delta\ddot\phi+3H\delta\dot\phi-\frac1{a^2}\nabla_{\rm com}^2\delta\phi+V''(\bar\phi)\delta\phi=0.
$$

Consequently each comoving [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) obeys

$$
\boxed{\delta\ddot\phi_{\mathbf k}+3H\delta\dot\phi_{\mathbf k}+\left(\frac{k^2}{a^2}+m_{\rm eff}^2\right)\delta\phi_{\mathbf k}=0,\qquad m_{\rm eff}^2=V''(\bar\phi)}.
$$

The unscaled Laplacian in the starting equation must be interpreted as the physical spatial Laplacian; for the explicitly comoving [wavevector](../../../continuum-mechanics.md#wavevector) it gives $k^2/a^2$, not $k^2$. Metric fluctuations have been discarded as permitted. The mode written later is a massless, minimally coupled approximation, requiring $|m_{\rm eff}^2|\ll H^2$; it is not a solution for an arbitrary potential [curvature](../../../differential-geometry.md#curvature).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Take a periodic comoving box of volume $L^3$, with $\mathbf k=2\pi\mathbf n/L$. A real field has the expansion

$$
\delta\hat\phi(\mathbf x,t)=\sum_{\mathbf k}\left[w_k(t)\hat a_{\mathbf k}e^{i\mathbf k\cdot\mathbf x}+w_k^*(t)\hat a_{\mathbf k}^\dagger e^{-i\mathbf k\cdot\mathbf x}\right],
$$

where $[\hat a_{\mathbf k},\hat a_{\mathbf q}^\dagger]=\delta_{\mathbf k\mathbf q}$ and the other ladder-operator [commutators](../../../lie-algebra.md#commutator) vanish. The coefficient of $e^{i\mathbf k\cdot\mathbf x}$ is therefore $w_k\hat a_{\mathbf k}+w_k^*\hat a_{-\mathbf k}^\dagger$. This opposite momentum is required by reality; the single-oscillator shorthand with the same label on both operators must not be read literally as every traveling-wave [Fourier coefficient](../../../fourier-series.md#fourier-coefficient).

The quadratic action has [canonical momentum](../../../classical-mechanics.md#canonical-momentum) $\hat\pi=a^3\delta\dot{\hat\phi}$. Its equal-time field [commutator](../../../lie-algebra.md#commutator) requires

$$
\boxed{a^3L^3(w_k\dot w_k^*-w_k^*\dot w_k)=i}.
$$

Choose the vacuum annihilated by all $a_{\mathbf k}$ and the subhorizon positive-frequency condition. For constant $H$ and negligible effective [mass](../../../classical-mechanics.md#mass), put $x=k/(aH)$, $C_k=L^{-3/2}H/\sqrt{2k^3}$. The candidate is $w_k=C_k(i+x)e^{ix}$. Since $\dot x=-Hx$,

$$
\dot w_k=-iHC_kx^2e^{ix},\qquad\ddot w_k=H^2C_k(2ix^2-x^3)e^{ix}.
$$

Direct substitution makes $\ddot w_k+3H\dot w_k+(k^2/a^2)w_k$ identically zero. Its [Wronskian](../../../differential-equation.md#wronskian) is $2iHC_k^2x^3=i/(L^3a^3)$, which has the required normalization. Thus

$$
\boxed{w_k=L^{-3/2}\frac H{\sqrt{2k^3}}\left(i+\frac{k}{aH}\right)e^{ik/(aH)}}.
$$

This is the existing [Bunch-Davies mode normalization in a finite comoving volume](../../../cosmic-inflation.md#bunch-davies-mode-normalization-in-a-finite-comoving-volume). It is exact for a massless minimally coupled test field in de Sitter and the leading approximation for a light slowly evolving field. The homogeneous zero mode needs separate treatment.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

For $k\gg aH$, the dominant term is

$$
w_k\simeq\frac{e^{ik/(aH)}}{L^{3/2}a\sqrt{2k}}=\frac{e^{-ik\eta}}{\sqrt{2L^3a^3\omega_{\rm phys}}},\qquad\eta=-\frac1{aH},\quad\omega_{\rm phys}=\frac ka.
$$

This is the positive-frequency harmonic-oscillator normalization with the physical box volume $a^3L^3$. Over a period much shorter than $H^{-1}$, the [scale factor](../../../cosmology.md#scale-factor-cosmology) and physical frequency are effectively constant. Equivalently, the rescaled field $aL^{3/2}w_k$ approaches $e^{-ik\eta}/\sqrt{2k}$ exactly in the short-wavelength limit.

For $k\ll aH$, $w_k\to iL^{-3/2}H/\sqrt{2k^3}$ and $\dot w_k=O(x^2)$, so the growing field mode freezes. A single [Fourier coefficient](../../../fourier-series.md#fourier-coefficient) has [variance](../../../variance.md) proportional to $k^{-3}$, which by itself is not scale-independent. The number of modes in a logarithmic shell is proportional to $L^3k^3$. Their product gives

$$
\boxed{\frac{d\langle\delta\phi^2\rangle}{d\log k}=\frac{L^3k^3}{2\pi^2}|w_k|^2\longrightarrow\frac{H^2}{4\pi^2}=\left(\frac H{2\pi}\right)^2}.
$$

Thus equal logarithmic intervals have equal [variance](../../../variance.md) in exact de Sitter. Slow evolution of $H$ or nonnegligible effective [mass](../../../classical-mechanics.md#mass) produces a tilt. Integrating an exactly flat spectrum over arbitrarily many logarithmic intervals still requires infrared and ultraviolet cutoffs; the statement concerns power per interval, not a finite all-scale total [variance](../../../variance.md).

## 7

↑ **Parent:** [Paper 71](paper-71.md)

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

Use the convention consistent with the supplied fluid transformations: $\delta g_{ij}=a^2h_{ij}$, so the synchronous spatial metric is $g_{ij}=-a^2\delta_{ij}+a^2h_{ij}$. For a passive coordinate displacement $\xi^0=T e^{i\mathbf k\cdot\mathbf x}$, $\xi^i=i\hat k^iL e^{i\mathbf k\cdot\mathbf x}$, the [metric perturbation](../../../general-relativity.md#linearized-gravity) changes by $\widetilde{\delta g}_{\mu\nu}=\delta g_{\mu\nu}-(\mathcal L_\xi\bar g)_{\mu\nu}$. Computing its components gives

$$
\widetilde{\delta g}_{00}=-2a^2(\mathcal HT+T'),\quad\widetilde{\delta g}_{0i}=ia^2k_i(L'/k-T),
$$



$$
\frac{\widetilde{\delta g}_{ij}}{a^2}=\left[\frac{h-h_S}{3}+2\mathcal HT\right]\delta_{ij}+(h_S-2kL)\hat k_i\hat k_j.
$$

The [Newtonian gauge](../../../linear-cosmological-perturbation-theory.md#newtonian-gauge) has no mixed component and no traceless spatial part. Thus

$$
\boxed{L=\frac{h_S}{2k},\qquad T=\frac{L'}k=\frac{h_S'}{2k^2}}.
$$

Matching $\widetilde{\delta g}_{00}=2a^2\Phi$ and $\widetilde{\delta g}_{ij}=2a^2\Psi\delta_{ij}$ gives

$$
\boxed{\Phi=-\mathcal HT-T'=-\frac{\mathcal Hh_S'+h_S''}{2k^2},\qquad\Psi=\frac{h-h_S}{6}+\frac{\mathcal Hh_S'}{2k^2}}.
$$

This is the [synchronous-to-Newtonian transformation with positive spatial perturbations](../../../linear-cosmological-perturbation-theory.md#synchronous-to-newtonian-transformation-with-positive-spatial-perturbations). The original PDF uses $i\hat{\mathbf k}L$ in the spatial displacement; the converted TeX loses the hat. Using $i\mathbf kL$ would require $L=h_S/(2k^2)$ instead. The nonzero modes $k>0$ are understood.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

There is a sign error in the printed synchronous line-of-sight integrand. Direct contraction of the stated decomposition gives $h'_{ij}n^in^j=(h'-h_S')/3+(\hat{\mathbf k}\cdot\mathbf n)^2h_S'$, with a **plus** sign in its last term. In the positive spatial-perturbation convention of part a, the [redshift](../../../optics.md#redshift) term is half this contraction. The printed minus sign cannot yield the requested Newtonian expression with the supplied transformations.

The consistent identity can be derived explicitly. Work mode by mode with $q=\mathbf k\cdot\mathbf n$, $E(\tau)=e^{iq(\tau-\tau_0)}$ along the unperturbed ray; the shift of the phase origin is immaterial. Put $A=(h-h_S)/6$. Part a gives $A=\Psi-\mathcal HT$, while $\Phi=-\mathcal HT-T'$. Therefore $A'=\Phi'+\Psi'+T''$. The corrected synchronous integral is

$$
I_S=\int_{\tau_d}^{\tau_0}E(A'+q^2T)\,d\tau=\int_{\tau_d}^{\tau_0}E(\Phi'+\Psi')\,d\tau+[E(T'-iqT)]_{\tau_d}^{\tau_0},
$$

since $[E(T'-iqT)]'=E(T''+q^2T)$. This is the [photon redshift identity with positive spatial perturbations](../../../linear-cosmological-perturbation-theory.md#photon-redshift-identity-with-positive-spatial-perturbations).

The supplied fluid shifts are $\delta_\gamma^N=\delta_\gamma+4\mathcal HT$ and $\mathbf v_\gamma^N=\mathbf v_\gamma+i\mathbf kT$. At emission, the synchronous intrinsic and Doppler terms are consequently $E_d[\delta_\gamma^N/4+\mathbf v_\gamma^N\cdot\mathbf n-\mathcal HT-iqT]_d$. Adding the lower integral endpoint cancels the velocity shift and leaves $-\mathcal HT-T'=\Phi$. The upper endpoint is the local observer monopole/dipole $[T'-iqT]_0$, removed by [temperature](../../../thermodynamics.md#temperature) calibration and the observer-rest-frame convention. With zero [anisotropic stress](../../../general-relativity.md#anisotropic-stress), $\Phi=\Psi$, the observable higher-multipole result is

$$
\boxed{\frac{\Delta T}{T}(\mathbf n)=\left[\frac14\delta_\gamma^N+\mathbf v_\gamma^N\cdot\mathbf n+\Phi\right]_d+2\int_{\tau_d}^{\tau_0}\Phi'\,d\tau}.
$$

All fields are evaluated along the ray; the integral contains the time derivative at fixed spatial position. Retaining the printed negative angular term would leave the additional $-2q^2\int ET\,d\tau$, generally a gauge-dependent, nonzero term. It is therefore not repaired merely by discarding observer monopole and dipole.

The first term is the intrinsic [photon](../../../quantum-mechanics.md#photon) [temperature](../../../thermodynamics.md#temperature) perturbation, important in acoustic compressions and rarefactions. The velocity term is the Doppler shift and is prominent near acoustic, roughly degree and subdegree, scales; it is suppressed on very large scales. The potential at emission is the ordinary [Sachs-Wolfe effect](../../../cosmic-microwave-background-anisotropy.md#sachs-wolfe-effect); combined with the intrinsic term it gives the familiar large-angle adiabatic matter-era result $\Phi/3$. The final term is the [Integrated Sachs-Wolfe effect](../../../cosmic-microwave-background-anisotropy.md#integrated-sachs-wolfe-effect), caused by changing potentials. It vanishes for constant matter-era potentials, receives an early contribution near radiation-matter transition, and has an important late large-angle contribution when [curvature](../../../differential-geometry.md#curvature) or dark [energy](../../../classical-mechanics.md#energy) causes potentials to evolve. The sign of the Doppler term follows the photon-propagation direction convention used in the ray; reversing that direction reverses it consistently.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
