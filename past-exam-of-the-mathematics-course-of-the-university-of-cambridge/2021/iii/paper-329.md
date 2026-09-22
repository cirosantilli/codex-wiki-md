# Paper 329

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_329.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_329.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)

## 1

↑ **Parent:** [Paper 329](paper-329.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

In a cross-section normal to the cylinder axes, measure $y$ from the line of contact. The two circular boundaries have the [parabolic approximation](../../../calculus.md#parabolic-approximation)

$$
h(y)=\frac{y^2}{a}+O\left(\frac{y^4}{a^3}\right)
$$

for their separation. The contact point of the meniscus is at $y=w+o(w)$, so the leading cross-sectional area is

$$
\boxed{A(w)=\int_0^w\frac{y^2}{a}\,dy=\frac{w^3}{3a}}.
$$

The area of the small meniscus cap is $O(w^4/a^2)$ and is lower order. At its upper end the gap has width $h(w)=w^2/a$. A tangent semicircle therefore has radius $w^2/(2a)$ and [curvature](../../../differential-geometry.md#curvature)

$$
\boxed{\kappa=\frac{2a}{w^2}}.
$$

The [Young–Laplace equation](../../../fluid-mechanics.md#young-laplace-equation) makes the liquid pressure, relative to the nearly uniform gas pressure,

$$
p=-\gamma\kappa=-\frac{2\gamma a}{w^2},
\qquad
p_z=\frac{4\gamma a}{w^3}w_z.
$$

At a fixed $y$, [lubrication theory](../../../viscous-fluid-flow.md#lubrication-theory) gives a planar [Poiseuille flow](../../../viscous-fluid-flow.md#hagen-poiseuille-equation) through a gap of width $h(y)$, with axial flux per unit $y$

$$
dQ=-\frac{h(y)^3}{12\mu}p_z\,dy.
$$

Integrating across the cusp,

$$
Q=-\frac{p_z}{12\mu}\int_0^w\frac{y^6}{a^3}\,dy
=-\frac{p_zw^7}{84\mu a^3}
=-\frac{\gamma}{21\mu a^2}w^4w_z.
$$

The [continuity equation](../../../physics.md#continuity-equation) $A_t+Q_z=0$ now gives

$$
\boxed{
\frac{\partial w^3}{\partial t}
=\frac{\gamma}{7\mu a}
\frac\partial{\partial z}
\left(w^4\frac{\partial w}{\partial z}\right)}.
$$

Set $q=w^3$. Since $w^4w_z=\frac15(q^{5/3})_z$, this is the [porous medium equation](../../../diffusion-equation.md#porous-medium-equation)

$$
q_t=K(q^{5/3})_{zz},
\qquad
K=\frac{\gamma}{35\mu a}.
$$

Conservation of the fixed volume

$$
V=\int_{\mathbb R}A\,dz
=\frac1{3a}\int_{\mathbb R}q\,dz
$$

and [dimensional analysis](../../../physics.md#dimensional-analysis) give the [self-similar solution](../../../partial-differential-equation.md#similarity-solution) $q=t^{-3/8}F(z/t^{3/8})$. One integration of the resulting ordinary differential equation yields the compactly supported [Barenblatt solution](../../../diffusion-equation.md#barenblatt-solution)

$$
F(\eta)=\left(C-B\eta^2\right)_+^{3/2},
\qquad
B=\frac{21\mu a}{8\gamma}.
$$

Equivalently,

$$
w(z,t)=t^{-1/8}
\left(C-B\frac{z^2}{t^{3/4}}\right)_+^{1/2}.
$$

Its tip is $z_N=(C/B)^{1/2}t^{3/8}$. Using

$$
\int_{-1}^1(1-s^2)^{3/2}\,ds=\frac{3\pi}{8}
$$

in the volume constraint gives $C^2=8aV\sqrt B/\pi$. Therefore

$$
\boxed{
z_N(t)=\left(\frac{8Va}{\pi}\right)^{1/4}
\left(\frac{8\gamma t}{21\mu a}\right)^{3/8}}.
$$

For vertical cylinders at equilibrium, [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure) gives $p-p_{\rm atm}=-\rho gz$. Balancing this with the [capillary pressure](../../../fluid-mechanics.md#capillary-pressure) $-2\gamma a/w^2$ gives the large-height profile

$$
\boxed{w(z)\sim\left(\frac{2\gamma a}{\rho gz}\right)^{1/2}}.
$$

## 2

↑ **Parent:** [Paper 329](paper-329.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

More surfactant is encountered on the side toward which the far-field concentration $\Gamma$ increases. Adsorption lowers the [surface tension](../../../fluid-mechanics.md#surface-tension) there, so the resulting [Marangoni stress](../../../fluid-mechanics.md#marangoni-effect) drives interfacial flow toward the cleaner, higher-tension side. The reaction force propels the bubble along the concentration gradient; this is [chemophoresis](../../../fluid-mechanics.md#chemophoresis).

The bulk concentration obeys the [advection-diffusion equation](../../../diffusion-equation.md#advection-diffusion-equation)

$$
\frac{\partial\Gamma}{\partial t}
+\mathbf u\mathbin\cdot\nabla\Gamma
=D\nabla^2\Gamma.
$$

At $r=a$,

$$
D\mathbf n\mathbin\cdot\nabla\Gamma=-k(C-b\Gamma)
$$

equates the outward bulk diffusive flux to minus the net adsorption rate: $C>b\Gamma$ favors desorption into the bulk, while $C<b\Gamma$ favors adsorption onto the interface.

With advection neglected, $\Gamma$ is [harmonic](../../../partial-differential-equation.md#harmonic-function). Rotational symmetry about $\mathbf G$ and the imposed far-field gradient select the dipolar form

$$
\Gamma=\Gamma_0+\mathbf G\mathbin\cdot\mathbf x
+B\frac{\mathbf G\mathbin\cdot\mathbf x}{r^3}.
$$

When $kab\ll D$, the boundary flux is smaller than the characteristic diffusive flux, so the leading boundary condition is $\partial_r\Gamma=0$ at $r=a$. This gives $B=a^3/2$, and hence

$$
\boxed{\Gamma(a,\mathbf n)=\Gamma_0+\frac32a\mathbf G\mathbin\cdot\mathbf n}.
$$

For an interface with unit normal directed from the bubble into the exterior liquid, the [interfacial stress balance with variable surface tension](../../../fluid-mechanics.md#interfacial-stress-balance-with-variable-surface-tension) may be written

$$
(\boldsymbol\sigma-\boldsymbol\sigma^{\rm in})\mathbin\cdot\mathbf n
=\gamma\kappa\mathbf n-\nabla_s\gamma,
$$

with signs tied to the stated curvature convention. Put $C'=A\mathbf G\mathbin\cdot\mathbf n$ and $\gamma=\gamma_0-\gamma_1C'$. The constant part of the normal traction is balanced by the uniform bubble pressure. Since $\kappa=2/a$ and

$$
\nabla_s(\mathbf G\mathbin\cdot\mathbf n)
=\frac1a(I-\mathbf n\mathbf n)\mathbin\cdot\mathbf G,
$$

the remaining exterior traction is

$$
\boxed{
\boldsymbol\sigma\mathbin\cdot\mathbf n
=\frac{\gamma_1A}{a}
\left\{\mathbf G-3(\mathbf G\mathbin\cdot\mathbf n)\mathbf n\right\}}.
$$

Its resultant vanishes because

$$
\int_{S_a}\mathbf n\mathbf n\,dS
=\frac{4\pi a^2}{3}I,
$$

and therefore the integrals of the two terms cancel. This is required because the bubble and its interfacial stresses exert no external body force on the combined bubble–fluid system.

The traction is a first spherical harmonic, so the decaying, force-free [Stokes flow](../../../stokes-flow.md) has no [Stokeslet](../../../stokes-flow.md#stokeslet) and is generated by the indicated [Papkovich–Neuber representation](../../../stokes-flow.md#papkovich-neuber-representation). Comparing the supplied traction

$$
\frac{3\beta}{a}
\{\mathbf G-3(\mathbf G\mathbin\cdot\mathbf n)\mathbf n\}
$$

with the capillary traction gives

$$
\boxed{\beta=\frac{\gamma_1A}{3}}.
$$

In the convention for these potentials, the normal velocity at $r=a$ is $(\beta/\mu)\mathbf G\mathbin\cdot\mathbf n$. The [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition) for a translating sphere is $\mathbf u\mathbin\cdot\mathbf n=\mathbf U\mathbin\cdot\mathbf n$, so

$$
\boxed{\mathbf U=\frac{\gamma_1A}{3\mu}\mathbf G}.
$$

Linearize the surface transport equation about $C=C_0$ by writing $C=C_0+C'$ and neglecting products of small perturbations. The tangential velocity relative to the translating bubble obtained from the same potential is

$$
\mathbf u_s=-\frac{\gamma_1A}{2\mu}
(I-\mathbf n\mathbf n)\mathbin\cdot\mathbf G.
$$

Using the identities supplied in the question,

$$
\nabla_s\mathbin\cdot\mathbf u_s
=\frac{\gamma_1A}{\mu a}\mathbf G\mathbin\cdot\mathbf n,
\qquad
\nabla_s^2C'=-\frac{2A}{a^2}\mathbf G\mathbin\cdot\mathbf n.
$$

The bulk result gives $\Gamma'=\frac32a\mathbf G\mathbin\cdot\mathbf n$ on the surface. The linearized equation

$$
C_0\nabla_s\mathbin\cdot\mathbf u_s
=D_s\nabla_s^2C'-k(C'-b\Gamma')
$$

then yields

$$
A\left(k+\frac{2D_s}{a^2}
+\frac{\gamma_1C_0}{\mu a}\right)
=\frac32kab.
$$

Thus

$$
\boxed{
A=\frac{3kab/2}
{k+2D_s/a^2+\gamma_1C_0/(\mu a)}}.
$$

Increasing $k$ strengthens exchange with the imposed bulk gradient, so $A$ and $U$ increase toward a saturation value. Increasing $D_s$ smooths surface-concentration differences and decreases $U$. Increasing $C_0$ strengthens advective redistribution of the background surfactant; the resulting feedback opposes the imposed dipole, so $U$ decreases.

## 3

↑ **Parent:** [Paper 329](paper-329.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Near the closest point, the cylinder–plane gap is

$$
h(x)=\frac a2\varepsilon+\frac{x^2}{2a}
=\frac a2(\varepsilon+\xi^2),
\qquad
\xi=\frac xa.
$$

For translation parallel to the cylinder axis, the leading flow is [Couette flow](../../../viscous-fluid-flow.md#couette-flow). Its shear traction is $\mu U/h$, so

$$
\frac{F_y}{U}
=\mu L\int_{-\infty}^{\infty}\frac{dx}{h(x)}
=2\mu L\int_{-\infty}^{\infty}
\frac{d\xi}{\varepsilon+\xi^2}
=\boxed{2\pi\varepsilon^{-1/2}\mu L}.
$$

Hence $A_{yy}=2\pi\varepsilon^{-1/2}\mu L$.

For transverse translation, the local [Couette-Poiseuille flow in a thin gap](../../../viscous-fluid-flow.md#couette-poiseuille-flow-in-a-thin-gap) and mass conservation give the [Reynolds lubrication equation](../../../viscous-fluid-flow.md#reynolds-equation). Writing $x=a\sqrt\varepsilon\,X$ and using pressure recovery at both ends determines its integration constant. The pressure and viscous contributions to the horizontal traction reduce to

$$
\frac{F_x}{U}
=\frac{\mu L}{\sqrt\varepsilon}
\left(16I_2-16I_3\right)
=\frac{\mu L}{\sqrt\varepsilon}
\left(8\pi-6\pi\right)
+\frac{2\pi\mu L}{\sqrt\varepsilon},
$$

where the final term is the direct Couette shear contribution. Therefore

$$
\boxed{A_{xx}=4\pi\varepsilon^{-1/2}\mu L}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Treat each short torus segment as a straight cylinder. For translation with velocity $U\mathbf e_x$, its components normal and tangent to the circular centreline are $U\cos\theta$ and $-U\sin\theta$. Integrating the local resistance per unit length around $ds=R\,d\theta$ gives

$$
\begin{aligned}
A_{xx}
&=\mu\varepsilon^{-1/2}R
\int_0^{2\pi}
(4\pi\cos^2\theta+2\pi\sin^2\theta)\,d\theta\\
&=\boxed{6\pi^2\mu R\varepsilon^{-1/2}}.
\end{aligned}
$$

Rotation at angular velocity $\Omega\mathbf e_z$ gives the everywhere tangential speed $\Omega R$. Only the axial-cylinder resistance $2\pi\mu\varepsilon^{-1/2}$ contributes. Multiplying the force by its moment arm $R$ and integrating around the centreline gives

$$
\boxed{D_{zz}=4\pi^2\mu R^3\varepsilon^{-1/2}}.
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

In the torus frame the two planes translate with velocity $U\mathbf e_x$. Away from the $O(a)$ neighborhood of the torus, the depth-averaged [Hele-Shaw flow](../../../viscous-fluid-flow.md#hele-shaw-flow) between planes separated by $2a$ is

$$
\overline{\mathbf u}
=U\mathbf e_x-\frac{a^2}{3\mu}\nabla p,
\qquad
\nabla^2p=0.
$$

Negligible leakage imposes $\overline u_r=0$ at $r=R$. The harmonic pressure that decays at infinity in the exterior and the regular harmonic pressure in the interior are therefore

$$
\boxed{
p_{>}(r,\theta)
=-\frac{3\mu UR^2}{a^2r}\cos\theta,
\qquad
p_{<}(r,\theta)
=\frac{3\mu U}{a^2}r\cos\theta},
$$

up to a common constant. The interior velocity is zero, while the exterior flow is the uniform stream diverted around a circular obstacle. In plan view the inside has high pressure on the $+x$ side and low pressure on the $-x$ side; the immediately adjacent exterior has the opposite signs, producing the pressure jump across the torus.

The jump at $r=R$ is

$$
p_<-p_>=\frac{6\mu UR}{a^2}\cos\theta.
$$

Integrating it over the projected vertical area $2aR\,d\theta$ gives the global pressure resistance

$$
\boxed{F_x\sim\frac{12\pi\mu UR^2}{a}}.
$$

There are two narrow gaps, so their local resistance is twice the one-plane result from part b:

$$
F_{\rm gap}\sim12\pi^2\mu UR\varepsilon^{-1/2}.
$$

Consequently the local gap resistance dominates when $a\ll R\ll a\varepsilon^{-1/2}$, whereas the global Hele–Shaw pressure resistance dominates when

$$
a\varepsilon^{-1/2}\ll R\ll a\varepsilon^{-5/2}.
$$

To interpret the upper bound, the pressure jump has scale $\Delta p\sim\mu UR/a^2$. Each narrow gap has thickness $a\varepsilon$ and streamwise lubrication length $a\sqrt\varepsilon$. Its pressure-driven leakage flux per unit centreline length therefore scales as

$$
q_{\rm leak}
\sim\frac{(a\varepsilon)^3}{\mu a\sqrt\varepsilon}\Delta p
\sim UR\varepsilon^{5/2}.
$$

The blocked Hele–Shaw flux has scale $Ua$. Leakage is negligible precisely when $UR\varepsilon^{5/2}\ll Ua$, or

$$
\boxed{R\ll a\varepsilon^{-5/2}}.
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
