# Paper 314

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_314.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_314.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
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

## 1

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

In a static spherical star, [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium) and the [Poisson equation](../../../partial-differential-equation.md#poisson-equation) give

$$
\boxed{\frac{dp}{dr}=-\rho g,
\qquad
g=\frac{d\Phi}{dr}=\frac{Gm(r)}{r^2},
\qquad
\frac{dm}{dr}=4\pi r^2\rho},
$$

or equivalently $r^{-2}d(r^2g)/dr=4\pi G\rho$.

Let $\boldsymbol\xi$ be the fluid [displacement field](../../../continuum-mechanics.md#displacement-field-mechanics), so the velocity perturbation is $\delta\mathbf u=\partial_t\boldsymbol\xi$. Linearizing the ideal-fluid momentum equation about the static state and cancelling the background hydrostatic terms gives

$$
\boxed{\rho\frac{\partial^2\boldsymbol\xi}{\partial t^2}
=-\rho\nabla\delta\Phi-\delta\rho\nabla\Phi-\nabla\delta p}.
$$

Conservation of mass says that the Lagrangian density perturbation is $\Delta_L\rho=-\rho\nabla\cdot\boldsymbol\xi$. The relation between [Eulerian and Lagrangian fluid perturbations](../../../fluid-mechanics.md#eulerian-and-lagrangian-fluid-perturbations) and adiabatic compression gives, with $\Delta=\nabla\cdot\boldsymbol\xi$,

$$
\boxed{\delta\rho=-\rho\Delta-\boldsymbol\xi\cdot\nabla\rho,
\qquad
\delta p=-\gamma p\Delta-\boldsymbol\xi\cdot\nabla p},
$$

while linearized self-gravity gives $\boxed{\nabla^2\delta\Phi=4\pi G\delta\rho}$.

For the stated [spherical harmonic](../../../analysis.md#spherical-harmonic) displacement, the radial divergence is $r^{-2}d(r^2\widetilde\xi_r)/dr$, while $\nabla\widetilde\xi_h$ is radial and orthogonal to the angular gradient of $Y_l^m$. Hence

$$
\boxed{\widetilde\Delta
=\frac1{r^2}\frac d{dr}(r^2\widetilde\xi_r)
-k_h^2\widetilde\xi_h,
\qquad
k_h^2=\frac{l(l+1)}{r^2}}.
$$

Equating the radial and horizontal coefficients of $Y_l^m$ and $\nabla Y_l^m$, and applying the separated [Laplacian in spherical coordinates](../../../partial-differential-equation.md#laplacian-in-spherical-coordinates) to $\widetilde{\delta\Phi}(r)Y_l^m$, gives

$$
\boxed{-\rho\omega^2\widetilde\xi_r
=-\rho\frac{d\widetilde{\delta\Phi}}{dr}
-g\widetilde{\delta\rho}
-\frac{d\widetilde{\delta p}}{dr}},
$$



$$
\boxed{-\rho\omega^2\widetilde\xi_h
=-\rho\widetilde{\delta\Phi}-\widetilde{\delta p}},
$$



$$
\boxed{\widetilde{\delta\rho}
=-\rho\widetilde\Delta-\widetilde\xi_r\frac{d\rho}{dr},
\qquad
\widetilde{\delta p}
=-\gamma p\widetilde\Delta-\widetilde\xi_r\frac{dp}{dr}},
$$



$$
\boxed{\frac1{r^2}\frac d{dr}
\left(r^2\frac{d\widetilde{\delta\Phi}}{dr}\right)
-k_h^2\widetilde{\delta\Phi}=4\pi G\widetilde{\delta\rho}}.
$$

Define the [stellar buoyancy frequency](../../../gravity-wave.md#stellar-buoyancy-frequency) by

$$
\boxed{N^2=g\left(
\frac1{\gamma p}\frac{dp}{dr}
-\frac1\rho\frac{d\rho}{dr}\right)}.
$$

Eliminating $\widetilde\Delta$ between the density and pressure perturbations gives

$$
\widetilde{\delta\rho}
=\frac{\rho}{\gamma p}\widetilde{\delta p}
+\frac{\rho N^2}{g}\widetilde\xi_r.
$$

Substitution in the radial equation, followed by use of $dp/dr=-\rho g$, yields

$$
\boxed{(\omega^2-N^2)\widetilde\xi_r
=\frac d{dr}\left(
\widetilde{\delta\Phi}+\frac{\widetilde{\delta p}}\rho\right)
-\frac{N^2\widetilde{\delta p}}{g\rho}}.
$$

Regular spherical profiles near the center have $\rho=\rho_c+O(r^2)$ and $p=p_c+O(r^2)$, while $m(r)=4\pi\rho_cr^3/3+O(r^5)$ and hence $g=O(r)$. Both logarithmic gradients in the definition of $N^2$ are $O(r)$, so $N^2=Ar^2+O(r^4)$. A Sun-like radiative central stratification is stable, making $A>0$.

## 2

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For one-dimensional [compressible flow](../../../compressible-flow.md), define the total energy density

$$
E=\frac{p}{\gamma-1}+\frac12\rho u_x^2.
$$

The conservative mass, momentum, and energy equations are

$$
\boxed{\partial_t\rho+\partial_x(\rho u_x)=0},
$$



$$
\boxed{\partial_t(\rho u_x)+\partial_x(\rho u_x^2+p)=0},
$$



$$
\boxed{\partial_tE+\partial_x[(E+p)u_x]=0}.
$$

A monatomic nonrelativistic perfect gas has $\gamma=5/3$, an ultrarelativistic gas or radiation-dominated fluid has $\gamma=4/3$, and a rotationally active diatomic gas has $\gamma=7/5$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Integrating the three conservation laws across a stationary [normal shock wave](../../../compressible-flow.md#normal-shock-wave) gives the [Rankine-Hugoniot conditions for a perfect gas](../../../compressible-flow.md#rankine-hugoniot-conditions-for-a-perfect-gas)

$$
\rho_1u_{x1}=\rho_2u_{x2},
$$



$$
p_1+\rho_1u_{x1}^2=p_2+\rho_2u_{x2}^2,
$$



$$
\frac{\gamma p_1}{(\gamma-1)\rho_1}+\frac12u_{x1}^2
=\frac{\gamma p_2}{(\gamma-1)\rho_2}+\frac12u_{x2}^2.
$$

Eliminate $u_{x2}$ with the conserved mass flux and write $v_s^2=\gamma p/\rho$ and $M_x=u_x/v_s$. Solving the remaining two algebraic equations gives

$$
\boxed{\frac{u_{x1}}{u_{x2}}=\frac{\rho_2}{\rho_1}
=\frac{(\gamma+1)M_{x1}^2}
{(\gamma-1)M_{x1}^2+2}},
$$



$$
\boxed{\frac{p_2}{p_1}
=\frac{2\gamma M_{x1}^2-(\gamma-1)}{\gamma+1}}.
$$

For a compressive shock, $M_{x1}>1$, the density and pressure increase, and the downstream normal flow is subsonic in the shock frame.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For an [oblique shock](../../../compressible-flow.md#oblique-shock), boost parallel to the front by the upstream tangential speed. The transformed upstream flow is normal, so part b applies. Inviscid momentum balance has no tangential stress and therefore makes the tangential velocity continuous. Transforming back gives

$$
\boxed{u_{y1}=u_{y2}},
$$

while all normal velocity, density, and pressure relations from part b remain unchanged with $M_x$ the normal Mach number.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The pressure jump relation with $p_2/p_1=1+\epsilon$ gives

$$
M_{x1}^2=1+\frac{\gamma+1}{2\gamma}\epsilon.
$$

If $\beta_1$ is the angle between the upstream velocity and the shock front, then $M_{x1}=M_1\sin\beta_1$. To leading order,

$$
\boxed{\beta_1\simeq\beta_2\simeq
\arcsin(M_1^{-1})},
$$

the [Mach angle](../../../compressible-flow.md#mach-angle). Expansion of the compression ratio gives

$$
\frac{\rho_2}{\rho_1}=1+\frac\epsilon\gamma+O(\epsilon^2).
$$

Because $u_y$ is continuous and $\tan\beta=u_x/u_y$,

$$
\boxed{\frac{\tan\beta_1}{\tan\beta_2}
=\frac{u_{x1}}{u_{x2}}
=1+\frac\epsilon\gamma+O(\epsilon^2)}.
$$

Writing $\theta=\beta_1-\beta_2$ and linearizing the tangent about $\sin\beta_1=1/M_1$ gives the [weak-oblique-shock deflection](../../../compressible-flow.md#weak-oblique-shock-deflection)

$$
\boxed{\theta\simeq
\frac\epsilon\gamma\sin\beta_1\cos\beta_1
=\frac{\epsilon\sqrt{M_1^2-1}}{\gamma M_1^2}}.
$$

The normal component decreases while the tangential component is unchanged, so $\beta_2<\beta_1$: the flow turns toward the shock front.

## 3

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Since $\nabla\phi=\mathbf e_\phi/r$, the vector field has cylindrical components

$$
\mathbf A=-\frac{\alpha_z}{r}\mathbf e_r
+\frac\beta r\mathbf e_\phi
+\frac{\alpha_r}{r}\mathbf e_z.
$$

The [divergence](../../../calculus.md#divergence) in cylindrical coordinates is therefore

$$
\nabla\cdot\mathbf A
=-\frac1r\partial_r\alpha_z
+\frac1r\partial_z\alpha_r=0.
$$

Direct use of the [curl](../../../calculus.md#curl) in cylindrical coordinates gives

$$
(\nabla\times\mathbf A)_r=-\frac{\beta_z}{r},
\qquad
(\nabla\times\mathbf A)_z=\frac{\beta_r}{r},
$$

and

$$
(\nabla\times\mathbf A)_\phi
=\frac1r\left[-r\partial_r(r^{-1}\alpha_r)-\alpha_{zz}\right].
$$

Thus, defining

$$
\boxed{L\alpha=-r\partial_r(r^{-1}\partial_r\alpha)-\partial_z^2\alpha},
$$

we obtain

$$
\boxed{\nabla\times\mathbf A
=\nabla\beta\times\nabla\phi+(L\alpha)\nabla\phi}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For the stated [magnetic vector potential](../../../electromagnetism.md#magnetic-vector-potential), part a gives

$$
\boxed{\mathbf B=\nabla\beta\times\nabla\phi
+(L\alpha)\nabla\phi}.
$$

Applying the same identity once more and using the [Ampère-Maxwell equation](../../../electromagnetism.md#ampere-s-circuital-law) in the magnetostatic limit gives

$$
\boxed{\mathbf J=\frac1{\mu_0}
\left[\nabla(L\alpha)\times\nabla\phi
+(L\beta)\nabla\phi\right]}.
$$

Expanding the [Lorentz force density](../../../electromagnetism.md#lorentz-force-density) $\mathbf F_m=\mathbf J\times\mathbf B$, using $\nabla\phi=\mathbf e_\phi/r$ and the vector triple-product identity, separates its poloidal and azimuthal parts:

$$
\boxed{r^2\mu_0\mathbf F_m
=(L\beta)\nabla\beta-(L\alpha)\nabla(L\alpha)
+f\mathbf e_\phi},
$$

where

$$
\boxed{f=[\nabla(L\alpha)\times\nabla\beta]\cdot\mathbf e_\phi}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

In an axisymmetric magnetostatic state, pressure and gravitational forces are poloidal, so the azimuthal component of the [Lorentz force density](../../../electromagnetism.md#lorentz-force-density) must vanish. Hence $f=0$ and

$$
\nabla(L\alpha)\times\nabla\beta=0.
$$

The two gradients are locally parallel, so $L\alpha$ is constant on each regular level surface of $\beta$. Therefore

$$
\boxed{L\alpha=F(\beta)}
$$

for an arbitrary flux function $F$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For a [barotropic fluid](../../../fluid-mechanics.md#barotropic-fluid), $\nabla p=\rho\nabla h$. Magnetostatic force balance and $L\alpha=F(\beta)$ give

$$
\rho\nabla(\Phi+h)=\mathbf F_m
=\frac{L\beta-FF'}{\mu_0r^2}\nabla\beta.
$$

The left side is a gradient multiplied by $\rho$, so taking the curl shows that $(L\beta-FF')/(r^2\rho)$ is constant on each $\beta$ surface. Absorbing the fixed factor $\mu_0$ into an arbitrary function $G$ gives the [Axisymmetric magnetostatic Grad-Shafranov system](../../../astrophysical-fluid-dynamics.md#axisymmetric-magnetostatic-grad-shafranov-system)

$$
\boxed{L\beta=F(\beta)\frac{dF}{d\beta}+r^2\rho G(\beta)}.
$$

## 4

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The divergence-free poloidal field can be represented by the [poloidal magnetic flux function](../../../astrophysical-fluid-dynamics.md#poloidal-magnetic-flux-function)

$$
\mathbf B_p=\nabla\psi\times\nabla\phi
=-\frac1r\mathbf e_\phi\times\nabla\psi.
$$

In a steady axisymmetric [ideal magnetohydrodynamics](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamics) flow, the azimuthal component of $\nabla\times(\mathbf u\times\mathbf B)=0$ makes $\mathbf u_p$ parallel to $\mathbf B_p$. Write

$$
\boxed{\rho\mathbf u_p=k\mathbf B_p}.
$$

Mass conservation and $\nabla\cdot\mathbf B=0$ then imply $\mathbf B\cdot\nabla k=0$, so the [magnetohydrodynamic mass loading](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-mass-loading) $k=k(\psi)$ is constant along each magnetic line.

The poloidal part of $\mathbf u\times\mathbf B$ is

$$
\mathbf u\times\mathbf B
=\frac1r\left(u_\phi-\frac{kB_\phi}{\rho}\right)\nabla\psi.
$$

Its curl vanishes only if its coefficient is a flux function, giving the [field-line angular velocity](../../../astrophysical-fluid-dynamics.md#field-line-angular-velocity)

$$
\boxed{\frac{u_\phi}{r}-\frac{kB_\phi}{r\rho}=\omega(\psi)}.
$$

The azimuthal component of momentum conservation is a divergence of matter and magnetic angular-momentum flux. Dividing its field-line constant by the mass loading yields the [magnetohydrodynamic angular-momentum invariant](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-angular-momentum-invariant)

$$
\boxed{ru_\phi-\frac{rB_\phi}{\mu_0k}=\ell(\psi)}.
$$

The conservative total-energy equation similarly gives the [magnetohydrodynamic Bernoulli invariant](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-bernoulli-invariant)

$$
\boxed{\frac12|\mathbf u|^2+\Phi+h
-\frac{r\omega B_\phi}{\mu_0k}=\epsilon(\psi)}.
$$

Finally, the [entropy advection equation](../../../astrophysical-fluid-dynamics.md#entropy-advection-equation) and $\mathbf u_p\parallel\mathbf B_p$ imply $s=s(\psi)$. Thus $k,\omega,\ell,\epsilon$, and $s$ are constant along each magnetic field line.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Introduce the squared poloidal [Alfvén number](../../../astrophysical-fluid-dynamics.md#alfven-number)

$$
M_A^2=\frac{\mu_0\rho u_p^2}{B_p^2}
=\frac{\mu_0k^2}{\rho}.
$$

Solving the two linear azimuthal invariants gives

$$
\boxed{u_\phi=
\frac{M_A^2\ell/r-r\omega}{M_A^2-1}},
$$



$$
\boxed{B_\phi=
\frac{\mu_0k(\ell/r-r\omega)}{M_A^2-1}}.
$$

At an [Alfvén surface](../../../astrophysical-fluid-dynamics.md#alfven-surface), $M_A^2=1$. Smooth passage through the apparent singularity requires both numerators to vanish at the same cylindrical radius $r_A$, giving the [Alfvén-surface regularity condition for an axisymmetric wind](../../../astrophysical-fluid-dynamics.md#alfven-surface-regularity-condition-for-an-axisymmetric-wind)

$$
\boxed{\ell=\omega r_A^2}.
$$

The finite limiting values of $u_\phi$ and $B_\phi$ then follow by l'Hopital's rule from the local variation of $M_A$ and $r$ along the field line; the algebraic invariants alone fix their combination rather than each value separately at the critical point.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Along the open line, $B_p\sim F/r^2$ and the mass-loading relation with $u_p\to u_\infty$ gives

$$
\rho\sim\frac{kF}{u_\infty r^2},
\qquad
M_A^2\sim\frac{\mu_0ku_\infty}{F}r^2\longrightarrow\infty.
$$

The solutions of part b consequently have

$$
u_\phi\sim\frac\ell r,
\qquad
B_\phi\sim-\frac{\omega F}{u_\infty r}.
$$

The azimuthal [Alfvén speed](../../../astrophysical-fluid-dynamics.md#alfven-speed) therefore approaches the nonzero constant

$$
\boxed{|v_{A\phi}|=\frac{|B_\phi|}{\sqrt{\mu_0\rho}}
\longrightarrow|\omega|\sqrt{\frac{F}{\mu_0ku_\infty}}}.
$$

For an unconfined outflow it is natural to take $\Phi\to0$ and $h\to0$ at infinity; also $u_\phi\to0$. The magnetic term in the [magnetohydrodynamic Bernoulli invariant](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-bernoulli-invariant) tends to

$$
-\frac{r\omega B_\phi}{\mu_0k}
\longrightarrow\frac{\omega^2F}{\mu_0ku_\infty}.
$$

Hence the [asymptotic energy of a radial magnetohydrodynamic wind](../../../astrophysical-fluid-dynamics.md#asymptotic-energy-of-a-radial-magnetohydrodynamic-wind) is

$$
\boxed{\epsilon=\frac12u_\infty^2
+\frac{\omega^2F}{\mu_0ku_\infty}}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
