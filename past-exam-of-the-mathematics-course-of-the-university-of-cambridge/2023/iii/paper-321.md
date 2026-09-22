# Paper 321

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_321.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_321.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
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
  - [f](#2/f)
    - [Solution](#2/f/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)

## 1

↑ **Parent:** [Paper 321](paper-321.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

In the [razor-thin disk approximation](../../../astrophysics.md#razor-thin-disk-approximation), the three-dimensional [Poisson equation](../../../partial-differential-equation.md#poisson-equation) is

$$
\nabla^2\Phi_d=4\pi G\Sigma(x,y)\delta(z).
$$

For a horizontal [Fourier mode](../../../fourier-analysis.md#fourier-mode) with [wavevector](../../../continuum-mechanics.md#wavevector) $\mathbf k$ and $k=|\mathbf k|>0$, the [Fourier transform](../../../analysis.md#fourier-transform) of this equation is

$$
\left(\frac{d^2}{dz^2}-k^2\right)\widehat\Phi_d
=4\pi G\widehat\Sigma\,\delta(z).
$$

The solution that decays away from the disk is

$$
\widehat\Phi_d(\mathbf k,z)
=-\frac{2\pi G}{k}\widehat\Sigma(\mathbf k)e^{-k|z|}.
$$

Consequently the required [razor-thin disk Poisson kernel](../../../astrophysics.md#razor-thin-disk-poisson-kernel) in the midplane is

$$
\boxed{\widehat\Phi_{d,m}(\mathbf k)
=-\frac{2\pi G}{k}\widehat\Sigma(\mathbf k)}.
$$

The spatially uniform $k=0$ background is excluded from this local perturbation formula.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For a [Keplerian shearing sheet](../../../gravitational-instability-of-an-astrophysical-disk.md#keplerian-shearing-sheet), the shear rate is $S=3\Omega/2$ and the [shearing-sheet tidal potential](../../../gravitational-instability-of-an-astrophysical-disk.md#shearing-sheet-tidal-potential) is

$$
\boxed{\Phi_{t,m}=-\Omega Sx^2=-\frac32\Omega^2x^2}.
$$

A uniform steady solution is

$$
\Sigma=\Sigma_0,
\qquad P=P_0,
\qquad \mathbf u_0=-Sx\,\mathbf e_y.
$$

The [Coriolis acceleration](../../../physics.md#coriolis-acceleration) of this [linear shear flow](../../../fluid-mechanics.md#linear-shear-flow) balances the radial tidal acceleration. The only nonzero background component of the [viscous stress tensor](../../../fluid-mechanics.md#viscous-stress-tensor) that matters is $T_{xy}=-\nu(\Sigma_0)\Sigma_0S$, which is spatially constant. Hence $\nabla\mathbin\cdot\mathbf T=0$: a local uniform patch has no stress gradient or torque divergence to drive an [accretion flow](../../../astrophysics.md#accretion-flow).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Write the perturbations as $(\sigma,u,v)e^{ik_xx+\lambda t}$, set $k=|k_x|$, and evaluate all unmarked background quantities at $\Sigma_0$. Define

$$
v_s^2=\left.\frac{dP}{d\Sigma}\right|_{\Sigma_0},
\qquad
\beta=\left.\frac{d\ln(\nu\Sigma)}{d\ln\Sigma}\right|_{\Sigma_0}.
$$

The linearized [mass conservation](../../../continuum-mechanics.md#mass-conservation) equation is

$$
\lambda\sigma+ik_x\Sigma_0u=0.
$$

The radial and azimuthal momentum equations are

$$
\left[\lambda+\left(\nu_b+\frac43\nu\right)k^2\right]u-2\Omega v
=-ik_x\left(v_s^2\frac{\sigma}{\Sigma_0}+\phi\right),
$$



$$
(\lambda+\nu k^2)v+(2\Omega-S)u
=-ik_xS\beta\nu\frac{\sigma}{\Sigma_0},
$$

where the [razor-thin disk Poisson kernel](../../../astrophysics.md#razor-thin-disk-poisson-kernel) gives $\phi=-2\pi G\sigma/k$. The term proportional to $\beta$ comes from perturbing the density-dependent background shear stress $T_{xy}=-\nu\Sigma S$.

Eliminating $\sigma,u,v$ and using $S=3\Omega/2$, so that the [radial epicyclic frequency](../../../astrophysics.md#radial-epicyclic-frequency) obeys $\kappa_r^2=2\Omega(2\Omega-S)=\Omega^2$, gives the [dispersion relation](../../../wave-equation.md#dispersion-relation)

$$
\boxed{
(\lambda+\nu k^2)
\left\{\lambda\left[\lambda+
\left(\nu_b+\frac43\nu\right)k^2\right]
-2\pi G\Sigma_0k+v_s^2k^2\right\}
+\lambda\Omega^2+3\beta\Omega^2\nu k^2=0}.
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Setting $\nu=\nu_b=0$, the [dispersion relation](../../../wave-equation.md#dispersion-relation) reduces to

$$
\lambda\left(\lambda^2+\Omega^2-2\pi G\Sigma_0k+v_s^2k^2\right)=0.
$$

An axisymmetric density mode grows when

$$
2\pi G\Sigma_0k-v_s^2k^2>\Omega^2.
$$

The left-hand side is a concave [quadratic function](../../../polynomial.md#quadratic-function) of $k$, with maximum $(\pi G\Sigma_0)^2/v_s^2$ at $k=\pi G\Sigma_0/v_s^2$. Growth is therefore possible precisely when the [Toomre stability criterion](../../../gravitational-instability-of-an-astrophysical-disk.md#toomre-s-stability-criterion) is violated:

$$
\boxed{Q=\frac{v_s\Omega}{\pi G\Sigma_0}<1}.
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The constant term of the real cubic [dispersion relation](../../../wave-equation.md#dispersion-relation) is

$$
c=\nu k^2\left(3\beta\Omega^2-2\pi G\Sigma_0k+v_s^2k^2\right).
$$

A negative $c$ guarantees a positive real root because the cubic tends to $+\infty$ as $\lambda\to+\infty$.

If $\beta<0$, then $c<0$ at sufficiently small positive $k$, producing a [viscous instability of an accretion disk](../../../astrophysics.md#viscous-instability-of-an-accretion-disk). This is the local form of the global thin-disk diffusion equation

$$
\frac{\partial\Sigma}{\partial t}
=\frac3r\frac{\partial}{\partial r}
\left[r^{1/2}\frac{\partial}{\partial r}
(\nu\Sigma r^{1/2})\right].
$$

Since $d(\nu\Sigma)/d\Sigma<0$, the effective diffusion reverses sign and amplifies surface-density variations.

If $\beta>0$, instability is still possible when the quadratic expression in parentheses is negative. Its minimum occurs at $k=\pi G\Sigma_0/v_s^2$, so the condition is

$$
3\beta\Omega^2-\frac{(\pi G\Sigma_0)^2}{v_s^2}<0,
$$

or

$$
\boxed{Q<\frac1{\sqrt{3\beta}}}.
$$

This is a [secular gravitational instability of an astrophysical disk](../../../gravitational-instability-of-an-astrophysical-disk.md#secular-gravitational-instability-of-an-astrophysical-disk): viscosity allows self-gravity to overcome rotational support even in part of the range that is stable by the inviscid $Q<1$ criterion.

## 2

↑ **Parent:** [Paper 321](paper-321.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $D/Dt=\partial_t-Sx\partial_y$ be the [material derivative](../../../continuum-mechanics.md#material-derivative) along the background [linear shear flow](../../../fluid-mechanics.md#linear-shear-flow) $\mathbf u_0=-Sx\mathbf e_y$. Linearizing about constant $\Sigma$ gives

$$
\frac{D\Sigma'}{Dt}
=-\Sigma(\partial_xv_x+\partial_yv_y),
$$



$$
\frac{Dv_x}{Dt}-2\Omega v_y
=-\partial_x\Psi-\frac{v_s^2}{\Sigma}\partial_x\Sigma',
$$



$$
\frac{Dv_y}{Dt}+(2\Omega-S)v_x
=-\partial_y\Psi-\frac{v_s^2}{\Sigma}\partial_y\Sigma'.
$$

The coefficient $2\Omega-S$ includes the contribution $\mathbf v\mathbin\cdot\nabla\mathbf u_0=-Sv_x\mathbf e_y$ from perturbation advection of the background shear.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The first-order perturbation of the [vortensity](../../../gravitational-instability-of-an-astrophysical-disk.md#vortensity) is

$$
\boxed{f'=
\frac1\Sigma(\partial_xv_y-\partial_yv_x)
-\frac{2\Omega-S}{\Sigma^2}\Sigma'}.
$$

Taking the curl of the linearized momentum equation and using the linearized continuity equation yields

$$
\boxed{\frac{Df'}{Dt}=0}.
$$

This is [linearized vortensity conservation](../../../gravitational-instability-of-an-astrophysical-disk.md#linearized-vortensity-conservation). It is the perturbative form of material conservation of [potential vorticity](../../../geophysical-fluid-dynamics.md#potential-vorticity) in an inviscid [barotropic fluid](../../../fluid-mechanics.md#barotropic-fluid); the forcing $-\nabla\Psi$ is a gradient and therefore creates no [vorticity](../../../fluid-mechanics.md#vorticity).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For zero forcing, the given equation for $v_y$ is

$$
\left(\frac{D^2}{Dt^2}+\kappa_r^2-v_s^2\nabla^2\right)v_y=0.
$$

Use the [shearing-wave ansatz](../../../gravitational-instability-of-an-astrophysical-disk.md#shearing-wave-ansatz)

$$
v_y=\Re\left\{\widetilde v(t)
e^{i[k_x(t)x+k_yy]}\right\}.
$$

The explicit $x$ dependence cancels from the [material derivative](../../../continuum-mechanics.md#material-derivative) when

$$
\boxed{\dot k_x=Sk_y,
\qquad k_x(t)=k_x(0)+Sk_yt}.
$$

The amplitude then obeys the time-dependent [harmonic oscillator](../../../classical-mechanics.md#simple-harmonic-motion) equation

$$
\boxed{\ddot{\widetilde v}+g(t)\widetilde v=0,
\qquad
g(t)=\kappa_r^2+v_s^2[k_x(t)^2+k_y^2]}.
$$

This evolving [wavevector](../../../continuum-mechanics.md#wavevector) is the characteristic signature of a [shearing wave](../../../gravitational-instability-of-an-astrophysical-disk.md#shearing-wave).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

A satellite on a circular orbit is stationary in the corotating sheet. Write its tidal forcing and the response as

$$
\Psi=\psi(x)e^{ik_yy},
\qquad
v_y=v(x)e^{ik_yy}.
$$

Since $D=-iSk_yx$, the forced wave equation becomes

$$
\boxed{
-v_s^2v''+
[\kappa_r^2+v_s^2k_y^2-S^2k_y^2x^2]v
=(2\Omega-S)\psi'-Sxk_y^2\psi}.
$$

This ordinary differential equation describes a [satellite-forced density wave in an astrophysical disk](../../../gravitational-instability-of-an-astrophysical-disk.md#satellite-forced-density-wave-in-an-astrophysical-disk).

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

The homogeneous equation can be written

$$
v''+\left[
\frac{S^2k_y^2x^2}{v_s^2}-k_y^2-
\frac{\kappa_r^2}{v_s^2}
\right]v=0.
$$

Its solutions are locally oscillatory where

$$
S^2k_y^2x^2>\kappa_r^2+v_s^2k_y^2,
$$

equivalently

$$
\boxed{|Sx|>\sqrt{v_s^2+\frac{\kappa_r^2}{k_y^2}}>v_s}.
$$

The relative background orbital speed is $|\mathbf u_0|=|Sx|$, so propagating wave zones occur only where the relative motion of the satellite and disk material is [supersonic](../../../compressible-flow.md#supersonic-flow).

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Take the [Fourier transform](../../../analysis.md#fourier-transform) in $x$, with convention $\widetilde v(k_x)=\int v(x)e^{-ik_xx}\,dx$. The differentiation rules $\widehat{v''}=-k_x^2\widetilde v$ and $\widehat{x^2v}=-\widetilde v''$ turn the forced equation into

$$
S^2k_y^2\frac{d^2\widetilde v}{dk_x^2}
+[\kappa_r^2+v_s^2(k_x^2+k_y^2)]\widetilde v
=i\left[(2\Omega-S)k_x\widetilde\psi
-Sk_y^2\frac{d\widetilde\psi}{dk_x}\right].
$$

For the unforced equation, $dk_x/dt=Sk_y$ implies

$$
\frac{d^2}{dt^2}=S^2k_y^2\frac{d^2}{dk_x^2}.
$$

It is therefore exactly the [shearing-wave oscillator](../../../gravitational-instability-of-an-astrophysical-disk.md#shearing-wave-oscillator) found in part c, now parametrized by radial [wavenumber](../../../wave-equation.md#wavenumber) rather than time.

## 3

↑ **Parent:** [Paper 321](paper-321.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a circular orbit of cylindrical radius $r$ in an axisymmetric gravitational potential,

$$
\Omega^2=\frac1r\frac{\partial\Phi}{\partial r}(r,0).
$$

A small vertical displacement satisfies

$$
\ddot z=-\frac{\partial^2\Phi}{\partial z^2}(r,0)z,
$$

so the [vertical epicyclic frequency](../../../astrophysics.md#vertical-epicyclic-frequency) is

$$
\boxed{\Omega_z^2=\frac{\partial^2\Phi}{\partial z^2}(r,0)}.
$$

For a [spherically symmetric potential](../../../classical-mechanics.md#spherically-symmetric-potential) $\Phi(R)$, where $R=(r^2+z^2)^{1/2}$,

$$
\frac{\partial^2\Phi}{\partial z^2}(r,0)
=\frac1r\frac{d\Phi}{dR}(r)=\Omega^2.
$$

Hence $\boxed{\Omega_z=\Omega}$. Geometrically, a slightly tilted circular orbit remains a circular orbit in a different plane, and its height completes one oscillation per revolution.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Vertical [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) gives

$$
\frac{dp}{dz}=-\rho\Omega_z^2z.
$$

Define vertically integrated pressure and the density-weighted [disk scale height](../../../astrophysics.md#disk-scale-height) by

$$
P=\int_{-\infty}^{\infty}p\,dz,
\qquad
H^2=\frac1\Sigma\int_{-\infty}^{\infty}\rho z^2\,dz.
$$

Multiply the hydrostatic equation by $z$ and integrate. Since $zp\to0$ at both boundaries, [integration by parts](../../../calculus.md#integration-by-parts) gives

$$
-P=-\Omega_z^2\Sigma H^2.
$$

Therefore

$$
\boxed{P=\Sigma H^2\Omega_z^2}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Introduce the [dimensionless variables](../../../mathematics.md#dimensionless-variable)

$$
\widetilde z=\frac zH,
\qquad
\rho=\frac\Sigma H\widetilde\rho(\widetilde z),
\qquad
p=\frac PH\widetilde p(\widetilde z).
$$

Using $P=\Sigma H^2\Omega_z^2$, vertical [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) becomes the parameter-free equation

$$
\boxed{\frac{d\widetilde p}{d\widetilde z}
=-\widetilde\rho\,\widetilde z},
$$

with normalizations $\int\widetilde\rho\,d\widetilde z=1$ and $\int\widetilde p\,d\widetilde z=1$. For an [isothermal atmosphere](../../../statistical-physics.md#isothermal-atmosphere), $p=c_s^2\rho$, and these conventions give the [Gaussian distribution](../../../probability-theory.md#normal-distribution)

$$
\boxed{
\widetilde\rho(\widetilde z)=\widetilde p(\widetilde z)
=\frac1{\sqrt{2\pi}}e^{-\widetilde z^2/2}}.
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Gas in hydrostatic balance has zero vertical velocity. A dust grain subject to linear drag with [aerodynamic stopping time](../../../fluid-mechanics.md#aerodynamic-stopping-time) $\tau$ therefore obeys

$$
\boxed{\ddot z+\frac1\tau\dot z+\Omega_z^2z=0}.
$$

This is a [damped harmonic oscillator](../../../analysis.md#damped-harmonic-oscillator). For $\Omega_z\tau>1/2$, the motion is underdamped, with angular frequency

$$
\sqrt{\Omega_z^2-\frac1{4\tau^2}}
$$

and envelope $e^{-t/(2\tau)}$. [Critical damping](../../../wave-equation.md#critical-damping) occurs at $\Omega_z\tau=1/2$. For $\Omega_z\tau<1/2$, the motion is overdamped. In the strong-drag limit $\Omega_z\tau\ll1$, a rapid transient on timescale $\tau$ leaves slow [dust settling in an astrophysical disk](../../../astrophysics.md#dust-settling-in-an-astrophysical-disk) at rate $\Omega_z^2\tau$; in the weak-drag limit the grain makes many damped vertical oscillations.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Let $\zeta=z/H(t)$ label a fluid element and use the [homologous vertical motion of an astrophysical disk](../../../astrophysics.md#homologous-vertical-motion-of-an-astrophysical-disk)

$$
\rho=\frac\Sigma H\widetilde\rho(\zeta),
\qquad
p=\frac{P(t)}H\widetilde p(\zeta),
\qquad
\mathbf u=-Sx\mathbf e_y+\dot H\zeta\mathbf e_z.
$$

Because $D\zeta/Dt=0$ and $\nabla\mathbin\cdot\mathbf u=\dot H/H$, this ansatz satisfies [mass conservation](../../../continuum-mechanics.md#mass-conservation). The pressure equation for an [adiabatic process](../../../thermodynamics.md#adiabatic-process) gives

$$
\frac{\dot P}{P}+(\gamma-1)\frac{\dot H}{H}=0,
$$

hence

$$
\boxed{PH^{\gamma-1}=\text{constant},
\qquad P\mathrel\propto H^{1-\gamma}}.
$$

The vertical acceleration is $D u_z/Dt=\ddot H\zeta$. Using the dimensionless hydrostatic profiles from part c, the pressure force is $(P/\Sigma H)\zeta$, and the vertical momentum equation reduces to

$$
\boxed{\ddot H+\Omega_z^2H=CH^{-\gamma}},
$$

where $C$ is constant.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

At the equilibrium thickness $H_0$,

$$
\Omega_z^2H_0=CH_0^{-\gamma}.
$$

Set $H=H_0+h$ and retain terms linear in $h$. The [linearization](../../../algebra.md#linearization) is

$$
\ddot h+(\gamma+1)\Omega_z^2h=0.
$$

Thus the [vertical breathing mode of an astrophysical disk](../../../astrophysics.md#vertical-breathing-mode-of-an-astrophysical-disk) has angular frequency

$$
\boxed{\omega_H=\sqrt{\gamma+1}\,\Omega_z}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
