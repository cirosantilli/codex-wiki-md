# Paper 314

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_314.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_314.pdf)

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
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
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
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $D/Dt=\partial_t+\mathbf u\cdot\nabla$ be the [material derivative](../../../continuum-mechanics.md#material-derivative), and write $h$ for [specific enthalpy](../../../thermodynamics.md#specific-enthalpy). The [ideal magnetohydrodynamic induction equation](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-induction-equation) and [Gauss's law for magnetism](../../../electromagnetism.md#gauss-s-law-for-magnetism) give

$$
\frac{D\mathbf B}{Dt}=(\mathbf B\cdot\nabla)\mathbf u-\mathbf B\nabla\cdot\mathbf u.
$$

Dotting the momentum equation with $\mathbf B$ eliminates the [Lorentz force density](../../../electromagnetism.md#lorentz-force-density). Therefore the [cross-helicity](../../../astrophysical-fluid-dynamics.md#cross-helicity) density satisfies

$$
\begin{aligned}
\frac{D(\mathbf u\cdot\mathbf B)}{Dt}
&=-\mathbf B\cdot\nabla\Phi-\frac{\mathbf B\cdot\nabla p}{\rho}
+\mathbf B\cdot\nabla\frac{u^2}{2}-(\mathbf u\cdot\mathbf B)\nabla\cdot\mathbf u.
\end{aligned}
$$

The [first law of thermodynamics](../../../thermodynamics.md#first-law-of-thermodynamics) gives $dh=T\,ds+dp/\rho$ for [specific entropy](../../../thermodynamics.md#specific-entropy) $s$, without requiring uniform [entropy](../../../thermodynamics.md#entropy). Consequently

$$
\partial_t h_c+\nabla\cdot(\mathbf u h_c)
=-\mathbf B\cdot\nabla\left(h+\Phi-\frac{u^2}{2}\right)+T\mathbf B\cdot\nabla s.
$$

Since $\nabla\cdot\mathbf B=0$, the first term on the right is a [divergence](../../../calculus.md#divergence). This proves the [cross-helicity conservation law](../../../astrophysical-fluid-dynamics.md#cross-helicity-conservation-law), with flux

$$
\boxed{\mathbf F=\mathbf u(\mathbf u\cdot\mathbf B)+\mathbf B\left(h+\Phi-\frac{u^2}{2}\right).}
$$

For the [perfect gas](../../../thermodynamics.md#ideal-gas) used here, $h=\gamma p/[(\gamma-1)\rho]$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The calculation in part (a) leaves the [cross-helicity conservation law](../../../astrophysical-fluid-dynamics.md#cross-helicity-conservation-law) source

$$
\boxed{Q_h=T\,\mathbf B\cdot\nabla s.}
$$

At positive [temperature](../../../thermodynamics.md#temperature), this vanishes exactly when the [magnetic field](../../../electromagnetism.md#magnetic-field) is tangent to constant-[specific entropy](../../../thermodynamics.md#specific-entropy) surfaces: $\mathbf B\cdot\nabla s=0$. A [homentropic flow](../../../compressible-flow.md#homentropic-flow) is a sufficient special case; uniform [entropy](../../../thermodynamics.md#entropy) throughout space is not necessary. Mere advection of [specific entropy](../../../thermodynamics.md#specific-entropy), $Ds/Dt=0$, constrains its variation along the velocity rather than along the [magnetic field](../../../electromagnetism.md#magnetic-field), so it does not by itself eliminate this source. To conserve total [cross-helicity](../../../astrophysical-fluid-dynamics.md#cross-helicity) in a volume, the net boundary flux must also vanish.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

For uniform [specific entropy](../../../thermodynamics.md#specific-entropy), the [material conservation of cross-helicity density](../../../astrophysical-fluid-dynamics.md#material-conservation-of-cross-helicity-density) criterion is

$$
\frac{Dh_c}{Dt}=\mathbf B\cdot\nabla\left(\frac{u^2}{2}-h-\Phi\right)-h_c\nabla\cdot\mathbf u.
$$

Thus the requested condition is

$$
\boxed{\mathbf B\cdot\nabla\left(\frac{u^2}{2}-h-\Phi\right)=(\mathbf u\cdot\mathbf B)\nabla\cdot\mathbf u.}
$$

In the [steady state](../../../dynamical-systems.md#steady-state), [mass conservation](../../../continuum-mechanics.md#mass-conservation) gives $\nabla\cdot\mathbf u=-\mathbf u\cdot\nabla\log\rho$. An equivalent form, expressed entirely in the flow and thermodynamic variables, is

$$
\boxed{\mathbf B\cdot\nabla\left(\frac{\gamma p}{(\gamma-1)\rho}+\Phi-\frac{u^2}{2}\right)
=(\mathbf u\cdot\mathbf B)\mathbf u\cdot\nabla\log\rho.}
$$

If “isentropic” means only constant [specific entropy](../../../thermodynamics.md#specific-entropy) along individual trajectories, rather than a [homentropic flow](../../../compressible-flow.md#homentropic-flow), the general criterion instead retains $T\mathbf B\cdot\nabla s$ on the right-hand side of the [material derivative](../../../continuum-mechanics.md#material-derivative) equation. The distinction matters because a source-free [cross-helicity conservation law](../../../astrophysical-fluid-dynamics.md#cross-helicity-conservation-law) need not make $h_c$ constant along each trajectory.

## 2

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

In the [shock frame](../../../compressible-flow.md#shock-frame), integrate [mass conservation](../../../continuum-mechanics.md#mass-conservation), momentum conservation, and total-energy conservation across a thin interval containing the stationary [normal shock wave](../../../compressible-flow.md#normal-shock-wave). No mass, momentum, or energy is stored in the vanishingly thin interval, so each flux has the same value on both sides. For a [perfect gas](../../../thermodynamics.md#ideal-gas), the [specific enthalpy](../../../thermodynamics.md#specific-enthalpy) is $h=\gamma p/[(\gamma-1)\rho]$. The resulting [Rankine-Hugoniot conditions for a perfect gas](../../../compressible-flow.md#rankine-hugoniot-conditions-for-a-perfect-gas) are

$$
\boxed{\begin{aligned}
\rho_1u_1&=\rho_2u_2,\\
p_1+\rho_1u_1^2&=p_2+\rho_2u_2^2,\\
u_1\left(\frac{\rho_1u_1^2}{2}+\frac{\gamma p_1}{\gamma-1}\right)
&=u_2\left(\frac{\rho_2u_2^2}{2}+\frac{\gamma p_2}{\gamma-1}\right).
\end{aligned}}
$$

The momentum flux includes both transported momentum and [pressure](../../../thermodynamics.md#pressure) force. The energy flux includes kinetic energy and [enthalpy](../../../thermodynamics.md#enthalpy), the latter accounting for internal energy and the work needed to push gas through the interval. [Entropy production](../../../thermodynamics.md#entropy-production) can occur inside the [normal shock wave](../../../compressible-flow.md#normal-shock-wave) even though total energy is conserved.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $m=\rho_1u_1=\rho_2u_2$ be the signed mass flux. Momentum conservation gives

$$
m^2\left(\frac1{\rho_1}-\frac1{\rho_2}\right)=p_2-p_1.
$$

Dividing the energy-flux equation by $m$ and eliminating $m^2$ yields the [pressure-density Hugoniot relation for a perfect gas](../../../compressible-flow.md#pressure-density-hugoniot-relation-for-a-perfect-gas):

$$
\frac{\gamma}{\gamma-1}\left(\frac{p_2}{\rho_2}-\frac{p_1}{\rho_1}\right)
=\frac{p_2-p_1}{2}\left(\frac1{\rho_1}+\frac1{\rho_2}\right).
$$

With $P=p_2/p_1$ and $D=\rho_2/\rho_1$, this becomes

$$
\frac{2\gamma}{\gamma-1}(P-D)=(P-1)(D+1).
$$

Solving for the [mass density](../../../fluid-mechanics.md#density) ratio gives

$$
\boxed{D=\frac{(\gamma+1)P+\gamma-1}{(\gamma-1)P+\gamma+1}.}
$$

For a compressive [normal shock wave](../../../compressible-flow.md#normal-shock-wave), $P>1$ and $D>1$; as $P\to\infty$, the finite [shock compression ratio](../../../compressible-flow.md#shock-compression-ratio) is $(\gamma+1)/(\gamma-1)$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For a [perfect gas](../../../thermodynamics.md#ideal-gas) with constant [specific heat capacity](../../../thermodynamics.md#specific-heat-capacity) $c_v$, the [first law of thermodynamics](../../../thermodynamics.md#first-law-of-thermodynamics) gives

$$
ds=c_v\,d\log\left(\frac p{\rho^\gamma}\right).
$$

Using the [pressure-density Hugoniot relation for a perfect gas](../../../compressible-flow.md#pressure-density-hugoniot-relation-for-a-perfect-gas), the [entropy production in a perfect-gas shock](../../../compressible-flow.md#entropy-production-in-a-perfect-gas-shock) is therefore

$$
\boxed{\frac{[s]}{c_v}=\log P-\gamma\log\left[\frac{(\gamma+1)P+\gamma-1}{(\gamma-1)P+\gamma+1}\right].}
$$

This is positive for $P>1$, as required by the [Second law of thermodynamics](../../../thermodynamics.md#second-law-of-thermodynamics) for the physical compressive [normal shock wave](../../../compressible-flow.md#normal-shock-wave).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Put $S(P)=[s]/c_v$. Differentiating the expression in part (c) gives

$$
S'(P)=\frac{(\gamma^2-1)(P-1)^2}{P[(\gamma+1)P+\gamma-1][(\gamma-1)P+\gamma+1]}.
$$

For $P=1+\delta$, the denominator is $4\gamma^2+O(\delta)$, so

$$
S'(1+\delta)=\frac{\gamma^2-1}{4\gamma^2}\delta^2+O(\delta^3).
$$

Integrating from the unshocked state, where $S(1)=0$, proves the cubic [entropy production in a perfect-gas shock](../../../compressible-flow.md#entropy-production-in-a-perfect-gas-shock):

$$
\boxed{\frac{[s]}{c_v}=\frac{\gamma^2-1}{12\gamma^2}\delta^3+O(\delta^4).}
$$

The first-order and second-order terms vanish: a [weak shock](../../../compressible-flow.md#weak-shock) agrees with reversible compression through second order.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

For $N$ equal [weak shocks](../../../compressible-flow.md#weak-shock), $(1+\delta)^N=P_s$, hence

$$
N=\frac{\log P_s}{\log(1+\delta)}=\frac{\log P_s}{\delta}[1+O(\delta)].
$$

Adding the individual increases in [specific entropy](../../../thermodynamics.md#specific-entropy) gives the [entropy production in successive weak shocks](../../../compressible-flow.md#entropy-production-in-successive-weak-shocks)

$$
\frac{\Delta s_{\rm weak}}{c_v}
=\frac{\gamma^2-1}{12\gamma^2}\delta^2\log P_s[1+O(\delta)].
$$

By contrast, a single [normal shock wave](../../../compressible-flow.md#normal-shock-wave) with the same total [pressure](../../../thermodynamics.md#pressure) ratio gives

$$
\frac{\Delta s_{\rm single}}{c_v}=\log P_s-\gamma\log D(P_s)
=\log P_s-\gamma\log\frac{\gamma+1}{\gamma-1}+O(P_s^{-1}).
$$

Thus **a single strong shock produces more entropy** than the chain of sufficiently small [weak shocks](../../../compressible-flow.md#weak-shock). At fixed $P_s$, the chain approaches zero [entropy production](../../../thermodynamics.md#entropy-production) as $\delta\to0$, while the single-shock result stays positive. The gradual compression approaches reversible [isentropic flow](../../../compressible-flow.md#isentropic-flow).

## 3

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

With no dependence on the azimuthal or axial coordinates, [Gauss's law for magnetism](../../../electromagnetism.md#gauss-s-law-for-magnetism) in [cylindrical coordinates](../../../calculus.md#cylindrical-coordinate-system) gives

$$
\frac1R\frac{d(RB_R)}{dR}=0,
\qquad B_R=\frac C R.
$$

Regularity at the axis forces $C=0$, so $B_R=0$. The radial component of the magnetostatic [Ampère-Maxwell equation](../../../electromagnetism.md#ampere-s-circuital-law) is

$$
j_R=\frac c{4\pi}(\nabla\times\mathbf B)_R
=\frac c{4\pi}\left(\frac1R\partial_\phi B_z-\partial_z B_\phi\right)=0.
$$

Consequently

$$
\boxed{B_R=j_R=0.}
$$

This is also the starting point of [cylindrical magnetostatic pressure balance](../../../electromagnetism.md#cylindrical-magnetostatic-pressure-balance).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The remaining [magnetic field](../../../electromagnetism.md#magnetic-field) has $\mathbf B=B_\phi(R)\mathbf e_\phi+B_z(R)\mathbf e_z$. The radial [Lorentz force density](../../../electromagnetism.md#lorentz-force-density) separates into a [magnetic pressure](../../../astrophysical-fluid-dynamics.md#magnetic-pressure) gradient and inward [magnetic tension](../../../astrophysical-fluid-dynamics.md#magnetic-tension):

$$
\frac1{4\pi}[(\nabla\times\mathbf B)\times\mathbf B]_R
=-\frac1{8\pi}\frac{d(B_z^2+B_\phi^2)}{dR}-\frac{B_\phi^2}{4\pi R}.
$$

Here $(\mathbf B\cdot\nabla)\mathbf B$ has radial component $-B_\phi^2/R$ because $\partial_\phi\mathbf e_\phi=-\mathbf e_R$. Thus [magnetostatic equilibrium](../../../electromagnetism.md#magnetostatic-equilibrium) gives

$$
\frac d{dR}\left(p+\frac{B_z^2+B_\phi^2}{8\pi}\right)+\frac{B_\phi^2}{4\pi R}=0.
$$

Integrating the axial component of the magnetostatic [Ampère-Maxwell equation](../../../electromagnetism.md#ampere-s-circuital-law) gives $I(R)=cRB_\phi/2$, since regularity removes the integration constant. Substituting $B_\phi=2I/(cR)$ combines the toroidal terms into

$$
\boxed{\frac d{dR}\left(p+\frac{B_z^2}{8\pi}\right)
+\frac1{2\pi c^2R^2}\frac{dI^2}{dR}=0.}
$$

This is the [cylindrical magnetostatic pressure balance](../../../electromagnetism.md#cylindrical-magnetostatic-pressure-balance) equation in terms of enclosed [electric current](../../../electromagnetism.md#electric-current).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For constant $B_z$, [cylindrical magnetostatic pressure balance](../../../electromagnetism.md#cylindrical-magnetostatic-pressure-balance) gives

$$
\frac{dI^2}{dR}=-2\pi c^2R^2\frac{dp}{dR}
=\frac{4\pi c^2kp_0R^3}{a^2}\left(1+\frac{R^2}{a^2}\right)^{-k-1}.
$$

Regularity gives $I(0)=0$. With $x=R^2/a^2$, integration yields the [power-law pressure-supported axial current](../../../electromagnetism.md#power-law-pressure-supported-axial-current)

$$
\boxed{I^2(R)=2\pi c^2p_0a^2
\begin{cases}
\displaystyle\frac{1-(1+kx)(1+x)^{-k}}{k-1},&k\ne1,\\
\log(1+x)+(1+x)^{-1}-1,&k=1.
\end{cases}}
$$

The sign of $I$ may be chosen either way and fixes the sense of the [toroidal magnetic field](../../../astrophysical-fluid-dynamics.md#toroidal-magnetic-field). For $p_0>0$ and nontrivial decreasing [pressure](../../../thermodynamics.md#pressure) ($k>0$), the integral converges at infinity precisely when

$$
\boxed{k>1,\qquad I^2(\infty)=\frac{2\pi c^2p_0a^2}{k-1}.}
$$

At $k=1$ it diverges logarithmically; for $0<k<1$ it diverges as $R^{2(1-k)}$. The degenerate case $k=0$ has constant [pressure](../../../thermodynamics.md#pressure) and zero [electric current](../../../electromagnetism.md#electric-current).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Setting $I=0$ in [cylindrical magnetostatic pressure balance](../../../electromagnetism.md#cylindrical-magnetostatic-pressure-balance) gives $p+B_z^2/(8\pi)=\mathrm{constant}$. The axial boundary value sets this constant to $p_0$. Thus the [magnetic pressure support with vanishing axial field](../../../electromagnetism.md#magnetic-pressure-support-with-vanishing-axial-field) solution is

$$
\boxed{B_z(R)=\sigma\sqrt{8\pi p_0}\sqrt{1-e^{-R^2/a^2}},\qquad \sigma=\pm1.}
$$

The azimuthal component of the magnetostatic [Ampère-Maxwell equation](../../../electromagnetism.md#ampere-s-circuital-law) gives

$$
\boxed{j_\phi(R)=-\sigma\frac{c\sqrt{8\pi p_0}}{4\pi a^2}
\frac{R e^{-R^2/a^2}}{\sqrt{1-e^{-R^2/a^2}}}.}
$$

Since $1-e^{-R^2/a^2}=R^2/a^2+O(R^4)$, the radial limit is

$$
\boxed{\lim_{R\downarrow0}j_\phi(R)=-\sigma\frac{c\sqrt{8\pi p_0}}{4\pi a}.}
$$

There is a regularity subtlety: $B_z\sim\sigma\sqrt{8\pi p_0}R/a$ is not a [smooth function](../../../analysis.md#smooth-function) of Cartesian position at the axis, and the nonzero limiting $j_\phi$ multiplies an azimuthal unit vector with no unique direction there. These formulas solve the radial problem for $R>0$ and give the requested scalar limit, but the data in this part do not admit the fully smooth vector-field regularity assumed in part (a).

## 4

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Align the polar axis with the [magnetic dipole moment](../../../electromagnetism.md#magnetic-dipole-moment). The [magnetic dipole field](../../../electromagnetism.md#magnetic-dipole-field) has

$$
B_r=\frac{2m\cos\theta}{r^3},\qquad B_\theta=\frac{m\sin\theta}{r^3}.
$$

The [magnetic-field-line equation](../../../electromagnetism.md#magnetic-field-line-equation) gives $dr/(r\,d\theta)=2\cot\theta$, hence the [dipole magnetic-field line](../../../electromagnetism.md#dipole-magnetic-field-line) is $r=C\sin^2\theta$. Normalize the loaded bundle by its small surface angular radius $\theta_\star$ at $r=R_\star$. Its boundary obeys

$$
\frac{\sin^2\theta(r)}{\sin^2\theta_\star}=\frac r{R_\star},
\qquad
\theta(r)^2\simeq\theta_\star^2\frac r{R_\star}.
$$

The [dipolar flux-tube area](../../../electromagnetism.md#dipolar-flux-tube-area) for one polar cap is consequently

$$
\boxed{A(r)\simeq\pi\theta_\star^2\frac{r^3}{R_\star}.}
$$

Equivalently, $BA$ is constant by conservation of [magnetic flux](../../../electromagnetism.md#magnetic-flux) and $B\propto r^{-3}$ near the axis. Two equal loaded caps double the total area. The $r^3$ scaling is independent of the normalization; if the loading angle is specified at another radius $r_L$, use $A(r)=\pi\theta_L^2r^3/r_L$ instead.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

In the narrow polar [flux tube](../../../electromagnetism.md#flux-tube), the [magnetic field lines](../../../electromagnetism.md#magnetic-field-line) are almost radial and the transverse width is much smaller than the radial scale. The [Lorentz force density](../../../electromagnetism.md#lorentz-force-density) has no component along the [magnetic field](../../../electromagnetism.md#magnetic-field), so the longitudinal [magnetically channelled accretion](../../../astrophysics.md#magnetically-channelled-accretion) is hydrodynamic. Let $v(r)>0$ denote inward speed. [Mass conservation](../../../continuum-mechanics.md#mass-conservation), the [Euler equations for an inviscid fluid](../../../fluid-mechanics.md#euler-equations-for-an-inviscid-fluid), and the [polytropic equation of state](../../../astrophysical-fluid-dynamics.md#polytropic-equation-of-state) give

$$
\rho vA=\dot M_{\rm tube},\qquad
v\frac{dv}{dr}=-\frac1\rho\frac{dp}{dr}-\frac{GM_\star}{r^2},\qquad
p=K\rho^\gamma.
$$

Using the [adiabatic sound speed](../../../compressible-flow.md#adiabatic-sound-speed) $c^2=\gamma K\rho^{\gamma-1}$ and $A\propto r^3$,

$$
\frac{\rho'}\rho=-\frac{v'}v-\frac3r,
\qquad
\boxed{\left(v-\frac{c^2}{v}\right)v'=\frac{3c^2}{r}-\frac{GM_\star}{r^2}.}
$$

The [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) is

$$
\boxed{\frac{v^2}{2}+\frac{c^2}{\gamma-1}-\frac{GM_\star}{r}=\frac{c_0^2}{\gamma-1},}
$$

where the right-hand side comes from matching to a nearly stationary reservoir with negligible [gravitational potential](../../../classical-mechanics.md#newtonian-potential-of-a-point-mass). The fixed [magnetic field](../../../electromagnetism.md#magnetic-field) provides transverse confinement; neglecting magnetic forces in this one-dimensional equation concerns their longitudinal component.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

A regular [sonic point](../../../compressible-flow.md#sonic-point) must make both sides of the flow equation vanish:

$$
v_s=c_s,\qquad r_s=\frac{GM_\star}{3c_s^2}.
$$

Substituting into the [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) yields

$$
c_s^2\left(\frac1{\gamma-1}-\frac52\right)=\frac{c_0^2}{\gamma-1},
\qquad
c_s^2=\frac{2c_0^2}{7-5\gamma}.
$$

For $\gamma>1$, positive finite [sound speed](../../../compressible-flow.md#speed-of-sound) therefore requires the [critical adiabatic index for dipolar accretion](../../../astrophysics.md#critical-adiabatic-index-for-dipolar-accretion)

$$
\boxed{1<\gamma<\gamma_{\rm crit}=\frac75.}
$$

To check that this gives real regular crossings, differentiate the flow equation at the [sonic point](../../../compressible-flow.md#sonic-point) and put $x=r_sv'_s/c_s$. The [transonic accretion in a power-law tube](../../../compressible-flow.md#transonic-accretion-in-a-power-law-tube) calculation gives

$$
(\gamma+1)x^2+6(\gamma-1)x+9\gamma-12=0,
\qquad
x=\frac{-3(\gamma-1)\pm\sqrt{3(7-5\gamma)}}{\gamma+1}.
$$

The minus sign gives the [transonic branch](../../../compressible-flow.md#transonic-branch) whose [Mach number](../../../compressible-flow.md#mach-number) increases inward. At $\gamma=7/5$ the positive-energy reservoir cannot match a finite [sonic point](../../../compressible-flow.md#sonic-point); for larger $\gamma$ the required $c_s^2$ is negative. A physical surface-crossing solution also requires $r_s>R_\star$ and validity of the narrow [flux tube](../../../electromagnetism.md#flux-tube) approximation up to the sonic region.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The [transonic accretion in a dipolar flux tube](../../../astrophysics.md#transonic-accretion-in-a-dipolar-flux-tube) values are

$$
\boxed{r_s=\frac{GM_\star(7-5\gamma)}{6c_0^2},\qquad
c_s=c_0\sqrt{\frac2{7-5\gamma}},\qquad
\rho_s=\rho_0\left(\frac2{7-5\gamma}\right)^{1/(\gamma-1)}.}
$$

The [mass density](../../../fluid-mechanics.md#density) follows from $c^2/c_0^2=(\rho/\rho_0)^{\gamma-1}$ for the same [polytropic equation of state](../../../astrophysical-fluid-dynamics.md#polytropic-equation-of-state). If $A_\star$ is the total loaded area at the surface, [mass conservation](../../../continuum-mechanics.md#mass-conservation) at the [sonic point](../../../compressible-flow.md#sonic-point) gives

$$
\boxed{\dot M=A_\star\left(\frac{r_s}{R_\star}\right)^3\rho_s c_s.}
$$

For two equal polar caps with surface angular radius $\theta_\star$, $A_\star\simeq2\pi R_\star^2\theta_\star^2$, so the total [mass accretion rate](../../../astrophysics.md#mass-accretion-rate) is

$$
\boxed{\dot M=\frac{2\pi\theta_\star^2\rho_0(GM_\star)^3}{27R_\star c_0^5}
\left(\frac2{7-5\gamma}\right)^{1/(\gamma-1)-5/2}.}
$$

For only one loaded polar cap, divide this expression by two. Expressing the result first in $A_\star$ also covers a bundle whose loading angle is defined at another radius. The smooth isothermal limit $\gamma\to1$ has $r_s=GM_\star/(3c_0^2)$, $c_s=c_0$, and $\rho_s=e^{5/2}\rho_0$.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

The [dipole magnetic-field line](../../../electromagnetism.md#dipole-magnetic-field-line) geometry gives the angular radius at the [sonic point](../../../compressible-flow.md#sonic-point) as $\theta_s\simeq\theta_\star\sqrt{r_s/R_\star}$. The sonic region must remain a narrow [flux tube](../../../electromagnetism.md#flux-tube) for the one-dimensional [transonic branch](../../../compressible-flow.md#transonic-branch) equations to apply. Thus a necessary small-angle constraint is

$$
\boxed{\theta_\star\ll\sqrt{\frac{R_\star}{r_s}}
=\sqrt{\frac{6c_0^2R_\star}{GM_\star(7-5\gamma)}}.}
$$

This also makes the transverse sound-crossing time $r_s\theta_s/c_s$ small compared with the radial flow time $r_s/c_s$. The restriction must hold at any larger matching radius as well. To match to a reservoir with negligible [gravitational potential](../../../classical-mechanics.md#newtonian-potential-of-a-point-mass) within the same narrow dipolar approximation, one needs an overlap region

$$
\frac{GM_\star}{c_0^2}\ll r_L\ll\frac{R_\star}{\theta_\star^2}.
$$

Hence the stronger useful sufficient scaling is $\theta_\star^2\ll R_\star c_0^2/(GM_\star)$. The small-angle dipolar model should not be extrapolated to literal infinity, where its boundary [magnetic field line](../../../electromagnetism.md#magnetic-field-line) turns toward the equatorial plane.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
