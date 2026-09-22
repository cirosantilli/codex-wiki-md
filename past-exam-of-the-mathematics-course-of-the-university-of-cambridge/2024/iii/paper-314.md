# Paper 314

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_314.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_314.pdf)

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

## 1

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

In a [magnetostatic equilibrium](../../../electromagnetism.md#magnetostatic-equilibrium), inertia is absent and all forces balance. A [force-free magnetic field](../../../astrophysical-fluid-dynamics.md#force-free-magnetic-field) is the limiting case in which the [Lorentz force density](../../../electromagnetism.md#lorentz-force-density) vanishes:

$$
\frac1c\mathbf j\times\mathbf B=0.
$$

Thus the [current density](../../../electromagnetism.md#current-density) is parallel to the [magnetic field](../../../electromagnetism.md#magnetic-field), so for some scalar [force-free parameter](../../../astrophysical-fluid-dynamics.md#force-free-parameter) $\alpha(\mathbf r)$,

$$
\mathbf j=\alpha\mathbf B.
$$

Using [Ampère's law](../../../electromagnetism.md#ampere-s-circuital-law) in magnetostatics gives

$$
\boxed{\nabla\times\mathbf B=\frac{4\pi}{c}\alpha\mathbf B}.
$$

Taking the [divergence](../../../calculus.md#divergence) and using both the [divergence of a curl is zero](../../../calculus.md#divergence-of-a-curl-is-zero) and $\nabla\mathbin\cdot\mathbf B=0$ yields

$$
0=\nabla\mathbin\cdot(\alpha\mathbf B)
=\mathbf B\mathbin\cdot\nabla\alpha,
$$

so

$$
\boxed{\mathbf B\mathbin\cdot\nabla\alpha=0}.
$$

The [force-free parameter](../../../astrophysical-fluid-dynamics.md#force-free-parameter) is therefore constant along every [magnetic field line](../../../electromagnetism.md#magnetic-field-line).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put

$$
q(R)=\frac{4\pi\alpha(R)}c.
$$

For an [axisymmetric vector field](../../../calculus.md#axisymmetric-vector-field) depending only on the [cylindrical radius](../../../calculus.md#cylindrical-radius) $R$, the [solenoidal vector field](../../../calculus.md#solenoidal-vector-field) condition is

$$
\frac1R\frac{d}{dR}(RB_R)=0.
$$

Hence $RB_R$ is constant. The hypothesis $B_R\to0$ on the axis forces

$$
\boxed{B_R=0}.
$$

The azimuthal and axial components of $\nabla\times\mathbf B=q\mathbf B$ are then

$$
-\frac{dB_z}{dR}=qB_\phi,
\qquad
\frac1R\frac{d}{dR}(RB_\phi)=qB_z.
$$

Eliminating $B_\phi=-B_z'/q$ gives the closed [ordinary differential equation](../../../differential-equation.md#ordinary-differential-equation)

$$
\boxed{B_z''+\left(\frac1R-\frac{q'}q\right)B_z'+q^2B_z=0},
\qquad q=\frac{4\pi\alpha}{c}.
$$

Once $B_z$ is known, $B_\phi=-B_z'/q$ and $B_R=0$ determine the full [cylindrical force-free magnetic field](../../../astrophysical-fluid-dynamics.md#cylindrical-force-free-magnetic-field).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Here $q=\kappa/R$, so the equation from part (b) becomes the [Euler-Cauchy equation](../../../differential-equation.md#euler-cauchy-equation)

$$
B_z''+\frac2R B_z'+\frac{\kappa^2}{R^2}B_z=0.
$$

The [power-law ansatz](../../../differential-equation.md#power-law-ansatz) $B_z=R^s$ gives the [indicial equation](../../../differential-equation.md#indicial-equation)

$$
s^2+s+\kappa^2=0,
\qquad
s_\pm=\frac{-1\pm\sqrt{1-4\kappa^2}}2.
$$

For $0<\kappa<1/2$, the general field is therefore

$$
\boxed{B_R=0,\qquad
B_z=C_+R^{s_+}+C_-R^{s_-},\qquad
B_\phi=-\frac1\kappa
\left(s_+C_+R^{s_+}+s_-C_-R^{s_-}\right)}.
$$

The [polynomial discriminant](../../../galois-theory.md#polynomial-discriminant) changes sign at

$$
\boxed{\kappa_c=\frac12}.
$$

For $\kappa>\kappa_c$, define $\mu=\sqrt{\kappa^2-1/4}$. A real form of the solution is

$$
B_z=R^{-1/2}\left[C\cos\!\left(\mu\ln\frac R{R_0}\right)
+D\sin\!\left(\mu\ln\frac R{R_0}\right)\right],
\qquad
B_\phi=-\frac R\kappa\frac{dB_z}{dR},
\qquad B_R=0.
$$

**Thus the field has a [log-periodic oscillation](../../../differential-equation.md#log-periodic-oscillation): its phase is periodic in $\ln R$, so it oscillates as the radius changes geometrically.**

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

At $\kappa=\kappa_c=1/2$, the [indicial equation](../../../differential-equation.md#indicial-equation) has the [multiple root](../../../polynomial.md#multiple-root) $s=-1/2$. The general axial component is

$$
\boxed{B_z=R^{-1/2}\left(C+D\ln\frac R{R_0}\right)}.
$$

Since $B_\phi=-2R B_z'$, the azimuthal component is

$$
\boxed{B_\phi=R^{-1/2}
\left(C+D\ln\frac R{R_0}-2D\right)},
\qquad B_R=0.
$$

Consequently

$$
\frac{B_\phi}{B_z}
=1-\frac{2D}{C+D\ln(R/R_0)}\longrightarrow1
$$

as $R\to\infty$; the same ratio is identically one when $D=0$. A [magnetic field line](../../../electromagnetism.md#magnetic-field-line) has tangent parallel to $\mathbf B$, so its asymptotic angle $\vartheta$ with the $z$-axis satisfies

$$
\tan\vartheta=\left|\frac{B_\phi}{B_z}\right|\longrightarrow1.
$$

Hence the field lines become helices making the constant angle

$$
\boxed{\vartheta=\frac\pi4=45^\circ}
$$

with the axis.

## 2

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $u(r)>0$ denote the inward [radial velocity](../../../fluid-mechanics.md#radial-velocity). Steady [spherical symmetry](../../../geometry-and-topology.md#spherical-symmetry) and [mass conservation](../../../continuum-mechanics.md#mass-conservation) give

$$
\dot M=4\pi r^2\rho u=\text{constant}.
$$

The radial [Euler momentum equation](../../../fluid-mechanics.md#euler-equations-for-an-inviscid-fluid) for the [globally isothermal equation of state](../../../compressible-flow.md#globally-isothermal-equation-of-state) $p=c_s^2\rho$ is

$$
u\frac{du}{dr}=-c_s^2\frac1\rho\frac{d\rho}{dr}-\frac{GM}{r^2}.
$$

The logarithmic derivative of mass conservation is $\rho'/\rho=-u'/u-2/r$. Substitution gives the [Isothermal Bondi equation](../../../astrophysics.md#isothermal-bondi-equation)

$$
\boxed{\left(u-\frac{c_s^2}{u}\right)\frac{du}{dr}
=\frac{2c_s^2}{r}-\frac{GM}{r^2}}.
$$

At a smooth [sonic point](../../../compressible-flow.md#sonic-point), $u=c_s$ makes the coefficient of $u'$ vanish, so the right-hand side must vanish too. Therefore

$$
\boxed{r_s=\frac{GM}{2c_s^2}}.
$$

The solution that crosses this [critical point of the isothermal Bondi equation](../../../astrophysics.md#critical-point-of-the-isothermal-bondi-equation) continuously is the transonic accretion solution.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The radial equation can be written

$$
\frac{d}{dr}\left(\frac{u^2}{2}
+c_s^2\ln\rho-\frac{GM}{r}\right)=0.
$$

Thus the [Bernoulli function](../../../fluid-mechanics.md#bernoulli-function) is constant on each [streamline](../../../fluid-mechanics.md#streamline):

$$
\boxed{\mathcal B=\frac{u^2}{2}+c_s^2\ln\rho+\Phi},
\qquad
\Phi=-\frac{GM}{r}.
$$

The boundary conditions $u\to0$ and $\rho\to\rho_0$ as $r\to\infty$ fix $\mathcal B=c_s^2\ln\rho_0$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

At the [Bondi sonic point](../../../astrophysics.md#bondi-sonic-point), $u_s=c_s$ and $GM/r_s=2c_s^2$. Evaluating the [Bernoulli function](../../../fluid-mechanics.md#bernoulli-function) there gives

$$
\frac{c_s^2}{2}+c_s^2\ln\rho_s-2c_s^2
=c_s^2\ln\rho_0,
$$

and hence

$$
\rho_s=e^{3/2}\rho_0.
$$

The conserved [mass accretion rate](../../../astrophysics.md#mass-accretion-rate) is therefore

$$
\dot M=4\pi r_s^2\rho_sc_s
=\pi e^{3/2}\rho_0\frac{(GM)^2}{c_s^3}.
$$

Thus

$$
\boxed{A=\pi e^{3/2}}.
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

With the [dimensionless variables](../../../mathematics.md#dimensionless-variable) $x=r/r_s$ and $y=u/c_s$, [mass conservation](../../../continuum-mechanics.md#mass-conservation) and part (c) give

$$
\frac\rho{\rho_0}=\frac{e^{3/2}}{x^2y}.
$$

Substitution into the [Bernoulli function](../../../fluid-mechanics.md#bernoulli-function), together with $GM/r=2c_s^2/x$, eliminates every dimensional parameter and gives the [transcendental equation](../../../mathematics.md#transcendental-equation)

$$
\boxed{\frac{y^2}{2}-\ln y-2\ln x+\frac32-\frac2x=0}.
$$

Equivalently,

$$
\boxed{y^2-\ln(y^2)=\frac4x+4\ln x-3},
$$

or

$$
\boxed{y^2e^{-y^2}=x^{-4}e^{3-4/x}}.
$$

The [transonic branch](../../../compressible-flow.md#transonic-branch) passes through $(x,y)=(1,1)$.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Put $Y=y^2$. On the inner supersonic branch, the equation from part (d) is

$$
Y-\ln Y=\frac4x+4\ln x-3.
$$

Its [asymptotic expansion](../../../analysis.md#asymptotic-expansion) as $x\to0^+$ begins

$$
Y=\frac4x+3\ln x+\ln4-3+O(x\ln x).
$$

Taking the positive [square root](../../../algebra.md#square-root) gives

$$
y=\frac2{\sqrt x}
\left[1+\frac x8\left(3\ln x+\ln4-3\right)
+O\!\left(x^2\ln^2x\right)\right].
$$

Since $x=r/r_s$ and $y=u/c_s$,

$$
\boxed{u(r)=2c_s\sqrt{\frac{r_s}{r}}
\left[1+\frac{r}{8r_s}
\left(3\ln\frac r{r_s}+\ln4-3\right)
+O\!\left(\frac{r^2}{r_s^2}\ln^2\frac r{r_s}\right)\right]}.
$$

The leading term is the [free-fall speed](../../../astrophysics.md#free-fall-speed) $\sqrt{2GM/r}$; the logarithmic term is the first pressure correction to the inner [Isothermal Bondi accretion](../../../astrophysics.md#isothermal-bondi-accretion) flow.

## 3

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

In the wing frame the unperturbed plasma moves with velocity $-u_0\mathbf e_x$. The [ideal magnetohydrodynamics](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamics) condition $\mathbf E+\mathbf u\times\mathbf B/c=0$ therefore produces the [motional electric field](../../../electromagnetism.md#motional-electric-field)

$$
\mathbf E=-\frac{(-u_0\mathbf e_x)\times(B_0\mathbf e_z)}c
=-\frac{u_0B_0}{c}\mathbf e_y.
$$

The wing's [surface conductivity](../../../electromagnetism.md#surface-conductivity) then gives the [surface current density](../../../electromagnetism.md#surface-current-density)

$$
\boxed{\mathbf J=\Sigma\mathbf E
=-\frac{\Sigma u_0B_0}{c}\mathbf e_y}.
$$

Its direction also follows directly from the [Lorentz force](../../../electromagnetism.md#lorentz-force) on the wing's mobile charges.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The wing and its forcing are time independent in the co-moving frame, so after transients have propagated away the perturbation is stationary there. Write the background velocity and field as

$$
\mathbf U=-u_0\mathbf e_x,
\qquad
\mathbf B_0=B_0\mathbf e_z,
$$

and take every perturbation to be independent of $y$. The cold-plasma [linearized ideal magnetohydrodynamic equations](../../../astrophysical-fluid-dynamics.md#linearized-ideal-magnetohydrodynamic-equations) are

$$
-\rho_0u_0\partial_x\delta\mathbf u
=\frac1{4\pi}(\nabla\times\delta\mathbf B)\times\mathbf B_0,
$$



$$
-u_0\partial_x\delta\mathbf B
=(\mathbf B_0\mathbin\cdot\nabla)\delta\mathbf u
-\mathbf B_0\nabla\mathbin\cdot\delta\mathbf u.
$$

Their relevant components are

$$
-\rho_0u_0\partial_x\delta u_x
=\frac{B_0}{4\pi}
(\partial_z\delta B_x-\partial_x\delta B_z),
$$



$$
-u_0\partial_x\delta B_x=B_0\partial_z\delta u_x,
\qquad
-u_0\partial_x\delta B_z=-B_0\partial_x\delta u_x.
$$

Differentiate the momentum equation with respect to $x$ and use the two induction relations. With the [Alfvén speed](../../../astrophysical-fluid-dynamics.md#alfven-speed)

$$
u_A^2=\frac{B_0^2}{4\pi\rho_0},
$$

the result is

$$
\boxed{(u_A^2-u_0^2)\frac{\partial^2\delta u_x}{\partial x^2}
+u_A^2\frac{\partial^2\delta u_x}{\partial z^2}=0}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Integrating the $y$ component of [Ampère's law](../../../electromagnetism.md#ampere-s-circuital-law),

$$
\partial_zB_x-\partial_xB_z=\frac{4\pi}{c}j_y,
$$

through the [current sheet](../../../electromagnetism.md#current-sheet) gives the [magnetic-field jump across a surface current](../../../electromagnetism.md#magnetic-field-jump-across-a-surface-current)

$$
\boxed{\delta B_x(0^+)-\delta B_x(0^-)
=\frac{4\pi}{c}J_y
=-\frac{4\pi\Sigma u_0B_0}{c^2}}.
$$

Reflection in the wing plane reverses the tangential perturbation $\delta B_x$. If

$$
b=\frac{2\pi\Sigma u_0B_0}{c^2},
$$

the upper and lower boundary values on the wing are consequently

$$
\boxed{\delta B_x(x,0^+)=-b,
\qquad
\delta B_x(x,0^-)=b,
\qquad |x|<\frac L2}.
$$

Outside the wing, the corresponding boundary value is zero.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For $u_0>u_A$, define the [Alfvénic Mach-cone slope](../../../astrophysical-fluid-dynamics.md#alfvenic-mach-cone-slope)

$$
m=\sqrt{\frac{u_0^2}{u_A^2}-1}
\simeq\frac{u_0}{u_A}.
$$

The equation in part (b) is the [hyperbolic partial differential equation](../../../partial-differential-equation.md#hyperbolic-partial-differential-equation)

$$
\partial_z^2\delta u_x-m^2\partial_x^2\delta u_x=0,
$$

whose [characteristic curves](../../../partial-differential-equation.md#characteristic-curve) are $x\pm mz=\text{constant}$. Let $W(s)$ be one for $|s|<L/2$ and zero otherwise. Selecting the characteristics that trail downstream, toward negative $x$, and imposing part (c) gives

$$
\boxed{\delta B_x=-\operatorname{sgn}(z)bW(x+m|z|)}.
$$

The stationary induction and [mass conservation](../../../continuum-mechanics.md#mass-conservation) equations then give

$$
\boxed{\delta u_x=\frac{u_0b}{mB_0}W(x+m|z|)},
$$



$$
\boxed{\delta B_z=\frac b mW(x+m|z|),
\qquad
\delta\rho=\frac{\rho_0b}{mB_0}W(x+m|z|)},
$$

with $\delta u_z=\delta u_y=\delta B_y=0$. In the strongly super-Alfvénic limit, $\delta u_x\simeq u_Ab/B_0$ and $\delta B_z\simeq bu_A/u_0$ inside the disturbed region.

The perturbations have support only where

$$
\boxed{|x+m|z||<\frac L2}.
$$

Because the wing is infinite in $y$, this is the union of two inclined slabs bounded by the [characteristic planes](../../../partial-differential-equation.md#characteristic-plane) $x+m|z|=\pm L/2$. These two trailing slabs are the [Alfvén wings](../../../astrophysical-fluid-dynamics.md#alfven-wing) generated by the conductor.

## 4

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The given velocity is a [homologous spherical flow](../../../fluid-mechanics.md#homologous-spherical-flow),

$$
\mathbf u=q(t)\mathbf r,
\qquad q(t)=\frac{u_0(t)}{R(t)},
$$

with the spatially uniform [velocity divergence](../../../continuum-mechanics.md#velocity-divergence)

$$
\nabla\mathbin\cdot\mathbf u=3q>0.
$$

Every shocked [fluid element](../../../continuum-mechanics.md#fluid-element) therefore expands rather than undergoing continued compression, and the velocity fills the remnant smoothly instead of concentrating its mass in a thin cooling shell. In the absence of radiative losses, the [entropy advection equation](../../../astrophysical-fluid-dynamics.md#entropy-advection-equation) then makes each element follow an [adiabatic process](../../../thermodynamics.md#adiabatic-process) after its one entropy-producing passage through the shock. This broad expanding structure is the expected [adiabatic phase of a supernova remnant](../../../galaxy.md#adiabatic-phase-of-a-supernova-remnant).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [Strong-shock Rankine-Hugoniot conditions](../../../compressible-flow.md#strong-shock-rankine-hugoniot-conditions) give the compression ratio

$$
\frac{\rho_2}{\rho_0}=\frac{\gamma+1}{\gamma-1}=4
$$

for $\gamma=5/3$. Thus

$$
\boxed{\rho(R(t),t)=4\rho_0}.
$$

In the shock frame, [mass conservation](../../../continuum-mechanics.md#mass-conservation) says

$$
\rho_0\dot R=\rho_2(\dot R-u_0).
$$

Using $\rho_2=4\rho_0$ gives

$$
\boxed{u_0(t)=\frac34\dot R(t)}.
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Resolve the upstream uniform field $\mathbf B_0=B_0\mathbf e_z$ into components normal and tangential to the spherical shock:

$$
B_{r,1}=B_0\cos\theta,
\qquad
B_{\theta,1}=-B_0\sin\theta,
\qquad B_{\phi,1}=0.
$$

The [ideal magnetohydrodynamic shock conditions](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-shock-conditions) preserve the normal magnetic component and multiply the tangential component of a weak passive field by the gas compression ratio. Part (b) therefore gives

$$
\boxed{B_r(R,\theta,t)=B_0\cos\theta,
\qquad
B_\theta(R,\theta,t)=-4B_0\sin\theta,
\qquad
B_\phi=0}.
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For the [homologous spherical flow](../../../fluid-mechanics.md#homologous-spherical-flow) $\mathbf u=q\mathbf r$, the [ideal magnetohydrodynamic induction equation](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-induction-equation) and $\nabla\mathbin\cdot\mathbf B=0$ give the [material derivative](../../../continuum-mechanics.md#material-derivative)

$$
\frac{D\mathbf B}{Dt}
=(\mathbf B\mathbin\cdot\nabla)\mathbf u
-\mathbf B\nabla\mathbin\cdot\mathbf u
=-2q\mathbf B.
$$

Let $x=r/R(t)$ and use the [self-similar ansatz](../../../fluid-mechanics.md#self-similar-ansatz)

$$
B_r=B_0f(x)\cos\theta,
\qquad
B_\theta=-B_0g(x)\sin\theta.
$$

Part (b) gives $q=3\dot R/(4R)$, and therefore

$$
\frac{Dx}{Dt}=x\left(q-\frac{\dot R}{R}\right)
=-\frac14\frac{\dot R}{R}x.
$$

The radial induction equation becomes $xf'=6f$. The boundary value $f(1)=1$ gives $f=x^6$. The [solenoidal vector field](../../../calculus.md#solenoidal-vector-field) condition requires

$$
g=f+\frac x2f'=4x^6,
$$

which also matches the tangential shock value in part (c). Hence the interior field is

$$
\boxed{B_r=B_0\left(\frac rR\right)^6\cos\theta,
\qquad
B_\theta=-4B_0\left(\frac rR\right)^6\sin\theta,
\qquad B_\phi=0}.
$$

Outside the shock, the uniform-field lines obey $r\sin\theta=\text{constant}$. Inside, the [magnetic-field-line equation](../../../electromagnetism.md#magnetic-field-line-equation) gives

$$
\frac{dr}{r\,d\theta}=\frac{B_r}{B_\theta}
=-\frac14\cot\theta,
$$

so

$$
\boxed{r^4\sin\theta=\text{constant}}.
$$

A sketch therefore shows straight exterior lines refracting at the spherical shock into north-south symmetric curves that bow toward the equatorial interior before leaving through the opposite hemisphere. The field strength falls as $r^6$ toward the centre.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
