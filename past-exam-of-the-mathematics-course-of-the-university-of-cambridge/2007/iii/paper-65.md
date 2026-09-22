# Paper 65

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper65.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper65.pdf)

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
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 65](paper-65.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

In the [energy](../../../classical-mechanics.md#energy)-conserving blast regime, neglect ambient [pressure](../../../thermodynamics.md#pressure), radiative losses, ejecta mass and gravity compared with the explosion. The cold ambient [ideal gas](../../../thermodynamics.md#ideal-gas) has no [sound speed](../../../compressible-flow.md#speed-of-sound) scale, and its power-law [mass density](../../../fluid-mechanics.md#density) has no preferred radius. The point explosion introduces only its [energy](../../../classical-mechanics.md#energy) $E$ and elapsed time $t$. This scale-free setting supports a [self-similar blast wave](../../../compressible-flow.md#self-similar-blast-wave); extra physics would limit the time interval over which that description applies.

The mass swept up to radius $R$ is

$$
M(R)=4\pi\int_0^R Cr^{2-\beta}\,dr=\frac{4\pi C}{3-\beta}R^{3-\beta}.
$$

It is finite because $\beta<3$. With no [energy](../../../classical-mechanics.md#energy) loss, the [kinetic energy](../../../classical-mechanics.md#kinetic-energy) and [internal energy](../../../thermodynamics.md#internal-energy) both scale as $CR^{3-\beta}\dot R^2$. Therefore $R^{3-\beta}\dot R^2$ is constant and integration gives

$$
\boxed{R(t)=A\left(\frac EC\right)^{1/(5-\beta)}t^{2/(5-\beta)}}.
$$

The dimensionless coefficient $A$ depends on the [adiabatic exponent](../../../thermodynamics.md#heat-capacity-ratio) and ambient exponent through the [similarity profiles](../../../partial-differential-equation.md#similarity-profile). Indeed, $[E/C]=L^{5-\beta}T^{-2}$, which independently verifies the scaling. The [shock wave](../../../partial-differential-equation.md#shock-wave) decelerates for $0<\beta<3$, since its time exponent lies between $2/5$ and $1$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $V=\dot R$, $a=2/(5-\beta)$ and

$$
\xi=\frac rR,\qquad u(r,t)=V U(\xi),\qquad
\rho(r,t)=CR^{-\beta}D(\xi),\qquad
p(r,t)=CR^{-\beta}V^2P(\xi).
$$

Here $u$ is the outward radial [velocity](../../../classical-mechanics.md#velocity); $U,D,P$ are dimensionless. The relations

$$
\partial_t\xi=-\frac VR\xi,\qquad
\partial_r\xi=\frac1R,\qquad
q\equiv\frac{R\dot V}{V^2}=\frac{a-1}{a}=\frac{\beta-3}{2}
$$

are sufficient for the reduction. In smooth post-shock gas the spherical [continuity equation](../../../physics.md#continuity-equation), [Euler equations](../../../fluid-mechanics.md#euler-equations-for-an-inviscid-fluid) and adiabatic [pressure](../../../thermodynamics.md#pressure) equation are

$$
\partial_t\rho+u\partial_r\rho=-\rho(\partial_ru+2u/r),\qquad
\partial_tu+u\partial_ru=-\frac1\rho\partial_rp,
$$



$$
\partial_tp+u\partial_rp=-\gamma p(\partial_ru+2u/r).
$$

For example, the [mass density](../../../fluid-mechanics.md#density) [material derivative](../../../continuum-mechanics.md#material-derivative) is $CR^{-\beta}(V/R)[(U-\xi)D'-\beta D]$, and the [velocity](../../../classical-mechanics.md#velocity) [material derivative](../../../continuum-mechanics.md#material-derivative) is $(V^2/R)[(U-\xi)U'+qU]$. After cancellation of the dimensional factors the [spherical blast wave in a power-law ambient density](../../../compressible-flow.md#spherical-blast-wave-in-a-power-law-ambient-density) obeys

$$
\boxed{(U-\xi)D'+D\left(U'+\frac{2U}{\xi}-\beta\right)=0,}
$$



$$
\boxed{(U-\xi)U'+\frac{\beta-3}{2}U=-\frac{P'}D,}
$$



$$
\boxed{(U-\xi)P'+\left[\gamma\left(U'+\frac{2U}{\xi}\right)-3\right]P=0.}
$$

Primes here mean $d/d\xi$. In the [pressure](../../../thermodynamics.md#pressure) equation the scale derivative $2q-\beta=-3$ explains the constant term. Once the profiles are found, their finite [energy](../../../classical-mechanics.md#energy) integral fixes $A$ through

$$
E=4\pi CR^{3-\beta}V^2\int_0^1\left[\frac12DU^2+\frac{P}{\gamma-1}\right]\xi^2\,d\xi.
$$

No global constant in $p/\rho^\gamma$ is assumed: the [shock wave](../../../partial-differential-equation.md#shock-wave) generates different [entropies](../../../thermodynamics.md#entropy) in shells swept up at different times.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Assume $\gamma>1$. The upstream [ideal gas](../../../thermodynamics.md#ideal-gas) is at rest in the laboratory frame and has [mass density](../../../fluid-mechanics.md#density) $\rho_1=CR^{-\beta}$. In the [shock frame](../../../compressible-flow.md#shock-frame) its incident speed is $V$. The strong-shock limit of the [Rankine-Hugoniot conditions for a perfect gas](../../../compressible-flow.md#rankine-hugoniot-conditions-for-a-perfect-gas) gives compression $\chi=(\gamma+1)/(\gamma-1)$ and downstream shock-frame speed $V/\chi$. Transforming back to the laboratory frame gives $u_2=V(1-1/\chi)=2V/(\gamma+1)$.

The normal momentum jump yields

$$
p_2+\rho_2(V-u_2)^2=\rho_1V^2,\qquad
p_2=\frac{2}{\gamma+1}\rho_1V^2,
$$

where the cold upstream [pressure](../../../thermodynamics.md#pressure) has been neglected. Thus the boundary values in the normalization of part (b) are

$$
\boxed{U(1)=\frac2{\gamma+1},\qquad
D(1)=\frac{\gamma+1}{\gamma-1},\qquad
P(1)=\frac2{\gamma+1}}.
$$

The [velocity](../../../classical-mechanics.md#velocity) jump uses the relative speed $V-u_2$, not the laboratory speed $u_2$. This distinction is essential to all three [shock wave](../../../partial-differential-equation.md#shock-wave) values.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Put $U=b\xi$ and $D=d\xi$. The [shock wave](../../../partial-differential-equation.md#shock-wave) conditions fix $b=2/(\gamma+1)$ and $d=(\gamma+1)/(\gamma-1)$. The [continuity equation](../../../physics.md#continuity-equation) then reduces to

$$
(b-1)+3b-\beta=0,
$$

so a linear [mass density](../../../fluid-mechanics.md#density) profile requires

$$
\boxed{\beta=4b-1=\frac{7-\gamma}{\gamma+1}}.
$$

Momentum requires $P'=-db(b-1+q)\xi^2$. At this exponent $q=-2(\gamma-1)/(\gamma+1)$, hence integration gives $P=2\xi^3/(\gamma+1)+P_0$. Substitution in the [pressure](../../../thermodynamics.md#pressure) equation makes the cubic coefficient vanish because $(\gamma+1)b=2$, while its constant term requires $(3\gamma b-3)P_0=0$. For $\gamma>1$ this implies $P_0=0$. Therefore all three equations and all [shock wave](../../../partial-differential-equation.md#shock-wave) conditions hold for the [linear-profile spherical blast wave](../../../compressible-flow.md#linear-profile-spherical-blast-wave),

$$
U=\frac{2\xi}{\gamma+1},\qquad
D=\frac{\gamma+1}{\gamma-1}\xi,\qquad
P=\frac{2\xi^3}{\gamma+1}.
$$

The prescribed range $0<\beta<3$ restricts this family to $1<\gamma<7$.

For $\gamma=5/3$ one has $\beta=2$, $a=2/3$, $U=3\xi/4$, $D=4\xi$ and $P=3\xi^3/4$. The [energy](../../../classical-mechanics.md#energy) integral is

$$
\int_0^1\left[\frac12DU^2+\frac{P}{\gamma-1}\right]\xi^2\,d\xi
=\int_0^1\frac94\xi^5\,d\xi=\frac38.
$$

Consequently $E=(3\pi/2)CR\dot R^2=(2\pi/3)CR^3/t^2$, which fixes the radius and dimensional fields completely:

$$
\boxed{R(t)=\left(\frac{3E}{2\pi C}\right)^{1/3}t^{2/3},\qquad
u(r,t)=\frac{r}{2t},}
$$



$$
\boxed{\rho(r,t)=\frac{4Cr}{R^3(t)}=\frac{8\pi C^2r}{3Et^2},\qquad
p(r,t)=\frac{Cr^3}{3R^3(t)t^2}=\frac{2\pi C^2r^3}{9Et^4},\quad 0<r<R(t)}.
$$

The [kinetic energy](../../../classical-mechanics.md#kinetic-energy) and [internal energy](../../../thermodynamics.md#internal-energy) integrands are each $9\xi^5/8$, so each accounts for half the explosion [energy](../../../classical-mechanics.md#energy). Integrating the [mass density](../../../fluid-mechanics.md#density) also gives the correct swept-up mass $4\pi CR$.

## 2

↑ **Parent:** [Paper 65](paper-65.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let the equilibrium [ideal gas](../../../thermodynamics.md#ideal-gas) be at rest, with uniform $\rho_0,p_0$ and $\mathbf B_0=B_0\mathbf e_z$. This local wave calculation neglects gravity, viscosity and magnetic diffusion. Define the [adiabatic sound speed](../../../compressible-flow.md#adiabatic-sound-speed) $c\equiv v_s=(\gamma p_0/\rho_0)^{1/2}$, the [Alfvén speed](../../../astrophysical-fluid-dynamics.md#alfven-speed) $v_a=B_0/(\mu_0\rho_0)^{1/2}$, and a [wavevector](../../../continuum-mechanics.md#wavevector) $\mathbf k=k(\sin\theta,0,\cos\theta)$, where $k=|\mathbf k|$ and $\theta$ is its angle to the equilibrium [magnetic field](../../../electromagnetism.md#magnetic-field). Perturbations have dependence $e^{i\mathbf k\cdot\mathbf x-i\omega t}$ and [phase speed](../../../wave-equation.md#phase-speed) $v=\omega/k$.

The [linearized ideal magnetohydrodynamic equations](../../../astrophysical-fluid-dynamics.md#linearized-ideal-magnetohydrodynamic-equations) for [mass conservation](../../../continuum-mechanics.md#mass-conservation), [pressure](../../../thermodynamics.md#pressure), induction and momentum give

$$
\delta\rho=\frac{\rho_0}{\omega}\mathbf k\cdot\mathbf u',\qquad
\delta p=c^2\delta\rho,\qquad
\mathbf b=\frac{\mathbf B_0(\mathbf k\cdot\mathbf u')-\mathbf u'(\mathbf k\cdot\mathbf B_0)}\omega,
$$



$$
\omega\rho_0\mathbf u'=\mathbf k\delta p-
\frac1{\mu_0}\left[(\mathbf k\cdot\mathbf B_0)\mathbf b-\mathbf k(\mathbf B_0\cdot\mathbf b)\right].
$$

The relation between [pressure](../../../thermodynamics.md#pressure) and [mass density](../../../fluid-mechanics.md#density) follows from eliminating $\mathbf k\cdot\mathbf u'$ between the two material evolution equations; it applies to the nonzero-frequency wave sector. The induction result automatically has $\mathbf k\cdot\mathbf b=0$.

The $y$ [MHD wave polarization](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-wave-polarization) is perpendicular to both the field and [wavevector](../../../continuum-mechanics.md#wavevector). It has $\delta p=\delta\rho=0$ and obeys

$$
\omega^2u'_y=v_a^2k^2\cos^2\theta\,u'_y.
$$

Thus the transverse [Alfvén wave](../../../astrophysical-fluid-dynamics.md#alfven-wave) has

$$
\boxed{v_A^2=v_a^2\cos^2\theta}.
$$

In the $x$-$z$ plane the two remaining [velocity](../../../classical-mechanics.md#velocity) components instead obey the [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) eigenproblem

$$
v^2\binom{u'_x}{u'_z}
=\begin{pmatrix}
v_a^2+c^2\sin^2\theta&c^2\sin\theta\cos\theta\\
c^2\sin\theta\cos\theta&c^2\cos^2\theta
\end{pmatrix}\binom{u'_x}{u'_z}.
$$

Taking its [determinant](../../../linear-algebra.md#determinant) gives $v^4-(c^2+v_a^2)v^2+c^2v_a^2\cos^2\theta=0$. Solving this [quadratic equation](../../../polynomial.md#quadratic-equation) in $v^2$ derives both [magnetoacoustic wave](../../../astrophysical-fluid-dynamics.md#magnetosonic-wave) [phase speeds](../../../wave-equation.md#phase-speed),

$$
\boxed{v_{f,\mathrm{slow}}^2=\frac{c^2+v_a^2}{2}\pm
\sqrt{\frac{(c^2+v_a^2)^2}{4}-c^2v_a^2\cos^2\theta}}.
$$

The plus sign is the [fast magnetosonic wave](../../../astrophysical-fluid-dynamics.md#fast-magnetosonic-wave), the minus sign the [slow magnetosonic wave](../../../astrophysical-fluid-dynamics.md#slow-magnetosonic-wave). The radicand is nonnegative, since it equals $[(c^2-v_a^2)^2+4c^2v_a^2\sin^2\theta]/4$. Both squared speeds are nonnegative. Each nonzero mode has forward and backward propagation; an advected [entropy](../../../thermodynamics.md#entropy) disturbance is a separate zero-frequency mode in this static equilibrium.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Set $\epsilon=v_a^2/c^2\ll1$. Expanding the [square root](../../../algebra.md#square-root) in part (a) gives

$$
\sqrt{(1+\epsilon)^2-4\epsilon\cos^2\theta}
=1+\epsilon(1-2\cos^2\theta)+O(\epsilon^2).
$$

Hence, to first absolute order in $\epsilon$,

$$
v_f^2=c^2+v_a^2\sin^2\theta+O(v_a^4/c^2),\qquad
v_{\rm slow}^2=v_a^2\cos^2\theta+O(v_a^4/c^2).
$$

The [high-pressure limit of magnetosonic waves](../../../astrophysical-fluid-dynamics.md#high-pressure-limit-of-magnetosonic-waves) can also be expressed as nonnegative speeds. Retaining the next squared-speed term gives the first relative correction for the slow mode:

$$
\boxed{v_f=c\left[1+\frac\epsilon2\sin^2\theta+O(\epsilon^2)\right],\qquad
v_{\rm slow}=v_a|\cos\theta|\left[1-\frac\epsilon2\sin^2\theta+O(\epsilon^2)\right]}.
$$

The exact [Alfvén speed](../../../astrophysical-fluid-dynamics.md#alfven-speed) along the propagation direction remains $v_a|\cos\theta|$.

The [fast magnetosonic wave](../../../astrophysical-fluid-dynamics.md#fast-magnetosonic-wave) is predominantly an [acoustic wave](../../../fluid-mechanics.md#acoustic-wave), with [velocity](../../../classical-mechanics.md#velocity) almost parallel to $\mathbf k$ and appreciable [mass density](../../../fluid-mechanics.md#density) and gas [pressure](../../../thermodynamics.md#pressure) variations. Its [magnetic pressure](../../../astrophysical-fluid-dynamics.md#magnetic-pressure) correction is weak. The [Alfvén wave](../../../astrophysical-fluid-dynamics.md#alfven-wave) is exactly incompressible, polarized perpendicular to the $\mathbf k$-$\mathbf B_0$ plane and restored by [magnetic tension](../../../astrophysical-fluid-dynamics.md#magnetic-tension).

The [slow magnetosonic wave](../../../astrophysical-fluid-dynamics.md#slow-magnetosonic-wave) is polarized inside that plane and almost perpendicular to $\mathbf k$. Indeed, the leading [sound speed](../../../compressible-flow.md#speed-of-sound) part of the matrix in (a) annihilates a vector perpendicular to $\mathbf k$, so only the smaller magnetic restoring force acts on that [MHD wave polarization](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-wave-polarization). Its compression is smaller by order $\epsilon$, with gas [pressure](../../../thermodynamics.md#pressure) changes almost cancelling [magnetic pressure](../../../astrophysical-fluid-dynamics.md#magnetic-pressure) changes. It is often called the [pseudo-Alfvén wave](../../../astrophysical-fluid-dynamics.md#pseudo-alfven-wave) [MHD wave polarization](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-wave-polarization) in this high [pressure](../../../thermodynamics.md#pressure) limit. Thus two distinct almost-incompressible magnetic [MHD wave polarizations](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-wave-polarization) have the same leading speed, while the third is predominantly sound. For exactly perpendicular propagation the [Alfvén wave](../../../astrophysical-fluid-dynamics.md#alfven-wave) and [slow magnetosonic wave](../../../astrophysical-fluid-dynamics.md#slow-magnetosonic-wave) frequencies vanish; for parallel propagation the two transverse magnetic [MHD wave polarizations](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-wave-polarization) are degenerate.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

Take $B_0=B_z>0$, $v_a=B_0/\sqrt{\mu_0\rho_0}$ and $\zeta=k(z-v_at)$. The transverse [ideal magnetohydrodynamic induction equation](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-induction-equation) and [magnetohydrodynamic momentum equation](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-momentum-equation) are satisfied by $u_x=-B_x/\sqrt{\mu_0\rho_0}$, $u_y=u_z=0$, with constant [mass density](../../../fluid-mechanics.md#density). However, the longitudinal [magnetohydrodynamic momentum equation](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-momentum-equation) also requires

$$
0=-\partial_z\left(p+\frac{B_x^2}{2\mu_0}\right).
$$

Here $B_x^2=a^2B_0^2\cos^2\zeta$ is not constant. Balancing its [gradient](../../../calculus.md#gradient) would require

$$
p=p_*(t)-\frac{a^2B_0^2}{2\mu_0}\cos^2\zeta.
$$

The adiabatic [pressure](../../../thermodynamics.md#pressure) equation instead gives $\partial_t p=0$, since this [velocity](../../../classical-mechanics.md#velocity) is divergence-free and has no component along the spatial variation. No choice of $p_*(t)$ removes the spatially varying time derivative. Thus **a nontrivial finite-amplitude linearly polarized sinusoidal [Alfvén wave](../../../astrophysical-fluid-dynamics.md#alfven-wave) is not an exact pure traveling wave in a compressible ideal fluid.** The [magnetic-pressure obstruction to a linearly polarized Alfvén wave](../../../astrophysical-fluid-dynamics.md#magnetic-pressure-obstruction-to-a-linearly-polarized-alfven-wave) is quadratic in $a$, so the wave is a valid linear approximation and drives a compressive response at higher order. In an incompressible model [pressure](../../../thermodynamics.md#pressure) is a constraint variable; it is not governed by the same compressible adiabatic evolution law.

Allowing longitudinal flow and varying [mass density](../../../fluid-mechanics.md#density) does not rescue a regular one-dimensional periodic traveling solution with precisely this transverse [magnetic field](../../../electromagnetism.md#magnetic-field). To see this, let $U=u_z-v_a$ and use the traveling coordinate. Integrated continuity, induction and transverse momentum give

$$
\rho U=m,\qquad UB_x-B_0u_x=A,\qquad
mu_x-\frac{B_0B_x}{\mu_0}=D,
$$

where $m,A,D$ are constants. Eliminating $u_x$ gives

$$
\left(\frac{m^2}{\rho}-\frac{B_0^2}{\mu_0}\right)B_x=mA+B_0D.
$$

At any zero of $B_x$, finite [mass density](../../../fluid-mechanics.md#density) and [velocity](../../../classical-mechanics.md#velocity) require the right side to vanish. Wherever $B_x\ne0$, the coefficient then vanishes and fixes $\rho=\mu_0m^2/B_0^2$, constant; continuity fixes $U$, and adiabatic [entropy](../../../thermodynamics.md#entropy) transport fixes $p$. The longitudinal [magnetohydrodynamic momentum equation](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-momentum-equation) again contradicts the varying $B_x^2$. The alternative $m=0$ makes transverse momentum force $B_x$ constant. Trivial cases such as $a=0$ or $k=0$ are excluded from the nontrivial wave conclusion.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

For the circular [MHD wave polarization](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-wave-polarization), $B_x^2+B_y^2=a^2B_0^2$ is constant. Choose any constant $\rho_0>0,p_0>0$, put $v_a=B_0/\sqrt{\mu_0\rho_0}$ and take

$$
\boxed{\mathbf u=-a v_a(\cos\zeta,\sin\zeta,0),\qquad
\rho=\rho_0,\qquad p=p_0,\qquad \zeta=k(z-v_at)}.
$$

This gives a [circularly polarized nonlinear Alfvén wave](../../../astrophysical-fluid-dynamics.md#circularly-polarized-nonlinear-alfven-wave) of arbitrary amplitude. All fields depend only on $z,t$, and $u_z=0$, so $\mathbf u\cdot\nabla\mathbf u=0$ and $\nabla\cdot\mathbf u=0$. Constant [mass density](../../../fluid-mechanics.md#density) and [pressure](../../../thermodynamics.md#pressure) then satisfy continuity and the adiabatic [pressure](../../../thermodynamics.md#pressure) equation, and $\nabla\cdot\mathbf B=0$ because $B_z$ is constant.

The remaining [ideal magnetohydrodynamic induction equation](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-induction-equation) and transverse [magnetohydrodynamic momentum equation](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-momentum-equation) are

$$
\partial_t\mathbf B_\perp=B_0\partial_z\mathbf u_\perp,\qquad
\rho_0\partial_t\mathbf u_\perp=\frac{B_0}{\mu_0}\partial_z\mathbf B_\perp.
$$

Since $\partial_t=-v_a\partial_z$ on the traveling profiles and $\mathbf u_\perp=-(v_a/B_0)\mathbf B_\perp$, both identities hold exactly when $v_a^2=B_0^2/(\mu_0\rho_0)$. The longitudinal [magnetohydrodynamic momentum equation](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-momentum-equation) holds because $p+|\mathbf B_\perp|^2/(2\mu_0)$ is constant. **The circularly polarized wave is therefore an exact nonlinear solution even though the fluid is compressible.** Compressibility permits [mass density](../../../fluid-mechanics.md#density) changes; it does not require every possible motion to compress the gas.

## 3

↑ **Parent:** [Paper 65](paper-65.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use a steady [axisymmetric flow](../../../fluid-mechanics.md#axisymmetric-flow) governed by [ideal magnetohydrodynamics](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamics) and take the [Newtonian gravitational potential](../../../classical-mechanics.md#newtonian-gravitational-potential) to be axisymmetric. Work locally on connected regular [magnetic flux](../../../electromagnetism.md#magnetic-flux) surfaces with nonzero poloidal flow. As usual for a wind without an imposed toroidal loop voltage, $E_\phi=0$; regularity on an included rotation axis guarantees this condition. It is needed to exclude steady cross-field flow in an annular domain.

Since $\nabla\phi=\mathbf e_\phi/R$, the [poloidal magnetic flux function](../../../astrophysical-fluid-dynamics.md#poloidal-magnetic-flux-function) gives

$$
\mathbf B_p=\frac1R\nabla\psi\times\mathbf e_\phi,
\qquad B_R=-\frac1R\partial_z\psi,\qquad
B_z=\frac1R\partial_R\psi,\qquad
\mathbf B_p\cdot\nabla\psi=0.
$$

The [poloidal magnetic field](../../../astrophysical-fluid-dynamics.md#poloidal-magnetic-field) is divergence-free. The zero toroidal [electric field](../../../electromagnetism.md#electric-field), with $\mathbf E=-\mathbf u\times\mathbf B$, gives $\mathbf u_p\parallel\mathbf B_p$. Define $k$ by $\rho\mathbf u_p=k\mathbf B_p$. Steady [mass conservation](../../../continuum-mechanics.md#mass-conservation) then gives

$$
0=\nabla\cdot(\rho\mathbf u_p)=\nabla\cdot(k\mathbf B_p)=\mathbf B_p\cdot\nabla k.
$$

Thus $k=k(\psi)$ is the [magnetohydrodynamic mass loading](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-mass-loading), the [mass flux](../../../physics.md#mass-flux) per unit poloidal [magnetic flux](../../../electromagnetism.md#magnetic-flux). Subtracting $(k/\rho)\mathbf B$ from the full [velocity](../../../classical-mechanics.md#velocity) leaves only an azimuthal component. The [cross product](../../../vector-space.md#cross-product) is

$$
\mathbf u\times\mathbf B
=\left(u_\phi-\frac{kB_\phi}{\rho}\right)\frac{\nabla\psi}{R}
\equiv\omega\nabla\psi.
$$

The steady [ideal magnetohydrodynamic induction equation](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-induction-equation) requires $0=\nabla\times(\omega\nabla\psi)=\nabla\omega\times\nabla\psi$. Consequently the [field-line angular velocity](../../../astrophysical-fluid-dynamics.md#field-line-angular-velocity) is $\omega=\omega(\psi)$ and

$$
\boxed{\mathbf u=\frac{k(\psi)\mathbf B}{\rho}+R\omega(\psi)\mathbf e_\phi}.
$$

Neither gas [pressure](../../../thermodynamics.md#pressure) nor axisymmetric gravity exerts an azimuthal [torque](../../../classical-mechanics.md#torque). Multiplying the azimuthal momentum equation by $R$ combines the cylindrical curvature terms into angular-momentum transport:

$$
\rho\mathbf u_p\cdot\nabla(Ru_\phi)
=\frac1{\mu_0}\mathbf B_p\cdot\nabla(RB_\phi).
$$

Insert $\rho\mathbf u_p=k\mathbf B_p$ and use $\mathbf B_p\cdot\nabla k=0$. It follows that

$$
\mathbf B_p\cdot\nabla\left[R\left(u_\phi-\frac{B_\phi}{\mu_0k}\right)\right]=0,
$$

so the [magnetohydrodynamic angular-momentum invariant](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-angular-momentum-invariant) is

$$
\boxed{u_\phi-\frac{B_\phi}{\mu_0k(\psi)}=\frac{\ell(\psi)}R}.
$$

The two terms account respectively for matter and [Maxwell stress tensor](../../../electromagnetism.md#maxwell-stress-tensor) transport of [angular momentum](../../../classical-mechanics.md#angular-momentum).

Finally, subtracting $\gamma$ times the logarithmic [mass density](../../../fluid-mechanics.md#density) equation from the logarithmic [pressure](../../../thermodynamics.md#pressure) equation gives $D\ln(p/\rho^\gamma)/Dt=0$. The [specific entropy](../../../thermodynamics.md#specific-entropy) of a fixed-composition [ideal gas](../../../thermodynamics.md#ideal-gas) is a function of $p/\rho^\gamma$. Steadiness and [axisymmetry](../../../calculus.md#axisymmetric-vector-field) reduce its advection to $\mathbf u_p\cdot\nabla s=0$. Hence

$$
\boxed{s=s(\psi),\qquad p=K(\psi)\rho^\gamma}.
$$

These flux-label functions are local on connected regular surfaces; disconnected components with the same numerical label need not share constants without an additional matching condition.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

On one [poloidal flux surface](../../../astrophysical-fluid-dynamics.md#axisymmetric-magnetic-flux-surface), the [field-line angular velocity](../../../astrophysical-fluid-dynamics.md#field-line-angular-velocity) $\omega(\psi)$ is constant. In a frame rotating at that rate the relative [velocity](../../../classical-mechanics.md#velocity) is $\mathbf v=\mathbf u-R\omega\mathbf e_\phi=k\mathbf B/\rho$, parallel to the [magnetic field](../../../electromagnetism.md#magnetic-field). The [Lorentz force](../../../electromagnetism.md#lorentz-force) is perpendicular to this motion, and the [Coriolis force](../../../physics.md#coriolis-force) also does no work. Centrifugal acceleration comes from the effective potential $-R^2\omega^2/2$. Since [entropy](../../../thermodynamics.md#entropy) is constant along the surface, [pressure](../../../thermodynamics.md#pressure) work integrates to [specific enthalpy](../../../thermodynamics.md#specific-enthalpy) $w$, with $dw=dp/\rho$ along the flow.

Therefore [kinetic energy](../../../classical-mechanics.md#kinetic-energy) relative to the rotating [poloidal flux surface](../../../astrophysical-fluid-dynamics.md#axisymmetric-magnetic-flux-surface), [enthalpy](../../../thermodynamics.md#enthalpy) and effective gravitational-plus-centrifugal potential have a constant sum:

$$
\boxed{\frac12|\mathbf u-R\omega\mathbf e_\phi|^2+w+\Phi-\frac12R^2\omega^2=\varepsilon(\psi)}.
$$

This is a corotating [energy](../../../classical-mechanics.md#energy) integral, not the laboratory [energy](../../../classical-mechanics.md#energy) alone: [Maxwell stress tensor](../../../electromagnetism.md#maxwell-stress-tensor) stresses can transfer [energy](../../../classical-mechanics.md#energy) and [angular momentum](../../../classical-mechanics.md#angular-momentum) in the laboratory frame. In fact the expression equals $|\mathbf u|^2/2+w+\Phi-\omega Ru_\phi$, namely the total [magnetohydrodynamic Bernoulli invariant](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-bernoulli-invariant) minus $\omega\ell$. Differential rotation between surfaces does not invalidate the argument, because the chosen [angular velocity](../../../classical-mechanics.md#angular-velocity) is fixed along the particular surface being followed.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

All invariants in this part refer to the selected [magnetic field line](../../../electromagnetism.md#magnetic-field-line). Its squared poloidal [Alfvén number](../../../astrophysical-fluid-dynamics.md#alfven-number) is

$$
M_{Ap}^2=\frac{\mu_0\rho u_p^2}{B_p^2}=\frac{\mu_0k^2}{\rho}.
$$

At the [Alfvén surface](../../../astrophysical-fluid-dynamics.md#alfven-surface) crossing it equals unity, so $\rho_a=\mu_0k^2$ and $M_{Ap}^2=1/y$. Subtract the two azimuthal integrals in part (a) to find

$$
R\omega-\frac\ell R=\frac{B_\phi}{\mu_0k}\left(1-\frac{\mu_0k^2}{\rho}\right),\qquad
v_\phi\equiv u_\phi-R\omega=\frac{R\omega-\ell/R}{y-1}.
$$

Finite azimuthal fields and [velocity](../../../classical-mechanics.md#velocity) at $y=1$ require the [Alfvén-surface regularity condition for an axisymmetric wind](../../../astrophysical-fluid-dynamics.md#alfven-surface-regularity-condition-for-an-axisymmetric-wind) $\ell=\omega R_a^2$. Hence

$$
v_\phi=\omega R_a\frac{x-x^{-1}}{y-1},\qquad
|u_p|=\frac{|k|C}{\rho_aR_a^2x^2y}
=\frac{C}{\sqrt{\mu_0\rho_a}R_a^2x^2y}.
$$

Here $v_\phi$ denotes the azimuthal [velocity](../../../classical-mechanics.md#velocity) relative to field-line rotation. For gravity of a [point mass](../../../classical-mechanics.md#point-mass) at $z=0$, $\Phi=-GM/R=-GM/(R_ax)$.

Insert these quantities in the corotating [energy](../../../classical-mechanics.md#energy) integral with $w=0$, and divide by the gravitational [energy](../../../classical-mechanics.md#energy) scale $GM/R_a$. This gives the [cold radial magnetohydrodynamic wind integral](../../../astrophysical-fluid-dynamics.md#cold-radial-magnetohydrodynamic-wind-integral),

$$
\boxed{f(x,y)=\frac\alpha2\left[\left(\frac{x-x^{-1}}{y-1}\right)^2-x^2\right]
+\frac\beta{2x^4y^2}-\frac1x=\frac{\varepsilon R_a}{GM}},
$$

with

$$
\boxed{\alpha=\frac{\omega^2R_a^3}{GM},\qquad
\beta=\frac{C^2}{\mu_0\rho_a GM R_a^3}}.
$$

Both are dimensionless. The apparent $0/0$ at $x=y=1$ must be evaluated on the smooth solution branch, not assigned an arbitrary value.

A constant-[energy](../../../classical-mechanics.md#energy) curve obeys $f_x+f_y\,dy/dx=0$. At a nondegenerate magnetosonic point, the vanishing coefficient of the [mass density](../../../fluid-mechanics.md#density) derivative requires simultaneous vanishing of its numerator:

$$
\boxed{f_y=0,\qquad f_x=0,\qquad f=f_{\rm wind}}.
$$

The curve must admit a real crossing slope. Expanding about such a point gives $f_{yy}m^2+2f_{xy}m+f_{xx}=0$, $m=dy/dx$, so a regular [saddle point of a scalar function](../../../analysis.md#saddle-point-of-a-scalar-function) crossing has $f_{xy}^2-f_{xx}f_{yy}>0$. These are the form of the slow and fast regularity conditions in a warm wind, with the [enthalpy](../../../thermodynamics.md#enthalpy) contribution retained in $f$.

In the strictly cold approximation used to obtain the displayed $f$, the slow speed is zero. There is a [cold-limit degeneracy of a slow magnetosonic point](../../../astrophysical-fluid-dynamics.md#cold-limit-degeneracy-of-a-slow-magnetosonic-point): a finite-speed interior slow crossing need not survive. Indeed,

$$
f_y=-\frac{\alpha(x-x^{-1})^2}{(y-1)^3}-\frac{\beta}{x^4y^3}<0\qquad(y>1,\ \beta>0),
$$

so this cold equation has no ordinary sub-Alfvénic slow critical point. A small retained [enthalpy](../../../thermodynamics.md#enthalpy) is needed to locate that point, which can approach the launching boundary as the [sound speed](../../../compressible-flow.md#speed-of-sound) tends to zero. The fast critical point still obeys the simultaneous conditions above wherever the reduced expression is nonsingular.

## 4

↑ **Parent:** [Paper 65](paper-65.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $\rho_0$ denote the midplane [mass density](../../../fluid-mechanics.md#density) and choose the symmetry plane at $z=0$. Isothermal [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) and the [Poisson equation for Newtonian gravity](../../../classical-mechanics.md#poisson-equation-for-newtonian-gravity) give

$$
c_s^2\frac{d\ln\rho}{dz}=-\frac{d\Phi_0}{dz},\qquad
\frac{d^2\Phi_0}{dz^2}=4\pi G\rho,
$$

so $c_s^2(d^2/dz^2)\ln\rho=-4\pi G\rho$. For $\rho=\rho_0\operatorname{sech}^2(z/H)$, direct differentiation yields

$$
\frac{d\ln\rho}{dz}=-\frac2H\tanh(z/H),\qquad
\frac{d^2\ln\rho}{dz^2}=-\frac2{H^2}\operatorname{sech}^2(z/H).
$$

Thus the profile is a [self-gravitating isothermal slab](../../../galaxy.md#self-gravitating-isothermal-slab) when $H^2=c_s^2/(2\pi G\rho_0)$. Integrating over both sides gives $\Sigma=2\rho_0H$, hence

$$
\boxed{H=\frac{c_s^2}{\pi G\Sigma},\qquad
\rho_0=\frac{\pi G\Sigma^2}{2c_s^2}}.
$$

The corresponding potential is $\Phi_0(z)-\Phi_0(0)=2c_s^2\ln\cosh(z/H)$, whose [gradient](../../../calculus.md#gradient) vanishes at the midplane and tends to $\pm2\pi G\Sigma$ far from the slab. The profile parameter $H$ is not its asymptotic exponential [mass density](../../../fluid-mechanics.md#density) [scale height](../../../statistical-physics.md#scale-height): that is $H/2$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

To distinguish [Eulerian and Lagrangian fluid perturbations](../../../fluid-mechanics.md#eulerian-and-lagrangian-fluid-perturbations), use $\boldsymbol\xi=(\xi_x,\xi_y,\xi_z)$ for the [fluid displacement](../../../fluid-mechanics.md#lagrangian-displacement-fluid-mechanics), $\phi=\Phi'$ for the Eulerian potential perturbation, and $\delta\rho$ for the Eulerian [mass density](../../../fluid-mechanics.md#density) perturbation. The equilibrium [mass density](../../../fluid-mechanics.md#density) $\rho(z)$ is the profile from part (a); subscript $z$ below denotes differentiation. Linearized [mass conservation](../../../continuum-mechanics.md#mass-conservation) and the [isothermal equation of state](../../../compressible-flow.md#globally-isothermal-equation-of-state) give

$$
\delta\rho=-ik\rho\xi_x-(\rho\xi_z)_z,\qquad
\delta p=c_s^2\delta\rho.
$$

The [velocity](../../../classical-mechanics.md#velocity) perturbation is $-i\omega\boldsymbol\xi$. Linearized momentum initially has the form

$$
-\omega^2\rho\boldsymbol\xi=-\nabla\delta p-\delta\rho\nabla\Phi_0-\rho\nabla\phi.
$$

Since $\nabla\Phi_0=-c_s^2\nabla\ln\rho$, the [pressure](../../../thermodynamics.md#pressure) and perturbed [mass density](../../../fluid-mechanics.md#density) gravity terms combine into $-\rho\nabla(c_s^2\delta\rho/\rho)$. Define $W=c_s^2\delta\rho/\rho+\phi$. The closed linearized system is

$$
\boxed{\omega^2\xi_x=ikW,\qquad \omega^2\xi_z=W_z,\qquad
\omega^2\xi_y=0,\qquad
\phi_{zz}-k^2\phi=4\pi G\delta\rho,\qquad
\delta\rho=-ik\rho\xi_x-(\rho\xi_z)_z}.
$$

The $y$ component is a neutral transverse sector; it vanishes for nonzero-frequency modes.

To prove reality rather than assume it, multiply momentum by $\rho\boldsymbol\xi^*$ and integrate over $z$. With $I=\int\rho|\boldsymbol\xi|^2dz>0$, [integration by parts](../../../calculus.md#integration-by-parts) and the conjugate [continuity equation](../../../physics.md#continuity-equation) give

$$
\omega^2I=\left[\rho\xi_z^*W\right]_{-\infty}^{\infty}
+c_s^2\int\frac{|\delta\rho|^2}{\rho}\,dz+\int\delta\rho^*\phi\,dz.
$$

Using the conjugate [Poisson equation for Newtonian gravity](../../../classical-mechanics.md#poisson-equation-for-newtonian-gravity) in the last integral gives

$$
\int\delta\rho^*\phi\,dz
=\frac1{4\pi G}\left[\phi\phi_z^*\right]_{-\infty}^{\infty}
-\frac1{4\pi G}\int(|\phi_z|^2+k^2|\phi|^2)\,dz.
$$

Take disturbances with finite $I$, finite [pressure](../../../thermodynamics.md#pressure) and gravitational integrals, and vanishing [pressure](../../../thermodynamics.md#pressure) work and gravitational boundary terms. For $k\ne0$, require the potential to decay at both infinities and the [fluid displacement](../../../fluid-mechanics.md#lagrangian-displacement-fluid-mechanics) to make $\rho\xi_z^*W\to0$ as well. In a source-free outer region the decaying potential is proportional to $e^{-|k||z|}$. The [isothermal displacement energy of a self-gravitating slab](../../../galaxy.md#isothermal-displacement-energy-of-a-self-gravitating-slab) then gives

$$
\boxed{\omega^2 I=c_s^2\int\frac{|\delta\rho|^2}{\rho}\,dz
-\frac1{4\pi G}\int(|\phi_z|^2+k^2|\phi|^2)\,dz\in\mathbb R}.
$$

Since $I$ is strictly positive for a nonzero displacement, **$\omega^2$ is real**. Positive values describe oscillations; negative values give pure growth and decay. The result is the [energy](../../../classical-mechanics.md#energy) identity for the pressure-gravity displacement operator, a [self-adjoint operator](../../../linear-operator-theory.md#self-adjoint-operator) in the [mass density](../../../fluid-mechanics.md#density)-weighted [inner product](../../../linear-algebra.md#inner-product). The identity excludes an oscillatory growing eigenmode under these [boundary conditions](../../../differential-equation.md#boundary-condition). At $k=0$ the same identity applies when its boundary terms vanish and its integrals remain finite, with the gravitational integral involving only $|\phi_z|^2$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Consider the nontrivial gravitational mode with $k\ne0$. At $\omega^2=0$, horizontal momentum requires $ikW=0$, hence $W=0$ and

$$
\delta\rho=-\frac{\rho}{c_s^2}\phi.
$$

Substituting into the [Poisson equation for Newtonian gravity](../../../classical-mechanics.md#poisson-equation-for-newtonian-gravity) and using $4\pi G\rho_0/c_s^2=2/H^2$ gives

$$
\phi_{zz}+\left[\frac2{H^2}\operatorname{sech}^2(z/H)-k^2\right]\phi=0.
$$

Set $\tau=\tanh(z/H)$ and $\nu=kH$. Since $\partial_z=(1-\tau^2)\partial_\tau/H$, this becomes the [associated Legendre equation](../../../differential-equation.md#associated-legendre-differential-equation) of degree one and order $\nu$:

$$
\boxed{\frac d{d\tau}\left[(1-\tau^2)\frac{d\phi}{d\tau}\right]
+\left[2-\frac{\nu^2}{1-\tau^2}\right]\phi=0}.
$$

To verify the two explicit solutions, put $\eta=z/H$ and $T=\tanh\eta$. They are

$$
F_+=e^{\nu\eta}(\nu-T),\qquad F_-=e^{-\nu\eta}(\nu+T),
$$

because $e^{2\eta}=(1+\tau)/(1-\tau)$. Differentiating $F_+$ twice gives

$$
(F_+)_{\eta\eta}=e^{\nu\eta}\left[\nu^2(\nu-T)-2\nu(1-T^2)+2T(1-T^2)\right],
$$

which cancels identically against $[2(1-T^2)-\nu^2]F_+$. Reflection $\eta\mapsto-\eta$ proves the same for $F_-$. Their [Wronskian](../../../differential-equation.md#wronskian) is $2\nu(1-\nu^2)$, evaluated at $\eta=0$; thus they are generally independent but coincide or become dependent at the exceptional orders $0,\pm1$.

Use $n=|k|H>0$ to analyze decay, which is unaffected by the sign of $k$. The solution decaying at $+\infty$ is proportional to $e^{-n\eta}(n+\tanh\eta)$. At $-\infty$ its leading term is $(n-1)e^{n|\eta|}$, so it also decays there only if $n=1$. At this value

$$
e^{-\eta}(1+\tanh\eta)=e^{\eta}(1-\tanh\eta)=\operatorname{sech}\eta.
$$

Therefore the [marginal fragmentation mode of an isothermal slab](../../../galaxy.md#marginal-fragmentation-mode-of-an-isothermal-slab) has

$$
\boxed{|k|=\frac1H,\qquad \Phi'=\phi\propto\operatorname{sech}(z/H),\qquad
\delta\rho\propto\operatorname{sech}^3(z/H)}.
$$

At $n=1$ the second independent solution obtained by [reduction of order](../../../differential-equation.md#reduction-of-order) grows at infinity, so the coincidence of the two explicit formulas does not supply an extra admissible mode. At $k=0$ a uniform vertical translation gives another neutral disturbance, and mass-preserving relabeling displacements can have $\delta\rho=\phi=0$. Neither is the nonzero-[wavenumber](../../../wave-equation.md#wavenumber) fragmentation threshold just calculated.

**The unstable fragmentation modes have wavelengths greater than $2\pi H$.** Gas-[pressure](../../../thermodynamics.md#pressure) support becomes less effective relative to [self-gravity](../../../classical-mechanics.md#self-gravity) at long wavelength. The side of the threshold can also be checked from the [energy](../../../classical-mechanics.md#energy) identity: at $|k|=1/H$ the marginal [mass density](../../../fluid-mechanics.md#density) disturbance has zero quadratic [energy](../../../classical-mechanics.md#energy). Keep that [mass density](../../../fluid-mechanics.md#density) disturbance and decrease $|k|$; the [pressure](../../../thermodynamics.md#pressure) integral stays fixed, while the gravitational term becomes more negative because the positive inverse operator $(-\partial_z^2+k^2)^{-1}$ increases as $k^2$ decreases. Thus the quadratic [energy](../../../classical-mechanics.md#energy) becomes negative, giving an unstable mode on the longer-wavelength side. This argument concerns the gravitational sector and its stated decay conditions.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
