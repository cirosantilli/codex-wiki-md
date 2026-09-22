# Paper 321

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_321.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_321.pdf)

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

## 1

↑ **Parent:** [Paper 321](paper-321.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Put $r_S=2R_g$. On the midplane, [circular orbit](../../../classical-mechanics.md#circular-orbit) balance gives $r\Omega^2=\partial_r\Phi=GM/(r-r_S)^2$. The [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum), [specific orbital energy](../../../classical-mechanics.md#specific-orbital-energy) and [orbital shear parameter](../../../gravitational-instability-of-an-astrophysical-disk.md#orbital-shear-parameter) of a [Paczyński-Wiita circular orbit](../../../astrophysics.md#paczynski-wiita-circular-orbit) are therefore

$$
\boxed{\Omega^2=\frac{GM}{r(r-2R_g)^2}},\qquad
\boxed{h=r^2\Omega=\frac{\sqrt{GM}\,r^{3/2}}{r-2R_g}},
$$



$$
\boxed{\varepsilon=\frac12r^2\Omega^2+\Phi(r,0)
=\frac{GM(4R_g-r)}{2(r-2R_g)^2}},\qquad
\boxed{q=-\frac{d\log\Omega}{d\log r}
=\frac12+\frac r{r-2R_g}}.
$$

For a small radial displacement at fixed [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum), the [effective potential stability criterion](../../../physics.md#effective-potential-stability-criterion) gives the [radial epicyclic frequency](../../../astrophysics.md#radial-epicyclic-frequency)

$$
\boxed{\kappa_r^2=\frac1{r^3}\frac{d(h^2)}{dr}
=\frac{GM(r-6R_g)}{r(r-2R_g)^3}
=2(2-q)\Omega^2}.
$$

Here $\kappa_r$ is the question's epicyclic $\kappa$. Its square is negative for $2R_g<r<6R_g$, so a radial displacement grows instead of undergoing [epicyclic motion](../../../astrophysics.md#epicyclic-motion). The orbit at $r_{\rm in}=6R_g$ is marginal, and the outer orbits are stable to small radial displacements. At this inner edge,

$$
\boxed{\varepsilon(6R_g)=-\frac{GM}{16R_g}=-\frac{c^2}{16}},\qquad
\boxed{\eta=\frac1{16}}.
$$

This efficiency belongs to the [Paczyński-Wiita potential](../../../astrophysics.md#paczynski-wiita-potential); it is an approximation to the relativistic black-hole result.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

In a [steady state](../../../dynamical-systems.md#steady-state), [mass conservation](../../../continuum-mechanics.md#mass-conservation) makes $\mathcal F$ independent of radius. Taking the [accretion rate](../../../astrophysics.md#accretion-rate) $\dot M>0$ for inward flow gives $\mathcal F=-\dot M$. The [conservation of angular momentum](../../../classical-mechanics.md#conservation-of-angular-momentum) equation then makes $-\dot M h+\mathcal G$ constant. The [zero-torque inner boundary condition](../../../astrophysics.md#zero-torque-inner-boundary-condition) fixes this constant to $-\dot M h_{\rm in}$, so

$$
\mathcal G=\dot M(h-h_{\rm in}).
$$

The [viscous torque in an accretion disk](../../../astrophysics.md#viscous-torque-in-an-accretion-disk) is $\mathcal G=-2\pi r^3\bar\nu\Sigma\Omega'=2\pi qh\bar\nu\Sigma$. Combining these expressions gives the [steady accretion disk with arbitrary rotation law](../../../astrophysics.md#steady-accretion-disk-with-arbitrary-rotation-law)

$$
\bar\nu\Sigma=\frac{\dot M}{2\pi q}
\left(1-\frac{h_{\rm in}}h\right).
$$

For $x=r/R_g$, the [Paczyński-Wiita circular orbit](../../../astrophysics.md#paczynski-wiita-circular-orbit) formulas give

$$
\frac3{2q}=\frac{x-2}{x-2/3},\qquad
\frac{h_{\rm in}}h=\frac{3\sqrt3(x-2)}{\sqrt2\,x^{3/2}}.
$$

Consequently

$$
\boxed{\bar\nu\Sigma=\frac{f\dot M}{3\pi}},\qquad
\boxed{f=\frac{x-2}{x-2/3}
\left[1-\frac{3\sqrt3(x-2)}{\sqrt2\,x\sqrt x}\right]}.
$$

In particular, $f(6)=0$ and $f\to1$ far from the black hole, recovering the outer [Keplerian accretion disk](../../../astrophysics.md#keplerian-accretion-disk).

Inside the [innermost stable circular orbit](../../../astrophysics.md#innermost-stable-circular-orbit), the gas enters the [plunging region of a black-hole accretion disk](../../../astrophysics.md#plunging-region-of-a-black-hole-accretion-disk). Its rapid inward motion leaves little time for stresses to exchange [angular momentum](../../../classical-mechanics.md#angular-momentum), motivating the [zero-torque inner boundary condition](../../../astrophysics.md#zero-torque-inner-boundary-condition). This is a thin-disc approximation; a strong magnetic stress could change it.

Matter supplied from very large radius has negligible [specific orbital energy](../../../classical-mechanics.md#specific-orbital-energy), while matter crossing the inner edge carries $\varepsilon_{\rm in}=-\eta c^2$. With zero inner torque, no energy is supplied by a stress at that edge. If the heat released outside it escapes by [radiative transfer](../../../astrophysics.md#radiative-transfer), rather than being lost through inward [advection](../../../fluid-mechanics.md#advection), the integrated [conservation of energy](../../../physics.md#conservation-of-energy) balance gives

$$
\boxed{L_{\rm disc}=-\dot M\varepsilon_{\rm in}=\eta\dot M c^2=\frac{\dot M c^2}{16}}.
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Here $\beta=p_{\rm rad}/p_{\rm gas}$ is the [radiation-to-gas pressure ratio](../../../astrophysics.md#radiation-to-gas-pressure-ratio), not [plasma beta](../../../astrophysics.md#plasma-beta). Write the [opacity](../../../stellar-structure.md#opacity) as $\kappa_{\rm op}$ to distinguish it from the [radial epicyclic frequency](../../../astrophysics.md#radial-epicyclic-frequency). The [radiation pressure](../../../thermodynamics.md#radiation-pressure) is $p_{\rm rad}=4\sigma T^4/(3c)$, so [radiative diffusion](../../../astrophysics.md#radiative-diffusion) can be written as

$$
F_z=-\frac{c}{\kappa_{\rm op}\rho}\frac{dp_{\rm rad}}{dz}.
$$

Since $\beta$ is independent of height, $p_{\rm rad}=\beta p/(1+\beta)$. Substitution of [hydrostatic equilibrium](../../../statistical-physics.md#hydrostatic-equilibrium), $p'=-\rho\Omega^2z$, gives

$$
F_z=\frac\beta{1+\beta}\frac{c\Omega^2}{\kappa_{\rm op}}z.
$$

Differentiating and using the viscous heating equation, together with $r\Omega'=-q\Omega$, yields

$$
\rho\nu q^2\Omega^2=\frac\beta{1+\beta}\frac{c\Omega^2}{\kappa_{\rm op}},\qquad
\boxed{\rho\nu=\frac\beta{1+\beta}\frac{c}{q^2\kappa_{\rm op}}}.
$$

Thus the effective [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity) $\rho\nu$ is independent of height. If the surfaces are at $z=\pm H$, the vertically integrated [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity) satisfies

$$
\bar\nu\Sigma=\int_{-H}^H\rho\nu\,dz
=2H\frac\beta{1+\beta}\frac{c}{q^2\kappa_{\rm op}}.
$$

Use the previous result and the specified [Eddington accretion rate](../../../astrophysics.md#eddington-accretion-rate) convention,

$$
\dot M_E=\frac{L_E}{\eta c^2}
=\frac{4\pi GM}{\eta\kappa_{\rm op}c},\qquad \eta=\frac1{16},
$$

to obtain the full thickness

$$
\boxed{2H=\frac{64}{3}\frac{1+\beta}{\beta}\,q^2f\,
\frac{\dot M}{\dot M_E}\frac{GM}{c^2}}.
$$

The [constant-pressure-ratio vertical disk model](../../../astrophysics.md#constant-pressure-ratio-vertical-disk-model) therefore has thickness proportional to the inward [accretion rate](../../../astrophysics.md#accretion-rate). This is a full surface-to-surface thickness, rather than a density [disk scale height](../../../astrophysics.md#disk-scale-height). Its use as a [thin disk](../../../astrophysics.md#thin-disk) requires $2H\ll r$.

## 2

↑ **Parent:** [Paper 321](paper-321.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For unit mass, the [Lagrangian](../../../calculus-of-variations.md#lagrangian) in [cylindrical coordinates](../../../calculus.md#cylindrical-coordinate-system) is

$$
L=\frac12\left(\dot r^2+r^2\dot\varphi^2+\dot z^2\right)-\Phi(r,z).
$$

Introduce [shearing sheet](../../../gravitational-instability-of-an-astrophysical-disk.md#shearing-sheet) coordinates by $r=r_0+x$ and $\varphi=\Omega_0t+y/r_0$. Evaluate all derivatives of $\Phi$ at $(r_0,0)$. The reference [circular orbit](../../../classical-mechanics.md#circular-orbit) obeys $\Phi_r=r_0\Omega_0^2$, while midplane symmetry gives $\Phi_z=\Phi_{rz}=0$. Its [Taylor expansion](../../../calculus.md#taylor-expansion) is

$$
\Phi=\Phi_0+\Phi_rx+\frac12\Phi_{rr}x^2+\frac12\Phi_{zz}z^2+O(3).
$$

Expanding the kinetic energy to the same order gives

$$
\frac12r^2\dot\varphi^2
=\frac12r_0^2\Omega_0^2+r_0\Omega_0^2x+r_0\Omega_0\dot y
+\frac12\Omega_0^2x^2+2\Omega_0x\dot y+\frac12\dot y^2+O(3).
$$

The terms linear in $x$ cancel by circular-orbit balance. Discard the constant and the term $r_0\Omega_0\dot y$ by [total-time-derivative invariance of a Lagrangian](../../../classical-mechanics.md#total-time-derivative-invariance-of-a-lagrangian); these do not change the [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation). The [particle Lagrangian in a shearing sheet](../../../gravitational-instability-of-an-astrophysical-disk.md#particle-lagrangian-in-a-shearing-sheet) is therefore

$$
\boxed{L_2=\frac12(\dot x^2+\dot y^2+\dot z^2)+2\Omega_0x\dot y-\Phi_t},
$$

with [shearing-sheet tidal potential](../../../gravitational-instability-of-an-astrophysical-disk.md#shearing-sheet-tidal-potential)

$$
\boxed{\Phi_t=\frac12(\Phi_{rr}-\Omega_0^2)x^2+\frac12\Phi_{zz}z^2
=-q_0\Omega_0^2x^2+\frac12\Omega_z^2z^2}.
$$

The second form follows from $\Phi_r=r\Omega^2$, the [orbital shear parameter](../../../gravitational-instability-of-an-astrophysical-disk.md#orbital-shear-parameter) $q_0=-d\log\Omega/d\log r$ and the [vertical epicyclic frequency](../../../astrophysics.md#vertical-epicyclic-frequency) $\Omega_z^2=\Phi_{zz}$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The [Euler-Lagrange equations](../../../analysis.md#euler-lagrange-equation) of the [particle Lagrangian in a shearing sheet](../../../gravitational-instability-of-an-astrophysical-disk.md#particle-lagrangian-in-a-shearing-sheet) are

$$
\ddot x-2\Omega_0\dot y-2q_0\Omega_0^2x=0,\qquad
\ddot y+2\Omega_0\dot x=0,\qquad
\ddot z+\Omega_z^2z=0.
$$

The terms coupling $x$ and $y$ are the [Coriolis acceleration](../../../physics.md#coriolis-acceleration). The [cyclic coordinate](../../../classical-mechanics.md#cyclic-coordinate) $y$ has conserved [canonical momentum](../../../classical-mechanics.md#canonical-momentum)

$$
p_y=\frac{\partial L_2}{\partial\dot y}=\dot y+2\Omega_0x.
$$

For a [Newtonian potential of a point mass](../../../classical-mechanics.md#newtonian-potential-of-a-point-mass), $q_0=3/2$ and $\Omega_z=\kappa_r=\Omega_0$. Set $p_y=\Omega_0x_0/2$ and substitute $\dot y=p_y-2\Omega_0x$ in the radial equation. It becomes $\ddot x+\Omega_0^2(x-x_0)=0$, a [harmonic oscillator equation](../../../classical-mechanics.md#simple-harmonic-motion) about the [epicyclic guiding center](../../../astrophysics.md#epicyclic-guiding-center) $x_0$. Integration gives

$$
\boxed{\begin{aligned}
x&=x_0+\operatorname{Re}(Ae^{-i\Omega_0t}),\\
y&=y_0-\frac32\Omega_0x_0t+\operatorname{Re}(-2iAe^{-i\Omega_0t}),\\
z&=\operatorname{Re}(Be^{-i\Omega_0t}).
\end{aligned}}
$$

The four real constants in $A,y_0,x_0$ and the two in $B$ account for the six initial position and velocity data.

Expanding the inertial [specific angular momentum](../../../classical-mechanics.md#specific-angular-momentum) gives $h=h_0+r_0p_y+O(2)$. Thus $p_y$ measures the angular-momentum offset from the reference [circular orbit](../../../classical-mechanics.md#circular-orbit), and $x_0$ specifies the radius of its associated [epicyclic guiding center](../../../astrophysics.md#epicyclic-guiding-center).

The conserved horizontal energy in the rotating frame is

$$
\varepsilon_h=\frac12(\dot x^2+\dot y^2)-\frac32\Omega_0^2x^2
=\boxed{\frac12\Omega_0^2\left(|A|^2-\frac34x_0^2\right)}.
$$

It is the horizontal part of the local [Jacobi energy in a shearing sheet](../../../gravitational-instability-of-an-astrophysical-disk.md#jacobi-energy-in-a-shearing-sheet), rather than the inertial [specific orbital energy](../../../classical-mechanics.md#specific-orbital-energy). Its positive term is the [epicyclic energy](../../../astrophysics.md#epicyclic-energy); its negative term is the energy of the background shear at guiding-center position $x_0$. Independently, the vertical [harmonic oscillator](../../../classical-mechanics.md#simple-harmonic-motion) has conserved energy

$$
\varepsilon_v=\frac12(\dot z^2+\Omega_0^2z^2)
=\boxed{\frac12\Omega_0^2|B|^2}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Initially every particle has $A=B=0$, so its [Jacobi energy in a shearing sheet](../../../gravitational-instability-of-an-astrophysical-disk.md#jacobi-energy-in-a-shearing-sheet) is $-3\Omega_0^2x_0^2/8$. During an [inelastic collision](../../../classical-mechanics.md#inelastic-collision), positions are fixed at the instant of impact, while [momentum conservation](../../../classical-mechanics.md#momentum-conservation) preserves the sum of the tangential velocities. Hence the sum of $p_y=\dot y+2\Omega_0x$, and therefore the sum of the [epicyclic guiding center](../../../astrophysics.md#epicyclic-guiding-center) positions $x_0=2p_y/\Omega_0$, is unchanged. Between collisions, these quantities are individually conserved.

The collision dissipates kinetic energy without changing the instantaneous tidal potential. Consequently the total [Jacobi energy in a shearing sheet](../../../gravitational-instability-of-an-astrophysical-disk.md#jacobi-energy-in-a-shearing-sheet) decreases. At any later time, writing $x_{0j}$ for the particles' current [epicyclic guiding center](../../../astrophysics.md#epicyclic-guiding-center) positions gives

$$
E=E_{\rm osc}-\frac38\Omega_0^2\sum_jx_{0j}^2,\qquad
E_{\rm osc}=\frac12\Omega_0^2\sum_j(|A_j|^2+|B_j|^2)\geq0.
$$

If $D\geq0$ is the accumulated energy dissipated in the [inelastic collisions](../../../classical-mechanics.md#inelastic-collision), comparison with the initial circular orbits gives

$$
\boxed{\sum_jx_{0j}^2
=\sum_jx_{0j,\rm initial}^2+\frac{8}{3\Omega_0^2}(D+E_{\rm osc})}.
$$

Thus the mean guiding-center position stays fixed, while its variance grows. The initial ensemble has no preference for positive or negative $x$, and the local equations and collision law preserve the symmetry $(x,y,z)\mapsto(-x,-y,z)$. The spreading is therefore symmetric in the ensemble average: [angular momentum transport](../../../classical-mechanics.md#angular-momentum-transport) moves some particles inward and others outward. A particular finite random realization need not be exactly symmetric. This is the microscopic energy argument for [dissipative spreading of a planetary ring](../../../gravitational-instability-of-an-astrophysical-disk.md#dissipative-spreading-of-a-planetary-ring).

## 3

↑ **Parent:** [Paper 321](paper-321.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

In the rotating [shearing sheet](../../../gravitational-instability-of-an-astrophysical-disk.md#shearing-sheet), write the background orbital shear as $\mathbf U_0=-q\Omega x\mathbf e_y$. The rotating momentum equation contains [Coriolis acceleration](../../../physics.md#coriolis-acceleration) $2\boldsymbol\Omega\times\mathbf u$ and the [shearing-sheet tidal potential](../../../gravitational-instability-of-an-astrophysical-disk.md#shearing-sheet-tidal-potential); the background shear balances the radial tidal acceleration.

Set

$$
\mathbf u=\mathbf U_0+(v_x(z,t),v_y(z,t),0),\qquad
\mathbf B=(B_x(z,t),B_y(z,t),B_z).
$$

[Gauss's law for magnetism](../../../electromagnetism.md#gauss-s-law-for-magnetism) gives $\partial_zB_z=0$, and the vertical [ideal magnetohydrodynamic induction equation](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-induction-equation) gives $\partial_tB_z=0$. Horizontal invariance and $v_z=0$ remove the nonlinear horizontal advection. The remaining background-shear term is $(\mathbf v\mathbin\cdot\nabla)\mathbf U_0=-q\Omega v_x\mathbf e_y$. The horizontal [magnetic tension](../../../astrophysical-fluid-dynamics.md#magnetic-tension) is $B_z\partial_z\mathbf B_h/\mu_0$, while horizontal pressure gradients vanish. Subtracting background balance yields

$$
\boxed{\partial_tv_x-2\Omega v_y=\frac{B_z}{\mu_0\rho}\partial_zB_x},\qquad
\boxed{\partial_tv_y+(2-q)\Omega v_x=\frac{B_z}{\mu_0\rho}\partial_zB_y}.
$$

For [ideal magnetohydrodynamics](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamics), the [ideal magnetohydrodynamic induction equation](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-induction-equation) is $\partial_t\mathbf B+\mathbf u\mathbin\cdot\nabla\mathbf B=\mathbf B\mathbin\cdot\nabla\mathbf u$. Its horizontal components give

$$
\boxed{\partial_tB_x=B_z\partial_zv_x},\qquad
\boxed{\partial_tB_y+q\Omega B_x=B_z\partial_zv_y}.
$$

These [horizontally invariant magnetized shearing-sheet equations](../../../astrophysics.md#horizontally-invariant-magnetized-shearing-sheet-equations) are exact within the stated local, incompressible ansatz, even for finite horizontal amplitudes. The vertical equation determines the pressure needed to balance vertical gravity and [magnetic pressure](../../../astrophysical-fluid-dynamics.md#magnetic-pressure); it does not add another horizontal evolution equation.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write $H=z^+$ and $B_+=B_x^+$, and assume $B_z\ne0$ and $q>0$. In a [steady state](../../../dynamical-systems.md#steady-state), the [horizontally invariant magnetized shearing-sheet equations](../../../astrophysics.md#horizontally-invariant-magnetized-shearing-sheet-equations) give

$$
v_x'=0,\qquad
B_y'=\frac{\mu_0\rho}{B_z}(2-q)\Omega v_x.
$$

Since $B_y$ vanishes at both boundaries, $v_x=0$ for $q\ne2$, and then $B_y=0$ throughout. The other two equations are

$$
v_y=-\frac{B_z}{2\mu_0\rho\Omega}B_x',\qquad
v_y'=\frac{q\Omega}{B_z}B_x.
$$

Eliminating $v_y$ gives the [harmonic oscillator equation](../../../classical-mechanics.md#simple-harmonic-motion)

$$
B_x''+K^2B_x=0,\qquad
K^2=\frac{2q\mu_0\rho\Omega^2}{B_z^2}.
$$

The midplane-symmetric [magnetic bending in an incompressible disk](../../../astrophysics.md#magnetic-bending-in-an-incompressible-disk) has odd $B_x$ and even $v_y$. Applying $B_x(\pm H)=\pm B_+$ gives

$$
\boxed{B_x=B_+\frac{\sin(Kz)}{\sin(KH)},\qquad B_y=0,\qquad v_x=0},
$$



$$
\boxed{v_y=-\frac{B_zKB_+}{2\mu_0\rho\Omega\sin(KH)}\cos(Kz)}.
$$

For nonzero imposed inclination $B_+$, this equilibrium exists only when $\sin(KH)\ne0$. More generally, $B_x=A\sin(Kz)+D\cos(Kz)$; the [boundary conditions](../../../differential-equation.md#boundary-condition) require $A\sin(KH)=B_+$ and $D\cos(KH)=0$. Thus the displayed solution is unique away from these resonances. At $\cos(KH)=0$, an additional even homogeneous solution is possible unless midplane symmetry is imposed. At $q=2$, an arbitrary constant $v_x$ is also allowed because its coefficient in the azimuthal equation vanishes; choosing $v_x=0$ gives the same symmetric equilibrium.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The [horizontally invariant magnetized shearing-sheet equations](../../../astrophysics.md#horizontally-invariant-magnetized-shearing-sheet-equations) are linear in the horizontal fields, so perturbations about the equilibrium satisfy the same equations. The fixed surface [boundary conditions](../../../differential-equation.md#boundary-condition) require $\delta B_x=\delta B_y=0$ at $z=\pm H$. Choose a [normal mode](../../../wave-equation.md#normal-mode) with

$$
(\delta B_x,\delta B_y)=(b_x,b_y)e^{st}\sin[k(z+H)],\qquad
(\delta v_x,\delta v_y)=(u,v)e^{st}\cos[k(z+H)],
$$

where the [vertical wavenumber](../../../partial-differential-equation.md#vertical-wavenumber) is $k=m\pi/(2H)$, $m=1,2,\ldots$. With the [Alfvén frequency](../../../astrophysical-fluid-dynamics.md#alfven-frequency)

$$
\omega_a^2=\frac{k^2B_z^2}{\mu_0\rho}=k^2v_{Az}^2,
$$

the four amplitude equations become

$$
su-2\Omega v=\frac{kB_z}{\mu_0\rho}b_x,\qquad
sv+(2-q)\Omega u=\frac{kB_z}{\mu_0\rho}b_y,
$$



$$
sb_x=-kB_zu,\qquad sb_y+q\Omega b_x=-kB_zv.
$$

Eliminating the velocities leaves

$$
(s^2+\omega_a^2-2q\Omega^2)b_x-2\Omega s b_y=0,\qquad
2\Omega s b_x+(s^2+\omega_a^2)b_y=0.
$$

A nonzero amplitude requires the [determinant](../../../linear-algebra.md#determinant) of this system to vanish, yielding the [ideal magnetorotational dispersion relation](../../../astrophysics.md#ideal-magnetorotational-dispersion-relation)

$$
\boxed{(s^2+\omega_a^2)(s^2+\omega_a^2-2q\Omega^2)+4\Omega^2s^2=0}.
$$

Equivalently, with $\kappa_r^2=2(2-q)\Omega^2$,

$$
s^4+(2\omega_a^2+\kappa_r^2)s^2+\omega_a^2(\omega_a^2-2q\Omega^2)=0.
$$

As a [quadratic equation](../../../polynomial.md#quadratic-equation) for $s^2$, its [discriminant](../../../polynomial.md#discriminant) is $\kappa_r^4+16\Omega^2\omega_a^2>0$. If $0<\omega_a^2<2q\Omega^2$, its constant term is negative, so one root $s^2$ is positive and there is an exponentially growing mode. If $\omega_a^2>2q\Omega^2$, both the constant term and the coefficient of $s^2$ are positive, giving two negative roots and only oscillatory modes. Equality is marginal.

The lowest allowed [vertical wavenumber](../../../partial-differential-equation.md#vertical-wavenumber), $k=\pi/(2H)$, is the last to be stabilized as $|B_z|$ increases. Therefore the [finite-thickness magnetorotational instability criterion](../../../astrophysics.md#finite-thickness-magnetorotational-instability-criterion) is

$$
\boxed{0<\frac{\pi^2B_z^2}{8q\mu_0\rho H^2\Omega^2}<1}.
$$

There is also a vertically uniform velocity mode with zero magnetic perturbation; for the usual orbitally stable regime $q<2$, it is just stable [epicyclic motion](../../../astrophysics.md#epicyclic-motion). For $q>2$, that uniform mode is already hydrodynamically unstable, independently of the magnetic criterion. At $q=2$ it is marginal. The criterion above concerns the magnetic modes.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Using $K^2=2q\mu_0\rho\Omega^2/B_z^2$, the [finite-thickness magnetorotational instability criterion](../../../astrophysics.md#finite-thickness-magnetorotational-instability-criterion) is precisely

$$
\boxed{KH>\frac\pi2}.
$$

For the midplane-symmetric equilibrium with $B_+\ne0$, the absolute radial [magnetic field](../../../electromagnetism.md#magnetic-field) is

$$
|B_x(z)|=\frac{|B_+|}{|\sin(KH)|}|\sin(Kz)|,\qquad 0\leq z\leq H.
$$

Its first maximum occurs at $z_* =\pi/(2K)$. The instability condition puts $z_*$ strictly inside the disc: $z_*<H$. The magnitude rises from zero to this maximum, then decreases on a nonempty interval before the surface. Thus the unstable equilibrium exhibits [nonmonotonic magnetic bending](../../../astrophysics.md#nonmonotonic-magnetic-bending), as illustrated below.

<a id="3/d/image-monotonic-and-nonmonotonic-magnetic-bending"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-321-magnetic-bending.png)

**[Figure 1](#3/d/image-monotonic-and-nonmonotonic-magnetic-bending). Monotonic and nonmonotonic magnetic bending**. The symmetric equilibrium profiles have $B_x(H)=B_+$. The weak-field example has an interior maximum and admits a growing magnetic mode.

The link between bending and instability concerns a nonzero imposed surface inclination. If $B_+=0$, the unbent equilibrium $B_x=0$ can still have [magnetorotational instability](../../../astrophysics.md#magnetorotational-instability); the literal nonmonotonic-bending conclusion does not apply to that degenerate case. Resonances with $\sin(KH)=0$ also require the separate equilibrium analysis in part (b).

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
