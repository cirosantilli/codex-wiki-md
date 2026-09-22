# Paper 314

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_314.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_314.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
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

In the inertial frame, rigid corotation gives $\mathbf u=\boldsymbol\Omega\mathbin\times\mathbf r$. The [ideal magnetohydrodynamics](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamics) condition is the [motional electric field](../../../electromagnetism.md#motional-electric-field)

$$
\mathbf E=-\frac{\mathbf u\mathbin\times\mathbf B_0}{c}.
$$

Apply [Gauss's law](../../../electromagnetism.md#gauss-s-law) in Gaussian units and use the [divergence and curl of a cross product](../../../calculus.md#divergence-and-curl-of-a-cross-product):

$$
4\pi n_q=\nabla\mathbin\cdot\mathbf E
=-\frac1c\left[\mathbf B_0\mathbin\cdot(\nabla\mathbin\times\mathbf u)-\mathbf u\mathbin\cdot(\nabla\mathbin\times\mathbf B_0)\right].
$$

The exterior field is produced by currents inside the star, so $\nabla\mathbin\times\mathbf B_0=0$ there, while rotation with constant [angular velocity](../../../classical-mechanics.md#angular-velocity) has $\nabla\mathbin\times\mathbf u=2\boldsymbol\Omega$. Hence the required [Goldreich-Julian charge density](../../../stellar-astrophysics.md#goldreich-julian-density) is

$$
\boxed{n_q(\mathbf r)=-\frac{\boldsymbol\Omega\mathbin\cdot\mathbf B_0(\mathbf r)}{2\pi c}}.
$$

Here $n_q$ denotes electric charge per unit volume, as in the question. If each carrier has charge $q$, its signed number density is $n_q/q$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

For the aligned [magnetic dipole field](../../../electromagnetism.md#magnetic-dipole-field),

$$
B_r=\frac{2\mu\cos\theta}{r^3},
\qquad
B_\theta=\frac{\mu\sin\theta}{r^3}.
$$

Since $\mathbf e_z=\cos\theta\,\mathbf e_r-\sin\theta\,\mathbf e_\theta$,

$$
\boldsymbol\Omega\mathbin\cdot\mathbf B_0
=\frac{\Omega\mu}{r^3}(3\cos^2\theta-1).
$$

The corotation velocity is $\mathbf u=\Omega r\sin\theta\,\mathbf e_\phi$. The [current density](../../../electromagnetism.md#current-density) is therefore the advected [charge density](../../../electromagnetism.md#charge-density),

$$
\boxed{
\mathbf j=n_q\mathbf u
=-\frac{\Omega^2\mu}{2\pi c r^2}
\sin\theta(3\cos^2\theta-1)\,\mathbf e_\phi}.
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

In the midplane, the vacuum [magnetic dipole field](../../../electromagnetism.md#magnetic-dipole-field) has scale $B_0\sim\mu/r^3$, while the result of part i gives $j\sim\Omega^2\mu/(cr^2)$. [Ampère's law](../../../electromagnetism.md#ampere-s-circuital-law) then gives the induced-field estimate

$$
\frac{B_i}{r}\sim\frac{j}{c},
\qquad
B_i\sim\frac{\Omega^2\mu}{c^2r},
$$

where numerical factors are immaterial in this [dimensional analysis](../../../physics.md#dimensional-analysis). Thus $B_i\sim B_0$ at

$$
\boxed{R_e\sim\frac c\Omega}.
$$

This is the [light cylinder radius](../../../stellar-astrophysics.md#light-cylinder-radius): rigid corotation would have $u=\Omega R_e\sim c$. The nonrelativistic approximation and the assumed unmodified vacuum field therefore fail at the same scale, and a self-consistent [pulsar magnetosphere](../../../stellar-astrophysics.md#pulsar-magnetosphere) must replace them.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

The [magnetic-field-line equation](../../../electromagnetism.md#magnetic-field-line-equation) for the dipole is

$$
\frac{dr}{r\,d\theta}=\frac{B_r}{B_\theta}=2\cot\theta.
$$

Integration gives the [dipole magnetic-field line](../../../electromagnetism.md#dipole-magnetic-field-line)

$$
r=C\sin^2\theta.
$$

The line crosses the midplane at $r=R_e$, so $C=R_e$. At the stellar surface,

$$
R_*=R_e\sin^2\theta_*.
$$

Consequently

$$
\boxed{\theta_*=\arcsin\sqrt{\frac{R_*}{R_e}}}
\simeq\sqrt{\frac{\Omega R_*}{c}}
$$

for a small [polar-cap opening angle](../../../stellar-astrophysics.md#polar-cap-opening-angle).

## 2

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

The collapse is perpendicular to the initial field, so [magnetic flux freezing](../../../astrophysical-fluid-dynamics.md#magnetic-flux-freezing) preserves the [mass-to-flux ratio](../../../astrophysical-fluid-dynamics.md#mass-to-flux-ratio) of each material flux tube:

$$
\frac{B_z}{\rho}=\frac{B_0}{\rho_0},
\qquad
B_z=\frac{B_0}{\rho_0}\rho.
$$

With no toroidal field, radial [magnetostatic equilibrium](../../../electromagnetism.md#magnetostatic-equilibrium) is

$$
\frac d{dR}\left(P+\frac{B_z^2}{8\pi}\right)
=-\rho\frac{d\Phi}{dR}.
$$

Define the effective polytropic constant

$$
K_{m eff}=K+\frac{B_0^2}{8\pi\rho_0^2}.
$$

Then gas and [magnetic pressure](../../../astrophysical-fluid-dynamics.md#magnetic-pressure) combine as $P+B_z^2/(8\pi)=K_{\rm eff}\rho^2$. Dividing equilibrium by $\rho$, differentiating, and using the cylindrical [Poisson equation](../../../partial-differential-equation.md#poisson-equation)

$$
\frac1R\frac d{dR}\left(R\frac{d\Phi}{dR}\right)=4\pi G\rho
$$

gives

$$
\boxed{
\frac1R\frac d{dR}\left(R\frac{d\rho}{dR}\right)
+\frac{2\pi G}{K_{\rm eff}}\rho=0}.
$$

Put $a^2=K_{\rm eff}/(2\pi G)$. This is the order-zero [Bessel differential equation](../../../analysis.md#bessel-differential-equation), and regularity on the axis together with $\rho(0)=\rho_1$ yields

$$
\boxed{\rho(R)=\rho_1J_0(R/a)}.
$$

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

The physical filament ends when the [mass density](../../../fluid-mechanics.md#density) first reaches zero. If $x_1\simeq2.4$ is the first positive zero of the [Bessel function](../../../analysis.md#bessel-function) $J_0$, then

$$
\boxed{
R_f=x_1a
=x_1\sqrt{\frac{K+B_0^2/(8\pi\rho_0^2)}{2\pi G}}}.
$$

The first zero must be used because continuing to the next lobe would make the density negative.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

The [line mass](../../../astrophysical-fluid-dynamics.md#line-mass) is

$$
\lambda=2\pi\int_0^{R_f}\rho(R)R\,dR.
$$

Using $d[xJ_1(x)]/dx=xJ_0(x)$ and $J_1(x)=-J_0'(x)$ gives

$$
\lambda=2\pi\rho_1a^2x_1J_1(x_1)
=-\frac{\rho_1K_{\rm eff}}Gx_1J_0'(x_1).
$$

Since $x_1\simeq2.4$ and $J_0'(x_1)\simeq-0.52$,

$$
\boxed{
\lambda\simeq1.25\frac{\rho_1}{G}
\left(K+\frac{B_0^2}{8\pi\rho_0^2}\right)}.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Write $Y=B_\phi^2$, $x=R^2/L^2$, and retain the frozen axial field $B_z=(B_0/\rho_0)\rho$. The radial [magnetostatic equilibrium](../../../electromagnetism.md#magnetostatic-equilibrium) equation now includes both the gradient of the toroidal [magnetic pressure](../../../astrophysical-fluid-dynamics.md#magnetic-pressure) and the inward [magnetic tension](../../../astrophysical-fluid-dynamics.md#magnetic-tension):

$$
\frac d{dR}(K_{\rm eff}\rho^2)
+\rho\Phi'
+\frac{Y'}{8\pi}
+\frac{Y}{4\pi R}=0.
$$

For $\rho=\rho_1e^{-x}$, cylindrical gravity gives

$$
\Phi'(R)=\frac{2G\lambda(<R)}R
=\frac{2\pi G\rho_1L^2}{R}(1-e^{-x}).
$$

Multiplication by the [integrating factor](../../../differential-equation.md#integrating-factor) $R^2$ therefore produces

$$
\frac d{dR}(R^2Y)
=-8\pi R^2\left[\rho\Phi'+\frac d{dR}(K_{\rm eff}\rho^2)\right].
$$

The integration constant must vanish for regularity on the axis. Direct integration gives

$$
\boxed{
B_\phi^2(R)=\frac{4\pi\rho_1^2}{R^2}
\left\{
K_{\rm eff}L^2[1-(1+2x)e^{-2x}]
-\pi GL^4(1-e^{-x})^2
\right\}}.
$$

Its [Taylor expansion](../../../calculus.md#taylor-expansion) at the axis is

$$
B_\phi^2
=4\pi\rho_1^2(2K_{\rm eff}-\pi GL^2)\frac{R^2}{L^2}
+O(R^4),
$$

so the regular field behaves as $B_\phi=O(R)$. At large radius,

$$
B_\phi^2\sim
\frac{4\pi\rho_1^2L^2}{R^2}(K_{\rm eff}-\pi GL^2).
$$

Nonnegativity at infinity requires

$$
\boxed{L^2\leq\frac{K_{\rm eff}}{\pi G}}.
$$

This condition is also sufficient: at the limiting value, the braces divided by $K_{\rm eff}L^2$ reduce to $2e^{-x}[1-(1+x)e^{-x}]\geq0$, and decreasing $L^2$ only increases them. Thus the [toroidal magnetic field](../../../astrophysical-fluid-dynamics.md#toroidal-magnetic-field) is real and regular at every radius exactly in the stated range.

## 3

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Steady spherical [mass conservation](../../../continuum-mechanics.md#mass-conservation) gives $4\pi r^2\rho u=\dot M$. For the [polytropic equation of state](../../../astrophysical-fluid-dynamics.md#polytropic-equation-of-state), $c_s^2=dp/d\rho$, so

$$
\frac{\rho'}\rho=-\frac{u'}u-\frac2r,
\qquad
\frac{p'}\rho=c_s^2\frac{\rho'}\rho.
$$

Substitution into the radial [Euler equations for an inviscid fluid](../../../fluid-mechanics.md#euler-equations-for-an-inviscid-fluid) gives the [Parker wind equation](../../../astrophysical-fluid-dynamics.md#parker-wind-equation)

$$
\boxed{
\left(u-\frac{c_s^2}{u}\right)\frac{du}{dr}
=\frac{2c_s^2}{r}-\frac{GM_*}{r^2}}.
$$

At a [sonic point](../../../compressible-flow.md#sonic-point), the coefficient of $du/dr$ vanishes. A smooth [transonic branch](../../../compressible-flow.md#transonic-branch) can pass it only if the right-hand side vanishes simultaneously. Hence

$$
\boxed{u_s=c_{s,s},
\qquad
r_s=\frac{GM_*}{2c_{s,s}^2}}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The steady [Bernoulli equation](../../../fluid-mechanics.md#bernoulli-equation) is

$$
\frac{u^2}{2}+\frac{c_s^2}{\gamma-1}-\frac{GM_*}{r}=E.
$$

At the regular [sonic point](../../../compressible-flow.md#sonic-point), part a gives

$$
E=c_{s,s}^2\left(\frac1{\gamma-1}-\frac32\right).
$$

Define

$$
\nu=\frac1{\gamma-1}-\frac32
=\frac{5-3\gamma}{2(\gamma-1)},
\qquad
x=\frac{c_{s,s}^2}{c_{s,0}^2}.
$$

The [isentropic flow](../../../compressible-flow.md#isentropic-flow) relation $c_s^2\propto\rho^{\gamma-1}$ and mass conservation between the stellar surface and the sonic point give

$$
\mathcal M_0=\frac{x^\nu}{4\alpha^2},
\qquad
x=(4\alpha^2\mathcal M_0)^{1/\nu}.
$$

Equating the surface and sonic values of the [Bernoulli function](../../../fluid-mechanics.md#bernoulli-function) therefore yields the required relation

$$
\boxed{
\frac{\mathcal M_0^2}{2}
+\frac1{\gamma-1}-\frac1\alpha
=\nu(4\alpha^2\mathcal M_0)^{1/\nu}}.
$$

An outflow reaching infinity with positive terminal kinetic energy requires $E>0$, hence

$$
\boxed{1<\gamma<\frac53}.
$$

At $\gamma=5/3$ the terminal state is marginal with $E=0$; larger $\gamma$ cannot support the stipulated wind to infinity.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

At $\alpha=1/2$, setting $\mathcal M_0=1$ gives $x=1$ in the mass relation, and both sides of the boxed relation in part b equal $\nu$. Moreover,

$$
\frac{r_s}{R_*}=\frac1{2\alpha x}=1,
$$

so the stellar surface itself is the [sonic point](../../../compressible-flow.md#sonic-point). This conclusion is independent of $\gamma$ throughout $1<\gamma<5/3$.

There is no other value of $\alpha$ giving a smooth solution with $\mathcal M_0=1$. Indeed, eliminating $\alpha$ in favour of $x$ reduces the Bernoulli relation to

$$
\nu x+2x^{-\nu/2}=\nu+2.
$$

The left side has its unique minimum at $x=1$, where it equals the right side. Thus $x=1$ and $\alpha=1/2$ are forced.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For fixed $0<\mathcal M_0<1$, eliminate $\alpha$ by

$$
\alpha=\frac{x^{\nu/2}}{2\sqrt{\mathcal M_0}}.
$$

The remaining equation is

$$
\nu x+2\sqrt{\mathcal M_0}\,x^{-\nu/2}
=\nu+\frac32+\frac{\mathcal M_0^2}{2}.
$$

Its left side diverges at both ends and has one minimum, at

$$
x=\mathcal M_0^{1/(\nu+2)}.
$$

For $0<\mathcal M_0<1$ this minimum lies strictly below the right side, so there are exactly two positive values of $x$, and hence exactly two values of $\alpha$. The branches merge at the marginal point $(\alpha,\mathcal M_0)=(1/2,1)$.

On the very hot branch, $\alpha\to\infty$ and $\mathcal M_0=O(\alpha^{-2})$. Dropping $1/\alpha$ and $\mathcal M_0^2$ in the relation from part b gives

$$
\boxed{
\mathcal M_0\sim\frac1{4\alpha^2}
\left(\frac{2}{5-3\gamma}\right)^\nu},
\qquad
\nu=\frac{5-3\gamma}{2(\gamma-1)}.
$$

## 4

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The shock speed is

$$
V_s=\dot R=\frac{C}{3}t^{-2/3}=\frac{R}{3t}.
$$

Apply the [Strong-shock Rankine-Hugoniot conditions](../../../compressible-flow.md#strong-shock-rankine-hugoniot-conditions) in the shock frame and transform the downstream velocity back to the ambient-medium frame. With the [shock compression ratio](../../../compressible-flow.md#shock-compression-ratio)

$$
\chi=\frac{\gamma+1}{\gamma-1},
$$

the post-shock values are

$$
\boxed{
\rho_{\rm ps}=\chi\rho_0,
\qquad
u_{\rm ps}=\frac{2}{\gamma+1}V_s,
\qquad
p_{\rm ps}=\frac{2}{\gamma+1}\rho_0V_s^2}.
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For $\gamma=5/3$, the shock data give $\rho_{\rm ps}=4\rho_0$ and $u_{\rm ps}=3V_s/4$. Since $V_s=R/(3t)$, the prescribed [homologous spherical flow](../../../fluid-mechanics.md#homologous-spherical-flow) is

$$
u(r,t)=\frac{r}{4t}.
$$

Put $\xi=r/R(t)$ and $\rho=\rho_0D(\xi)$. The spherical [continuity equation](../../../physics.md#continuity-equation) becomes

$$
-\frac{\xi}{3}D'+\frac14(3D+\xi D')=0,
$$

so $D\propto\xi^9$. Matching the post-shock density gives

$$
\rho(r,t)=4\rho_0\xi^9.
$$

The [material acceleration](../../../continuum-mechanics.md#material-acceleration) is

$$
\frac{Du}{Dt}=-\frac{3r}{16t^2}.
$$

The radial [Euler equations for an inviscid fluid](../../../fluid-mechanics.md#euler-equations-for-an-inviscid-fluid) thus give $dp/dr=3\rho r/(16t^2)$. Integrating from the centre to the shock,

$$
p_{\rm ps}-p(0,t)
=\frac{3}{16t^2}\int_0^R\rho r\,dr
=\frac{3\rho_0R^2}{44t^2}.
$$

Since $p_{\rm ps}=\rho_0R^2/(12t^2)$,

$$
\boxed{p(0,t)=\frac{\rho_0R^2}{66t^2}
=\frac{2}{11}p_{\rm ps}}.
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Resolve the uniform upstream field into components normal and tangential to the spherical shock:

$$
B_{0r}=B_0\cos\theta,
\qquad
B_{0\theta}=-B_0\sin\theta,
\qquad
B_{0\phi}=0.
$$

The [ideal magnetohydrodynamic shock conditions](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-shock-conditions) leave the normal field continuous and multiply the tangential field by the gas compression ratio $\chi$. Therefore

$$
\boxed{
\mathbf B_{\rm ps}
=B_0\cos\theta\,\mathbf e_r
-\chi B_0\sin\theta\,\mathbf e_\theta,
\qquad
\chi=\frac{\gamma+1}{\gamma-1}}.
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The post-shock density is $\chi\rho_0$, while part c gives

$$
|\mathbf B_{\rm ps}|^2
=B_0^2(\cos^2\theta+\chi^2\sin^2\theta).
$$

Using the [Alfvén speed](../../../astrophysical-fluid-dynamics.md#alfven-speed) $v_A=B/\sqrt{4\pi\rho}$ in Gaussian units,

$$
\boxed{
\frac{v_{A,\rm ps}}{v_{A,0}}
=\left(\frac{\cos^2\theta+\chi^2\sin^2\theta}{\chi}\right)^{1/2}}.
$$

The ratio is largest in the equatorial plane, where the field is tangential to the shock:

$$
\boxed{
\left(\frac{v_{A,\rm ps}}{v_{A,0}}\right)_{\max}
=\sqrt\chi
=\sqrt{\frac{\gamma+1}{\gamma-1}}}.
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
