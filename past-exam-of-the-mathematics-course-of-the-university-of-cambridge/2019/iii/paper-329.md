# Paper 329

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_329.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_329.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 329](paper-329.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [material derivative](../../../continuum-mechanics.md#material-derivative) follows the interfacial [surfactant](../../../fluid-mechanics.md#surfactant). The term $-C\nabla_s\cdot\mathbf u_s$ describes dilution by tangential expansion and concentration by compression. The term $-C(\mathbf u\cdot\mathbf n)\nabla_s\cdot\mathbf n$ accounts for changing [surface area](../../../differential-geometry.md#surface-area) due to normal motion of a curved interface. Finally, $D_s\nabla_s^2C$ describes [surface diffusion](../../../fluid-mechanics.md#surface-diffusion). Together these give [conservation of insoluble surfactant on a moving interface](../../../fluid-mechanics.md#conservation-of-insoluble-surfactant-on-a-moving-interface).

The relevant surface [Péclet number](../../../fluid-mechanics.md#peclet-number) is

$$
\mathrm{Pe}_s=\frac{a^2|\mathbf A|}{D_s}\ll1.
$$

Write $S=\mathbf n\cdot\mathbf A\cdot\mathbf n$ and $\mathbf u_s=\mathbf A\mathbf x-S\mathbf x$. Since $\mathbf A$ has zero [trace](../../../linear-algebra.md#matrix-trace) and $\nabla_s\mathbf n=\mathbf I_s/a$, the [surface divergence](../../../riemannian-geometry.md#surface-divergence) is

$$
\nabla_s\cdot(\mathbf A\mathbf x)=\mathbf I_s:\mathbf A=-S,\qquad
\nabla_s\cdot(S\mathbf x)=2S,
\qquad\boxed{\nabla_s\cdot\mathbf u_s=-3S.}
$$

There is no normal motion. To first order in $\mathrm{Pe}_s$, the steady [surfactant](../../../fluid-mechanics.md#surfactant) balance becomes $D_s\nabla_s^2C'=C_0\nabla_s\cdot\mathbf u_s=-3C_0S$. The traceless quadratic $S$ is a degree-two [spherical harmonic](../../../analysis.md#spherical-harmonic), so $\nabla_s^2S=-6S/a^2$. The mean of $C'$ is zero by total [surfactant](../../../fluid-mechanics.md#surfactant) conservation; consequently

$$
\boxed{C'=KS,\qquad K=\frac{C_0a^2}{2D_s}.}
$$

The discarded advective term $\mathbf u_s\cdot\nabla_sC'$ is smaller by $\mathrm{Pe}_s$. This is the [quadrupolar surfactant distribution on a spherical interface](../../../fluid-mechanics.md#quadrupolar-surfactant-distribution-on-a-spherical-interface).

With the unit normal directed from the bubble into the exterior, the [interfacial stress balance with variable surface tension](../../../fluid-mechanics.md#interfacial-stress-balance-with-variable-surface-tension) is

$$
[\boldsymbol\sigma\cdot\mathbf n]_-^+=\gamma\kappa\mathbf n-\nabla_s\gamma.
$$

Using the specified first-order [curvature](../../../differential-geometry.md#curvature) and $\gamma=\gamma_0-K\gamma_1S$, together with $\nabla_sS=2\mathbf I_s\mathbf A\mathbf n/a$, gives

$$
\boxed{[\boldsymbol\sigma\cdot\mathbf n]_-^+=\frac{2\gamma_0}{a}\mathbf n+\frac{4\gamma_0}{a}(\mathbf n\cdot\mathbf D\cdot\mathbf n)\mathbf n+\frac{2K\gamma_1}{a}\left[\mathbf I_s\mathbf A\mathbf n-S\mathbf n\right].}
$$

The first term is the spherical [capillary pressure](../../../fluid-mechanics.md#capillary-pressure); the last contains the normal tension correction and the tangential [Marangoni stress](../../../fluid-mechanics.md#marangoni-effect).

The ambient [Stokes flow](../../../stokes-flow.md) has the symmetry of the symmetric traceless [tensor](../../../linear-algebra.md#tensor) $\mathbf E$. In the [Unscaled Papkovich–Neuber representation](../../../stokes-flow.md#unscaled-papkovich-neuber-representation), $\chi_\infty=\mathbf x\cdot\mathbf E\cdot\mathbf x/2$ is [harmonic](../../../partial-differential-equation.md#harmonic-function) and yields $\mathbf E\mathbf x$. The decaying vector potential must have the form $\mathbf E\nabla(1/r)$, and the scalar disturbance must have the degree-two form $\mathbf E:\nabla\nabla(1/r)$. They are [harmonic](../../../partial-differential-equation.md#harmonic-function) outside the bubble and have precisely the required rotational covariance. Dimensionless amplitudes may therefore be written

$$
\boldsymbol\Phi=\frac{Pa^3}{3}\mathbf E\nabla\frac1r,\qquad
\chi=\frac12\mathbf x\cdot\mathbf E\cdot\mathbf x+\frac{Qa^5}{3}\mathbf E:\nabla\nabla\frac1r.
$$

For a steady bubble, the [no-penetration boundary condition](../../../viscous-fluid-flow.md#no-penetration-boundary-condition) gives $1+P-3Q=0$. Its tangential velocity gives $\alpha=1+2Q$. The tangential [stress boundary condition](../../../viscous-fluid-flow.md#stress-boundary-condition) then yields

$$
2\mu(1+P-8Q)=\frac{2K\gamma_1}{a}\alpha,
\qquad
5(1-\alpha)=2M\alpha,
\qquad M=\frac{K\gamma_1}{\mu a}.
$$

Hence $\alpha=5/(5+2M)$, $Q=-M/(5+2M)$ and $P=-(5+5M)/(5+2M)$. The inviscid interior supplies only the constant pressure balancing $2\gamma_0/a$. Matching the remaining normal [stress](../../../continuum-mechanics.md#stress) gives

$$
2\mu(1-3P+12Q)=\frac{4\gamma_0}{a}\beta-2\mu M\alpha.
$$

Eliminating $P,Q,\alpha$ gives

$$
\boxed{\mathbf D=\frac{5\mu a}{\gamma_0}\frac{2+M}{5+2M}\mathbf E,\qquad\alpha=\frac5{5+2M}.}
$$

As $M\to\infty$, $\alpha\to0$: the [Marangoni stress](../../../fluid-mechanics.md#marangoni-effect) suppresses tangential motion and effectively immobilizes the interface. This limit must retain the small surface [Péclet number](../../../fluid-mechanics.md#peclet-number) and small-deformation assumptions; $M$ can grow through increasing $\gamma_1$ without invalidating the linear concentration approximation.

## 2

↑ **Parent:** [Paper 329](paper-329.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For the stated [axisymmetric flow](../../../fluid-mechanics.md#axisymmetric-flow), the diagonal components of the [rate-of-strain tensor](../../../viscous-fluid-flow.md#strain-rate-tensor) are

$$
e_{rr}=u_r,\qquad e_{\theta\theta}=u/r,\qquad e_{zz}=w_z.
$$

Their sum is $u_r+u/r+w_z=0$, the [incompressibility condition](../../../fluid-mechanics.md#incompressible-flow). In the leading thin-sheet approximation, vanishing tangential [traction](../../../continuum-mechanics.md#traction) makes $u$ independent of $z$. The normal [stress boundary condition](../../../viscous-fluid-flow.md#stress-boundary-condition) is $\sigma_{zz}=-p_{\rm ext}$, so the [Newtonian fluid stress tensor](../../../viscous-fluid-flow.md#newtonian-fluid-stress-tensor) gives

$$
p=p_{\rm ext}+2\mu w_z=p_{\rm ext}-2\mu(u_r+u/r).
$$

Therefore

$$
\boxed{\sigma_{rr}=-p_{\rm ext}+4\mu u_r+2\mu u/r,\qquad
\sigma_{\theta\theta}=-p_{\rm ext}+2\mu u_r+4\mu u/r.}
$$

For the small annular sector, the inner and outer radial faces contribute $2\delta\theta\,\partial_r(rh\sigma_{rr})\delta r$ in the radial direction. The two azimuthal faces contribute $-2\delta\theta\,h\sigma_{\theta\theta}\delta r$: their hoop [tractions](../../../continuum-mechanics.md#traction) have inward radial components. The combined radial force of the external pressure on the sloping upper and lower surfaces is $2\delta\theta\,r p_{\rm ext}h_r\delta r$.

<a id="2/image-forces-on-an-annular-viscous-sheet-sector-and-capillary-traction-at-a-hole-edge"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-329-sheet-forces.png)

**[Figure 1](#2/image-forces-on-an-annular-viscous-sheet-sector-and-capillary-traction-at-a-hole-edge). Forces on an annular viscous-sheet sector and capillary traction at a hole edge**. The left panel shows the radial and hoop tractions on the four vertical faces. The right panel shows the two surface-tension forces pulling the rounded hole edge into the sheet. The separate radial pressure force on the sloping broad surfaces is proportional to $p_{\rm ext}h_r$.

Neglecting inertia, [force balance](../../../classical-mechanics.md#force-balance) is thus

$$
\partial_r(rh\sigma_{rr})-h\sigma_{\theta\theta}+rp_{\rm ext}h_r=0.
$$

Substituting the two [stresses](../../../continuum-mechanics.md#stress) cancels the terms involving $p_{\rm ext}h_r$ and gives the [axisymmetric viscous-sheet stretching equations](../../../viscous-fluid-flow.md#axisymmetric-viscous-sheet-stretching-equations):

$$
\boxed{2\mu\left[\partial_r(2rhu_r+hu)-h(2u/r+u_r)\right]=rh\,\partial_rp_{\rm ext}.}
$$

Finally, [conservation of mass](../../../continuum-mechanics.md#mass-conservation) in the sector gives

$$
\boxed{h_t+\frac1r\partial_r(rhu)=0.}
$$

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Put $b=\Delta\rho\,g>0$, so $p_{\rm ext}=bh$. Balancing the viscous and pressure terms in the [axisymmetric viscous-sheet stretching equations](../../../viscous-fluid-flow.md#axisymmetric-viscous-sheet-stretching-equations), together with fixed [volume](../../../geometry-and-topology.md#volume), suggests a [similarity solution](../../../partial-differential-equation.md#similarity-solution)

$$
h=t^{-1}H(\eta),\qquad u=t^{-1/2}U(\eta),\qquad \eta=r/\sqrt t.
$$

The [conservation of mass](../../../continuum-mechanics.md#mass-conservation) equation becomes

$$
-H-\frac\eta2H'+\frac1\eta(\eta HU)'=0,
\qquad [\eta H(U-\eta/2)]'=0.
$$

There is no ongoing source at the origin, so the integration constant vanishes and $U=\eta/2$ wherever $H>0$. Thus $u=r/(2t)$. Substitution into radial [force balance](../../../classical-mechanics.md#force-balance) gives

$$
\left(\frac{3\mu}{t}-bh\right)h_r=0,
\qquad (3\mu-bH)H'=0.
$$

A differentiable $H$ cannot have nonzero derivative on an interval while being fixed there at $3\mu/b$. Hence $H'=0$: the spreading sheet has uniform thickness.

At the material edge, $R'=u(R,t)=R/(2t)$. Since $\sigma_{rr}=-bh+3\mu/t$, the edge condition $h\sigma_{rr}=-bh^2/2$ fixes $h=6\mu/(bt)$. Fixed [volume](../../../geometry-and-topology.md#volume) $V=\pi R^2h$ then fixes the radius. The [self-similar spreading of a viscous oil slick](../../../viscous-fluid-flow.md#self-similar-spreading-of-a-viscous-oil-slick) is

$$
\boxed{h(r,t)=\frac{6\mu}{\Delta\rho\,g\,t},\quad
u(r,t)=\frac r{2t},\quad
R(t)=\left(\frac{\Delta\rho\,g\,Vt}{6\pi\mu}\right)^{1/2},\qquad 0\leq r<R(t).}
$$

The point-release idealization is singular at $t=0$; a finite initial uniform slick gives the same solution with a time shift.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Each broad face supplies [surface tension](../../../fluid-mechanics.md#surface-tension) $\gamma$ pulling the rounded hole edge into the remaining sheet. Their resultant is $2\gamma$ per unit circumference. At the inner boundary the fluid's outward normal is $-\mathbf e_r$, so the boundary [traction](../../../continuum-mechanics.md#traction) is outward in the radial direction when $h\sigma_{rr}=-2\gamma$. The right panel of the preceding diagram shows these two capillary pulls.

With uniform thickness and $p_{\rm ext}=0$, the [axisymmetric viscous-sheet stretching equations](../../../viscous-fluid-flow.md#axisymmetric-viscous-sheet-stretching-equations) reduce to

$$
r u_{rr}+u_r-u/r=0.
$$

This [Euler-Cauchy equation](../../../differential-equation.md#euler-cauchy-equation) gives $u=Ar+B/r$. The fixed outer rim imposes $u(R_0)=0$, hence $B=-AR_0^2$. Because $(ru)_r/r=2A$, [conservation of mass](../../../continuum-mechanics.md#mass-conservation) gives $\dot h=-2Ah$, independent of $r$. Thus a uniform sheet remains uniform.

The radial [stress](../../../continuum-mechanics.md#stress) is $\sigma_{rr}=6\mu A-2\mu B/r^2$. Its value at the hole edge determines

$$
\boxed{A=-\frac{\gamma R^2}{\mu h(R_0^2+3R^2)},\qquad
B=\frac{\gamma R^2R_0^2}{\mu h(R_0^2+3R^2)}.}
$$

The edge is material, so $\dot R=u(R)$ and

$$
\dot R=\frac{\gamma R(R_0^2-R^2)}{\mu h(R_0^2+3R^2)}.
$$

Neglecting the initially tiny hole's volume, [conservation of mass](../../../continuum-mechanics.md#mass-conservation) gives $\pi h(R_0^2-R^2)=\pi h_0R_0^2$, or $h=h_0/(1-x^2)$ with $x=R/R_0$. Therefore the [capillary growth of a hole in a viscous sheet](../../../viscous-fluid-flow.md#capillary-growth-of-a-hole-in-a-viscous-sheet) obeys

$$
\boxed{\frac{dx}{dt}=\frac{\gamma}{\mu h_0}\frac{x(1-x^2)^2}{1+3x^2}.}
$$

For a finite initial hole $x_i$, replace $h_0$ in the denominator by $h_0(1-x_i^2)$. A nonzero seed is needed: the exact initial condition $x(0)=0$ gives the stationary solution of this differential equation. For a small positive seed, $x$ initially grows exponentially at rate $\gamma/(\mu h_0)$.

## 3

↑ **Parent:** [Paper 329](paper-329.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Reflection in $y=0$ preserves the prescribed translational [velocity](../../../classical-mechanics.md#velocity) and axial [angular velocity](../../../classical-mechanics.md#angular-velocity). A [force](../../../classical-mechanics.md#force) transforms as a polar [vector](../../../vector-space.md#vector), whereas a [torque](../../../classical-mechanics.md#torque) transforms as an axial vector; consequently $F_y=G_x=G_z=0$. Reflection in $x=0$ reverses both imposed motions but preserves the normal force component. The [linearity](../../../vector-space.md#linearity) of [Stokes flow](../../../stokes-flow.md) then gives $F_z=0$. Thus only $F_x$ and $G_y$ can be nonzero.

There is a sign inconsistency in the printed question. In right-handed coordinates, $\boldsymbol\Omega=\Omega\mathbf e_y$ gives a rotational velocity $-\Omega a\mathbf e_x$ at the sphere's lowest point. The printed shear and force formulas instead use the opposite rotational sense. Below, let $\omega$ be the right-handed component along $+\mathbf e_y$; the paper's displayed formulas are recovered by setting $\omega=-\Omega$.

In the translating frame, the parabolic gap and leading boundary velocities are

$$
h=a\epsilon+\frac{x^2+y^2}{2a},\qquad
\mathbf v_\parallel(0)=-U\mathbf e_x,\qquad
\mathbf v_\parallel(h)=-\omega a\mathbf e_x.
$$

The [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) and [lubrication theory](../../../viscous-fluid-flow.md#lubrication-theory) give

$$
\mathbf v_\parallel(z)=\frac{z(z-h)}{2\mu}\nabla_\parallel p-U\mathbf e_x+(U-\omega a)\frac zh\mathbf e_x,
\qquad
\mathbf q=-\frac{h^3}{12\mu}\nabla_\parallel p-\frac h2(U+\omega a)\mathbf e_x.
$$

The gap is stationary in this frame, so $\nabla_\parallel\cdot\mathbf q=0$. The [Reynolds lubrication equation](../../../viscous-fluid-flow.md#reynolds-equation) is therefore

$$
\nabla_\parallel\cdot(h^3\nabla_\parallel p)=-6\mu(U+\omega a)h_x.
$$

Since $h_x=x/a$ and $\nabla_\parallel^2h=2/a$,

$$
\nabla_\parallel\cdot\left[h^3\nabla_\parallel(x/h^2)\right]=-5x/a,
\qquad
\boxed{p=\frac{6\mu}{5}(U+\omega a)\frac{x}{h^2}.}
$$

Differentiating the velocity profile gives the leading [shear stresses](../../../viscous-fluid-flow.md#shear-stress)

$$
\begin{aligned}
\frac{\sigma_{xz}(0)}\mu&=\frac{6(U+\omega a)x^2}{5ah^2}+\frac{2U-8\omega a}{5h},\\
\frac{\sigma_{xz}(h)}\mu&=-\frac{6(U+\omega a)x^2}{5ah^2}+\frac{8U-2\omega a}{5h},\\
\frac{\sigma_{yz}(0)}\mu&=\frac{6(U+\omega a)xy}{5ah^2},\\
\frac{\sigma_{yz}(h)}\mu&=-\frac{6(U+\omega a)xy}{5ah^2}.
\end{aligned}
$$

The first expression becomes the printed formula after $\omega=-\Omega$.

For the [logarithmic lubrication resistance of a sphere near a wall](../../../viscous-fluid-flow.md#logarithmic-lubrication-resistance-of-a-sphere-near-a-wall), write $\ell=\log(1/\epsilon)$. The logarithmic region is $a\sqrt\epsilon\ll r\ll a$, where $h\sim r^2/(2a)$. Consequently

$$
\int\frac{dx\,dy}{h}=2\pi a\ell+O(a),\qquad
\int\frac{x^2\,dx\,dy}{ah^2}=2\pi a\ell+O(a).
$$

These follow from $\int r/h\,dr=a\ell+O(a)$ and $\int r^3/h^2\,dr=2a^2\ell+O(a^2)$, with a fixed small outer cutoff. The general logarithmic radial numerator is $r^{2n-1}$ over $h^n$; the numerator in the printed integration hint appears to have a typographical error.

The force exerted on the fluid through the upper gap boundary includes pressure acting on its slope:

$$
F_x=\int\left[\sigma_{xz}(h)+p h_x\right]dx\,dy.
$$

The pressure cancels the $x^2/h^2$ term, giving

$$
\boxed{F_x=\frac{4\pi\mu a}{5}(4U-\omega a)\ell+O\!\left(\mu a(|U|+a|\omega|)\right).}
$$

Pressure exerts no [torque](../../../classical-mechanics.md#torque) about the centre of a sphere because its traction is radial. To logarithmic order, the shear has lever arm $-a\mathbf e_z$, so

$$
G_y=-a\int\sigma_{xz}(h)dx\,dy
=\frac{4\pi\mu a^2}{5}(4\omega a-U)\ell+O\!\left(\mu a^2(|U|+a|\omega|)\right).
$$

The other components vanish by parity: $G_x$ involves an integral of the $xy$ term, and $G_z$ has an integrand odd in $y$. The combined [hydrodynamic resistance matrix](../../../stokes-flow.md#hydrodynamic-resistance-matrix) is

$$
\boxed{\begin{pmatrix}F_x\\G_y/a\end{pmatrix}\sim\frac{4\pi\mu a}{5}\ell\begin{pmatrix}4&-1\\-1&4\end{pmatrix}\begin{pmatrix}U\\a\omega\end{pmatrix}.}
$$

Its equal off-diagonal coefficients are required by the [Lorentz reciprocal theorem for Stokes flow](../../../stokes-flow.md#lorentz-reciprocal-theorem-for-stokes-flow). It is a [positive-definite matrix](../../../linear-algebra.md#positive-definite-matrix), as required by [viscous dissipation](../../../stokes-flow.md#viscous-dissipation).

In the rotational convention of the printed force formula, set $\Omega=-\omega$ and measure the scalar couple along $-\mathbf e_y$, so $G=-G_y$. Then

$$
\boxed{F\sim\frac{4\pi\mu a}{5}(4U+a\Omega)\ell,\qquad
G\sim\frac{4\pi\mu a^2}{5}(U+4a\Omega)\ell.}
$$

For sedimentation under the buoyancy-adjusted weight $F$, a uniform sphere is [torque-free](../../../stokes-flow.md#torque-free). Thus $\omega a=U/4$, and the force balance gives

$$
\boxed{U\sim\frac{F}{3\pi\mu a\log(1/\epsilon)},\qquad
\omega\sim\frac{F}{12\pi\mu a^2\log(1/\epsilon)}.}
$$

The rotational scalar in the paper's displayed-force convention is $\Omega=-U/(4a)$. The sphere rolls in the right-handed $+\mathbf e_y$ sense but still slips: its lowest point has laboratory velocity $U-a\omega=3U/4$. The signs and coefficients of the right-handed resistance agree with the rigid-wall terms of [Bertin et al., equations (4.4)–(4.5)](https://vincent-bertin.github.io/Papers/09_Bertin2022JFM.pdf), after reversing the forces and torques there from fluid-on-sphere to sphere-on-fluid.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
