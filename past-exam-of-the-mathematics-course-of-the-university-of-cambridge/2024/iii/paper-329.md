# Paper 329

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_329.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_329.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
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

## 1

↑ **Parent:** [Paper 329](paper-329.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Put $\delta=H/L\ll1$. In a thin gap, the streamwise [Stokes flow](../../../stokes-flow.md) balance is

$$
\frac PL\sim\mu\frac U{H^2},
$$

so $P\sim\mu UL/H^2$. The characteristic [shear stress](../../../viscous-fluid-flow.md#shear-stress) is $\tau\sim\mu U/H$, and therefore

$$
\boxed{\frac\tau P\sim\frac HL=\delta\ll1}.
$$

This is the [pressure-dominance scaling of lubrication theory](../../../viscous-fluid-flow.md#lubrication-pressure-dominates-shear-stress).

Let the centre displacement be $\lambda\Delta$ in the downward direction. To first order in $\Delta/a$, projecting this displacement onto the radial direction at polar angle $\theta$ changes the concentric gap $\Delta$ by $-\lambda\Delta\cos\theta$. Hence

$$
\boxed{h(\theta)=\Delta(1-\lambda\cos\theta)}.
$$

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

Axisymmetric [mass conservation](../../../continuum-mechanics.md#mass-conservation) in the spherical gap gives

$$
\frac{\partial h}{\partial t}
+\frac1{a\sin\theta}
\frac{\partial}{\partial\theta}(q\sin\theta)=0.
$$

Since $h_t=-V\cos\theta$ and regularity requires $q\sin\theta=0$ at $\theta=0$, integration gives

$$
q\sin\theta
=aV\int_0^\theta\sin\vartheta\cos\vartheta\,d\vartheta
=\frac12aV\sin^2\theta,
\qquad
\boxed{q=\frac12Va\sin\theta}.
$$

The leading [pressure-driven lubrication flux](../../../viscous-fluid-flow.md#hagen-poiseuille-equation) is

$$
q=-\frac{h^3}{12\mu a}\frac{dp}{d\theta}.
$$

Substitution of $h$ and $q$ gives

$$
\frac{dp}{d\theta}
=-\frac{6\mu a^2V\sin\theta}
{\Delta^3(1-\lambda\cos\theta)^3},
$$

and therefore

$$
\boxed{
p(\theta)=
\frac{3\mu a^2V}
{\lambda\Delta^3(1-\lambda\cos\theta)^2}+p_0}.
$$

Take downward as the positive vertical direction. The constant pressure contributes no resultant, while the pressure force on the inner sphere is opposite its outward normal. Thus

$$
F_z=-2\pi a^2\int_0^\pi
(p-p_0)\cos\theta\sin\theta\,d\theta.
$$

With $t=\lambda\cos\theta$ and the supplied integral,

$$
\boxed{
F_z=-\frac{6\pi\mu a^4V}{\lambda^3\Delta^3}
\left[
\frac{2\lambda}{1-\lambda^2}
+\log\left(\frac{1-\lambda}{1+\lambda}\right)
\right]}.
$$

The sign is upward for $V>0$, so this is a [drag force](../../../fluid-mechanics.md#drag-physics). As $\lambda\to0$, the bracket is $4\lambda^3/3+O(\lambda^5)$ and $F_z\to-8\pi\mu a^4V/\Delta^3$.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Rotation about the vertical axis gives the inner surface the azimuthal speed $\Omega a\sin\theta$. The leading [Couette flow](../../../viscous-fluid-flow.md#couette-flow) shear traction is opposing and has magnitude

$$
\frac{\mu\Omega a\sin\theta}{h(\theta)}.
$$

Its moment arm about the vertical axis is $a\sin\theta$, and $dS=2\pi a^2\sin\theta\,d\theta$. Consequently

$$
G_z=-\frac{2\pi\mu\Omega a^4}{\Delta}
\int_0^\pi\frac{\sin^3\theta}{1-\lambda\cos\theta}\,d\theta.
$$

Putting $t=\lambda\cos\theta$ and using the supplied integral gives

$$
\boxed{
G_z=-\frac{2\pi\mu\Omega a^4}{\lambda^3\Delta}
\left[
2\lambda+(1-\lambda^2)
\log\left(\frac{1-\lambda}{1+\lambda}\right)
\right]}.
$$

This [viscous shear torque](../../../viscous-fluid-flow.md#viscous-shear-torque) opposes the rotation. Its concentric limit is $-8\pi\mu\Omega a^4/(3\Delta)$, agreeing with the thin-gap limit of [Torque in rotational Stokes flow between concentric spheres](../../../stokes-flow.md#torque-in-rotational-stokes-flow-between-concentric-spheres).

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

A rotation by $\pi$ about the vertical symmetry axis maps a horizontal angular velocity $\boldsymbol\Omega'$ to $-\boldsymbol\Omega'$ but leaves a possible vertical force unchanged. Linearity and uniqueness of [Stokes flow](../../../stokes-flow.md) therefore require that vertical force to equal its own negative, so it vanishes. A horizontal force and a horizontal couple are allowed by the same symmetry.

Write $\lambda=1-\epsilon$ and examine the lower pole, where $\theta\ll1$. Since $\cos\theta=1-\theta^2/2+O(\theta^4)$,

$$
h=\Delta\left[\epsilon+\frac{\theta^2}{2}
+O(\epsilon\theta^2+\theta^4)\right].
$$

Thus $h=O(\epsilon\Delta)$ for $\theta=O(\epsilon^{1/2})$, a circular patch of radius

$$
\boxed{\ell=O(a\epsilon^{1/2})}.
$$

In the broad region, the surface speed is $O(\Omega'a)$, the shear is $O(\mu\Omega'a/\Delta)$, the area is $O(a^2)$, and the moment arm is $O(a)$. Hence

$$
G'_{\rm broad}=O\left(\frac{\mu\Omega'a^4}{\Delta}\right).
$$

In the narrow patch, the shear rises to $O(\mu\Omega'a/(\epsilon\Delta))$, while its area falls to $O(\epsilon a^2)$; the moment arm remains $O(a)$. Therefore

$$
\boxed{G'_{\rm patch}=G'_{\rm broad}
=O\left(\frac{\mu\Omega'a^4}{\Delta}\right)}.
$$

Dropping the moment arm gives the shear-force scale. Pressure produces the same horizontal order after multiplication by the small surface slope. Both regions consequently contribute

$$
\boxed{F'_{\rm patch}=F'_{\rm broad}
=O\left(\frac{\mu\Omega'a^3}{\Delta}\right)}.
$$

## 2

↑ **Parent:** [Paper 329](paper-329.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For two body-force-free [Stokes flows](../../../stokes-flow.md) $(\mathbf u^{(1)},\boldsymbol\sigma^{(1)})$ and $(\mathbf u^{(2)},\boldsymbol\sigma^{(2)})$ in the same domain, the [Lorentz reciprocal theorem for Stokes flow](../../../stokes-flow.md#lorentz-reciprocal-theorem-for-stokes-flow) is

$$
\int_{\partial\mathcal D}
\mathbf u^{(1)}\mathbin\cdot\boldsymbol\sigma^{(2)}\mathbf n\,dS
=
\int_{\partial\mathcal D}
\mathbf u^{(2)}\mathbin\cdot\boldsymbol\sigma^{(1)}\mathbf n\,dS.
$$

Indeed, the difference of the two volume integrands is

$$
\nabla\mathbf u^{(1)}:\boldsymbol\sigma^{(2)}
-\nabla\mathbf u^{(2)}:\boldsymbol\sigma^{(1)}=0
$$

because both flows are incompressible and the [Newtonian fluid stress tensor](../../../viscous-fluid-flow.md#newtonian-fluid-stress-tensor) is symmetric. The [divergence theorem](../../../calculus.md#divergence-theorem) proves the boundary identity.

On a rigid body, $\mathbf u^{(r)}=\mathbf U^{(r)}+\boldsymbol\Omega^{(r)}\times\mathbf x$. The reciprocal theorem becomes

$$
\mathbf U^{(1)}\mathbin\cdot\mathbf F^{(2)}
+\boldsymbol\Omega^{(1)}\mathbin\cdot\mathbf G^{(2)}
=
\mathbf U^{(2)}\mathbin\cdot\mathbf F^{(1)}
+\boldsymbol\Omega^{(2)}\mathbin\cdot\mathbf G^{(1)}.
$$

Writing $(\mathbf F,\mathbf G)^T=\mathsf R(\mathbf U,\boldsymbol\Omega)^T$ and choosing arbitrary pairs of rigid velocities shows that

$$
\boxed{\mathsf R=\mathsf R^T}.
$$

**Thus the [hydrodynamic resistance matrix](../../../stokes-flow.md#hydrodynamic-resistance-matrix) is symmetric.**

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The body is invariant under the reflections and half-turns that preserve its $z$-axis. A polar vector force $F\mathbf e_z$ can therefore produce only the polar velocity $U_z\mathbf e_z$; every rotation is excluded because [angular velocity](../../../classical-mechanics.md#angular-velocity) is a [pseudovector](../../../vector-space.md#pseudovector). Hence only $U_z$ is nonzero when $\mathbf F=(0,0,F)$ and $\mathbf G=0$.

For $\mathbf F=(F,0,0)$, the surviving symmetry-allowed components are

$$
\boxed{U_x\ne0,\qquad\Omega_y\ne0},
$$

while $U_y,U_z,\Omega_x,\Omega_z$ vanish. The coupling between translation in $x$ and rotation about $y$ is permitted because the two horizontal rods lie at opposite vertical offsets.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For pure translation, integrate the [slender-body force density](../../../stokes-flow.md#slender-body-force-density) over each rod and take its moment about $O$. The three coordinate directions give

$$
\begin{array}{c|c|c}
\mathbf U&\mathbf F/(CL U)&\mathbf G/(CL^2U)\\ \hline
U\mathbf e_x&(5,0,0)&(0,1,0)\\
U\mathbf e_y&(0,5,0)&(1,0,0)\\
U\mathbf e_z&(0,0,5)&(0,0,0).
\end{array}
$$

Thus

$$
\mathbf F=5CL\mathbf U,
\qquad
\mathbf G=CL^2(U_y,U_x,0)
$$

when $\boldsymbol\Omega=0$.

Let

$$
K=\begin{pmatrix}0&1&0\\1&0&0\\0&0&0\end{pmatrix},
\qquad
D=\begin{pmatrix}13/3&0&0\\0&13/3&0\\0&0&4/3\end{pmatrix}.
$$

The symmetry proved in part (a) determines the force generated by rotation from the translation-generated couple. Combining this with the given rotational resistance gives the complete matrix

$$
\boxed{
\begin{pmatrix}\mathbf F\\\mathbf G\end{pmatrix}
=C
\begin{pmatrix}
5L I&L^2K\\
L^2K&L^3D
\end{pmatrix}
\begin{pmatrix}\mathbf U\\\boldsymbol\Omega\end{pmatrix}}.
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The zero-couple equations in the two coupled horizontal blocks are

$$
L\Omega_y=-\frac3{13}U_x,
\qquad
L\Omega_x=-\frac3{13}U_y,
$$

and $\Omega_z=0$. The force equations then become

$$
k_x=5U_x+L\Omega_y=\frac{62}{13}U_x,
\qquad
k_y=\frac{62}{13}U_y,
\qquad
k_z=5U_z.
$$

Therefore

$$
\boxed{\alpha=\frac{13}{62},\qquad\gamma=\frac3{62}},
$$

and

$$
\boxed{
\mathbf U=\left(\frac{13}{62}k_x,
\frac{13}{62}k_y,\frac15k_z\right),
\qquad
L\boldsymbol\Omega
=-\frac3{62}(k_y,k_x,0)}.
$$

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

A vector fixed in space has [body-frame derivative of a space-fixed vector](../../../classical-mechanics.md#body-frame-derivative-of-a-space-fixed-vector)

$$
\left(\frac{d\mathbf k}{dt}\right)_{\rm body}
=-\boldsymbol\Omega\times\mathbf k.
$$

Substitution of part (d) gives

$$
\boxed{
\frac d{dt}(k_x,k_y,k_z)
=\frac\gamma L
(k_xk_z,-k_yk_z,k_y^2-k_x^2)}.
$$

If $\boldsymbol\Omega$ is constant and nonzero, then $k_x$ and $k_y$ are constant and not both zero. Their evolution equations force $k_z=0$, and the last equation then gives $k_x^2=k_y^2$. Hence

$$
\boxed{\mathbf k\parallel(1,1,0)
\quad\text{or}\quad
\mathbf k\parallel(1,-1,0)}.
$$

For $\mathbf k=(1,1,0)$, both the translational velocity and the angular velocity are parallel to the fixed vertical force, with the latter oppositely directed. The body therefore falls on a straight vertical line while spinning steadily about that line. Its body $z$-axis remains horizontal, and its $x$- and $y$-axes remain at $45^\circ$ to the vertical.

For the initial condition $(1,0,0)$, symmetry preserves $k_y=0$. With $c=\gamma/L$ the exact body-frame solution is

$$
k_x=\operatorname{sech}(ct),
\qquad
k_z=-\tanh(ct).
$$

The body rotates about its $y$-axis, its fall path bends slightly because the horizontal and axial mobilities differ, and $\mathbf k\to(0,0,-1)$. Thus the body $z$-axis becomes vertical and the angular velocity tends to zero; asymptotically it falls without rotating.

## 3

↑ **Parent:** [Paper 329](paper-329.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For an axisymmetric surface $r=a(z,t)$, twice the [mean curvature](../../../second-fundamental-form.md#mean-curvature) with the outward-normal convention is

$$
\kappa=\frac1{a\sqrt{1+a_z^2}}
-\frac{a_{zz}}{(1+a_z^2)^{3/2}}.
$$

Writing $a=a_0+\eta$ and retaining linear terms gives

$$
\boxed{\kappa=\frac1{a_0}
-\frac{\eta}{a_0^2}-\eta_{zz}},
\qquad
\kappa'= -\frac{\eta}{a_0^2}-\eta_{zz}.
$$

At the unperturbed boundary $r=a_0$, the linearized [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition), tangential-stress condition, and [Young–Laplace equation](../../../fluid-mechanics.md#young-laplace-equation) are

$$
u=\eta_t,
\qquad
\sigma_{rz}=\mu(u_z+w_r)=0,
\qquad
p'-2\mu u_r=\gamma\kappa'.
$$

For a normal mode $e^{ikz+st}$ these become $u(a_0)=s\eta$, $\sigma_{rz}(a_0)=0$, and

$$
p'(a_0)-2\mu u_r(a_0)
=\gamma(k^2-a_0^{-2})\eta.
$$

The [Papkovich–Neuber representation](../../../stokes-flow.md#papkovich-neuber-representation) of body-force-free [Stokes flow](../../../stokes-flow.md) is

$$
2\mu\mathbf u=\nabla(\mathbf x\mathbin\cdot\boldsymbol\Phi+\chi)-2\boldsymbol\Phi,
\qquad
p=\nabla\mathbin\cdot\boldsymbol\Phi,
$$

where $\boldsymbol\Phi$ and $\chi$ are harmonic.

Let $x=kr$ and $E=e^{ikz+st}$. Substitution of the given radial vector potential and scalar potential gives

$$
\boxed{
u=\frac{E}{2\mu}
\left[P(xI_1'(x)-I_1(x))+QI_0'(x)\right]},
$$



$$
\boxed{
w=\frac{iE}{2\mu}
\left[PxI_1(x)+QI_0(x)\right]},
\qquad
p=PkI_0(x)E.
$$

Using the [modified Bessel function](../../../analysis.md#modified-bessel-function) identity $(xI_1)'=xI_0$, the tangential stress simplifies to

$$
\boxed{
\sigma_{rz}=ikE
\left[PxI_1'(x)+QI_0'(x)\right]}.
$$

The stress-free condition at $r=a$ therefore yields

$$
\boxed{PxI_1'(x)+QI_0'(x)=0
\quad\text{at }x=ka}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The expression in braces in the first equation is the net axial force. The term $-\pi a^2\gamma/a$ is the compressive force from the [capillary pressure](../../../fluid-mechanics.md#capillary-pressure) $\gamma/a$, $3\pi\mu a^2w_z$ is the Newtonian extensional tension with [Trouton ratio](../../../rheology.md#trouton-ratio) three, and $2\pi a\gamma$ is the axial pull of [surface tension](../../../fluid-mechanics.md#surface-tension) around the circumference. Its $z$-derivative vanishes because axial force is conserved.

The final equation is conservation of an [insoluble surfactant](../../../fluid-mechanics.md#insoluble-surfactant). The surface divergence $w_z+u/a$ is the sum of axial and circumferential extension rates. Positive surface divergence increases interfacial area and dilutes $C$; negative divergence concentrates it. The absence of a diffusion term expresses the assumption of negligible surface diffusion.

Linearizing the area and surfactant equations gives

$$
2\eta_t=-a_0w_z,
\qquad
C'_t=-C_0\left(w_z+\frac{\eta_t}{a_0}\right)
=\frac{C_0}{a_0}\eta_t.
$$

Thus

$$
\frac\partial{\partial t}(a_0C'-C_0\eta)=0,
$$

and hence

$$
\boxed{a_0C'(z,t)=C_0\eta(z,t)+\psi(z)},
$$

where $\psi$ is fixed by the initial data.

Linearizing the displayed net axial force and using $\gamma'=-AC'$ gives

$$
3\pi\mu a_0^2w_z+\pi\gamma_0\eta
-\pi Aa_0C'=0.
$$

Eliminating $w_z$ and $C'$ therefore gives directly

$$
6\mu a_0\eta_t
=(\gamma_0-AC_0)\eta-A\psi(z).
$$

Thus the three displayed evolution equations imply

$$
\boxed{
\eta_t=s\eta-\frac{A\psi(z)}{6\mu a_0},
\qquad
s=\frac{\gamma_0-AC_0}{6\mu a_0}}.
$$

The target formula printed later in the paper contains an additional factor of $\pi$ in both denominators. That factor does not follow from the displayed equations because every term in the axial-force balance contains the same factor $\pi$. If the target formula is adopted as the intended normalization, its corresponding value is $s=(\gamma_0-AC_0)/(6\pi\mu a_0)$.

Initially $\eta=0$ and $C'>0$, so $\psi>0$ and $\eta_t<0$: a surfactant-rich, low-tension region begins to neck as neighboring higher tension pulls fluid away. The accompanying axial extension dilutes the surfactant.

If $A<\gamma_0/C_0$, then $s>0$. The [Rayleigh–Plateau instability](../../../fluid-mechanics.md#rayleigh-plateau-instability) overwhelms the weak surface-elastic response: the necking perturbation grows in the linear model while the original concentration excess is diluted and eventually changes sign.

If $A>\gamma_0/C_0$, then $s<0$. Strong surface elasticity arrests the disturbance at

$$
\eta_\infty=\frac{A\psi}{\gamma_0-AC_0}<0.
$$

The concentration perturbation becomes negative, raising the local surface tension until its axial force balances that of the wider regions. This is stabilization by a [surfactant-induced Marangoni stress](../../../fluid-mechanics.md#marangoni-effect).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The condition $a\gamma=a_0\gamma_0$ makes the leading extensional axial force uniform, but it does not make the [capillary pressure](../../../fluid-mechanics.md#capillary-pressure) uniform. Since

$$
p_c=\frac\gamma a=\frac{a_0\gamma_0}{a^2},
$$

a nonuniform radius gives a nonuniform pressure. Its axial gradient must drive flow, so the prediction $w=0$ is inconsistent.

For $a=a_0+\eta$ varying over the axial scale $L$,

$$
p_c'\sim\frac{\gamma_0\eta}{a_0^2},
\qquad
\frac{\partial p_c}{\partial z}
\sim\frac{\gamma_0\eta}{a_0^2L}.
$$

An axial [Hagen-Poiseuille flow](../../../viscous-fluid-flow.md#hagen-poiseuille-equation) in a cylinder has speed scale

$$
w\sim\frac{a_0^2}{\mu}\frac{\partial p_c}{\partial z}
\sim\frac{\gamma_0\eta}{\mu L}.
$$

Cross-sectional [mass conservation](../../../continuum-mechanics.md#mass-conservation) gives $\eta_t\sim a_0w/L$, and consequently

$$
\boxed{
\frac{\partial\eta}{\partial t}
\sim\frac{\gamma_0a_0}{\mu L^2}\eta}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
