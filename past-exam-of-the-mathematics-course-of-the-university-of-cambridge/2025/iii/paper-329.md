# Paper 329

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_329.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_329.pdf)

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
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 329](paper-329.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [Papkovich–Neuber representation](../../../stokes-flow.md#papkovich-neuber-representation) writes a homogeneous [Stokes flow](../../../stokes-flow.md) in terms of a [harmonic vector field](../../../partial-differential-equation.md#harmonic-function) $\boldsymbol\Phi$ and a harmonic scalar $\chi$ as

$$
\mu\mathbf u=\boldsymbol\Phi-\frac12\nabla(\mathbf x\mathbin\cdot\boldsymbol\Phi)+\nabla\chi,
\qquad
p=-\nabla\mathbin\cdot\boldsymbol\Phi.
$$

For translation, rotational symmetry and decay at infinity restrict the trial harmonic fields to the fundamental harmonic $1/r$ and its directional derivatives contracted with $\mathbf U$. For rotation, the only decaying isotropic axial-vector field with the required boundary value is proportional to $\boldsymbol\Omega\times\mathbf x/r^3$. Matching the [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) $\mathbf u=\mathbf U+\boldsymbol\Omega\times\mathbf x$ at $r=a$ gives the superposition of the [translating sphere in Stokes flow](../../../stokes-flow.md#translating-sphere-in-stokes-flow) and the [rotating sphere in Stokes flow](../../../stokes-flow.md#rotating-sphere-in-stokes-flow):

$$
\boxed{
\mathbf u=
\frac{3a}{4r}\left(\mathbf I+\frac{\mathbf x\mathbf x}{r^2}\right)\mathbf U
+\frac{a^3}{4r^3}\left(\mathbf I-3\frac{\mathbf x\mathbf x}{r^2}\right)\mathbf U
+\frac{a^3}{r^3}\boldsymbol\Omega\times\mathbf x,
\qquad
p=\frac{3\mu a}{2r^3}\mathbf U\mathbin\cdot\mathbf x .}
$$

Each term decays at infinity, and direct substitution at $r=a$ gives the prescribed rigid velocity.

When $\mathbf U=0$, the pressure is constant and may be set to zero. Differentiating the rotational velocity and using the [Newtonian fluid stress tensor](../../../viscous-fluid-flow.md#newtonian-fluid-stress-tensor) gives

$$
\boxed{
\boldsymbol\sigma
=-\frac{3\mu a^3}{r^5}
\left[(\boldsymbol\Omega\times\mathbf x)\mathbf x
+\mathbf x(\boldsymbol\Omega\times\mathbf x)\right].}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For two zero-body-force [Stokes flows](../../../stokes-flow.md) $(\mathbf u,\boldsymbol\sigma)$ and $(\widehat{\mathbf u},\widehat{\boldsymbol\sigma})$ in the same domain, the [Lorentz reciprocal theorem for Stokes flow](../../../stokes-flow.md#lorentz-reciprocal-theorem-for-stokes-flow) states

$$
\int_{\partial D}\mathbf u\mathbin\cdot\widehat{\boldsymbol\sigma}\mathbf n\,dS
=\int_{\partial D}\widehat{\mathbf u}\mathbin\cdot\boldsymbol\sigma\mathbf n\,dS.
$$

Apply it first with the auxiliary translating-sphere solution and then with the auxiliary rotating-sphere solution. The swimmer is [force-free](../../../stokes-flow.md#force-free) and [torque-free](../../../stokes-flow.md#torque-free), while the auxiliary surface tractions are known. The resulting [surface slip velocity](../../../stokes-flow.md#surface-slip-velocity) formulas are

$$
\boxed{
\mathbf V=-\frac1{4\pi a^2}\int_{r=a}\mathbf u_s\,dS,
\qquad
\boldsymbol\omega=-\frac3{8\pi a^4}\int_{r=a}\mathbf x\times\mathbf u_s\,dS.}
$$

On $r=a$, the first part of the prescribed slip is

$$
\frac{(\mathbf A\times\mathbf x)\times\mathbf x}{a^2}
=\frac{\mathbf x(\mathbf A\mathbin\cdot\mathbf x)}{a^2}-\mathbf A.
$$

Its surface average is $-2\mathbf A/3$, whereas the $\mathbf B$ term has zero average by [oddness](../../../calculus.md#odd-function). Thus

$$
\boxed{\mathbf V=\frac23\mathbf A.}
$$

The $\mathbf A$ term contributes no rotation. For the other term, the isotropic second and fourth surface moments give

$$
\int_{r=a}\mathbf x\times\mathbf u_s\,dS
=\frac{8\pi a^3}{15}|\mathbf B|^2\mathbf B,
$$

and hence

$$
\boxed{\boldsymbol\omega=-\frac{|\mathbf B|^2}{5a}\mathbf B.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

When $\mathbf B=0$, part (b) gives $\mathbf V=2\mathbf A/3$ and $\boldsymbol\omega=0$. The total boundary velocity is therefore

$$
\mathbf V+\mathbf u_s
=-\frac13\mathbf A+\frac{\mathbf x(\mathbf A\mathbin\cdot\mathbf x)}{a^2}.
$$

The decaying [velocity potential](../../../fluid-mechanics.md#velocity-potential)

$$
\phi=-\frac{a^3}{3}\frac{\mathbf A\mathbin\cdot\mathbf x}{r^3}
$$

is harmonic for $r>a$, and

$$
\boxed{\mathbf u=\nabla\phi
=-\frac{a^3}{3}\nabla\left(\frac{\mathbf A\mathbin\cdot\mathbf x}{r^3}\right)}
$$

has exactly this value at $r=a$. It is a force-free potential-dipole field and decays as $r^{-3}$.

When $\mathbf A=0$, define the degree-three [harmonic polynomial](../../../partial-differential-equation.md#harmonic-polynomial)

$$
H_3(\mathbf x)=(\mathbf B\mathbin\cdot\mathbf x)^3
-\frac35|\mathbf B|^2r^2(\mathbf B\mathbin\cdot\mathbf x).
$$

An appropriate decaying harmonic potential is

$$
\Psi=C\frac{H_3(\mathbf x)}{r^7},
\qquad
\mathbf u=\nabla\Psi\times\mathbf x.
$$

Indeed, the tangential boundary value is proportional to

$$
\left[\frac{(\mathbf B\mathbin\cdot\mathbf x)^2}{a^3}
-\frac{|\mathbf B|^2}{5a}\right]\mathbf B\times\mathbf x,
$$

which combines the prescribed slip with the rigid rotation found in part (b). Since $H_3/r^7=O(r^{-4})$ and multiplication of its gradient by $\mathbf x$ preserves that order, the exterior velocity decays as

$$
\boxed{|\mathbf u|=O(r^{-4}).}
$$

## 2

↑ **Parent:** [Paper 329](paper-329.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $z$ increase downward. The [slender viscous thread](../../../viscous-fluid-flow.md#slender-viscous-thread) is locally in uniaxial extension. The transverse stress equals the ambient pressure, so the [Trouton ratio](../../../rheology.md#trouton-ratio) gives the excess axial stress $\sigma_{zz}+p_e=3\mu w_z$. [Mass conservation](../../../continuum-mechanics.md#mass-conservation) and axial force balance therefore give

$$
\boxed{A_t+(Aw)_z=0,}
\qquad
\boxed{\rho gA+\partial_z(3\mu A w_z)=0.}
$$

In steady flow $Aw=Q$. Dividing the momentum equation by $A=Q/w$ gives

$$
3\mu w\left(\frac{w_z}{w}\right)_z+\rho g=0.
$$

With $w=\widehat wW$ and $z=\widehat zZ$, choose

$$
\boxed{\widehat z=\left(\frac{3\mu\widehat w}{\rho g}\right)^{1/2}.}
$$

The dimensionless equation becomes

$$
W\left(\frac{W'}W\right)'=-1,
\qquad
WW''-(W')^2=-W.
$$

Treating $(W')^2$ as a function of $W$ and using an [integrating factor](../../../differential-equation.md#integrating-factor) yields

$$
\boxed{\frac12(W')^2=CW^2+W.}
$$

Because $A=Q/(\widehat wW)$, the area sketches are the reciprocals of the functions $W$ found below. The dimensional vertical deviatoric stress is

$$
\boxed{\sigma_{zz}+p_e=\frac{3\mu\widehat w}{\widehat z}W'.}
$$

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

For $C=0$, the increasing branch with $W(0)=0$ satisfies $W'=\sqrt{2W}$, hence

$$
\boxed{W(Z)=\frac12Z^2,
\qquad A(Z)\propto\frac2{Z^2}.}
$$

The thread thins algebraically, and the tensile vertical stress is proportional to $W'=Z$.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

For $C=1/2$,

$$
(W')^2=W^2+2W=(W+1)^2-1,
$$

so

$$
\boxed{W(Z)=\cosh Z-1,
\qquad A(Z)\propto\frac1{\cosh Z-1}.}
$$

The thread thins exponentially for large $Z$, and its tensile stress is proportional to $\sinh Z$.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

For $C=-1/2$,

$$
(W')^2=2W-W^2=1-(W-1)^2,
$$

so the branch emerging from zero is

$$
\boxed{W(Z)=1-\cos Z,
\qquad A(Z)\propto\frac1{1-\cos Z}.}
$$

The area decreases until $Z=\pi$, where $W=2$ and the vertical deviatoric stress, proportional to $W'=\sin Z$, vanishes. A formal continuation beyond that point has compressive stress and thickens until the model reaches another zero of $W$; unlike the first two cases, it does not describe indefinite monotone drawing.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The broad faces have curvature zero to leading order, so their [stress boundary condition](../../../viscous-fluid-flow.md#stress-boundary-condition) gives $\sigma_{xx}=-p_e$. The semicircular edges have curvature $1/h$, giving $\sigma_{yy}=-p_e-\gamma/h$. [Incompressible flow](../../../fluid-mechanics.md#incompressible-flow) gives $u_x+v_y+w_z=0$; uniform transverse normal stresses imply uniform transverse extension rates, and eliminating them from the [Newtonian fluid stress tensor](../../../viscous-fluid-flow.md#newtonian-fluid-stress-tensor) yields

$$
\boxed{\sigma_{zz}=-p_e-\frac{\gamma}{2h}+3\mu w'.}
$$

At an edge, the [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition) balances axial advection of $b$, lateral strain, and capillary retraction. This gives

$$
\boxed{wb'+\frac b2w'+\frac{\gamma b}{4\mu h}=0.}
$$

The equation $hbw=Q$ expresses conservation of volume flux, while

$$
3\mu hbw'+\frac{\gamma b}{2}=F
$$

states that the total axial tension is constant. Define

$$
\boxed{\Gamma=\frac\gamma{\mu Q},
\qquad T=\frac F{\mu Q}.}
$$

Then $[\Gamma]=L^{-2}$ and $[T]=L^{-1}$, and substitution of $h=Q/(bw)$ gives

$$
\frac{b'}b+\frac12\frac{w'}w=-\frac{\Gamma b}{4},
\qquad
3\frac{w'}w=-\frac{\Gamma b}{2}+T.
$$

Subtracting these logarithmic-derivative equations gives

$$
\left(\log\frac wb\right)'=\frac T2,
\qquad
\boxed{w(z)=\frac{w(0)}{b_0},b(z)e^{Tz/2}.}
$$

The remaining width equation is

$$
\frac{b'}b=-\frac{\Gamma b+T}{6}.
$$

Thus, for $T\ne0$,

$$
\boxed{
\frac1{b(z)}=\frac{e^{Tz/6}}{b_0}
+\frac\Gamma T\left(e^{Tz/6}-1\right),}
$$

while the continuous $T=0$ limit is $1/b=1/b_0+\Gamma z/6$.

If $\Gamma=0$, then $b/b_0=e^{-Tz/6}$, $w/w(0)=e^{Tz/3}$, and [mass conservation](../../../continuum-mechanics.md#mass-conservation) gives $h/h(0)=e^{-Tz/6}$. Therefore a prescribed thinning ratio $R=h(L)/h(0)$ requires

$$
\boxed{F=\mu QT
=\frac{6\mu Q}{L}\log\frac{h(0)}{h(L)}.}
$$

## 3

↑ **Parent:** [Paper 329](paper-329.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

In the cylinder frame the wall moves at velocity $-U$. The [parabolic lubrication gap](../../../viscous-fluid-flow.md#parabolic-lubrication-gap) and its natural stretched coordinate are

$$
h(x)=\frac{\epsilon a}{2}+\frac{x^2}{2a}
=\frac{\epsilon a}{2}(1+\xi^2),
\qquad
\xi=\frac{x}{a\sqrt\epsilon}.
$$

The wall values are $u(0)=-U$ and $u(h)=\Omega a$ to leading order. The [Couette-Poiseuille flow in a thin gap](../../../viscous-fluid-flow.md#couette-poiseuille-flow-in-a-thin-gap) is therefore

$$
u(x,y)=-U+\frac{U+\Omega a}{h}y
+\frac{p_x}{2\mu}y(y-h),
$$

and its constant flux is

$$
q=\frac h2(\Omega a-U)-\frac{h^3}{12\mu}p_x.
$$

The [pressure recovery condition in lubrication flow](../../../viscous-fluid-flow.md#pressure-recovery-condition-in-lubrication-flow) gives $\int_{-\infty}^{\infty}p_xdx=0$. Since

$$
\frac{\int h^{-2}dx}{\int h^{-3}dx}
=\frac{2\epsilon a}{3},
$$

it follows that

$$
\boxed{q=\frac13\epsilon a(\Omega a-U),}
\qquad
p_x=\frac{6\mu(\Omega a-U)}{h^2}-\frac{12\mu q}{h^3}.
$$

Differentiating the velocity profile gives the two surface shear stresses

$$
\boxed{
\left.\frac{\sigma_{xy}}\mu\right|_{y=0}
=\frac{4U-2\Omega a}{h}+\frac{6q}{h^2},
\qquad
\left.\frac{\sigma_{xy}}\mu\right|_{y=h}
=\frac{-2U+4\Omega a}{h}-\frac{6q}{h^2}.}
$$

Using $\int h^{-1}dx=2\pi/\sqrt\epsilon$ and $\int h^{-2}dx=2\pi/(a\epsilon^{3/2})$, the shear force exerted by the fluid on the wall is

$$
\boxed{F^{(s)}_{\rm wall}=\frac{4\pi\mu U}{\sqrt\epsilon},}
$$

and that exerted by the fluid on the cylinder is

$$
\boxed{F^{(s)}_{\rm cyl}=-\frac{4\pi\mu\Omega a}{\sqrt\epsilon}.}
$$

They are not equal and opposite because pressure acting on the sloping cylinder surface also transfers tangential momentum. Indeed, integration by parts gives the cylinder's pressure force

$$
F^{(p)}_{\rm cyl}=\int hp_x\,dx
=\frac{4\pi\mu(\Omega a-U)}{\sqrt\epsilon},
$$

so its total leading hydrodynamic force is $-4\pi\mu U/\sqrt\epsilon$.

The cylinder's excess weight per unit axial length is $\pi a^2\Delta\rho g$ in the falling direction, and it has no gravitational couple about its axis. Force and couple balance therefore give

$$
\boxed{U=\frac{a^2\Delta\rho g}{4\mu}\sqrt\epsilon,}
\qquad
\boxed{\Omega=0\quad\hbox{at leading order}.}
$$

The second result follows because the leading viscous couple is $-4\pi\mu\Omega a^2/\sqrt\epsilon$.

For $\Omega=0$, write $h=(\epsilon a/2)(1+\xi^2)$. Then

$$
p_x=\frac{2\mu U}{h^2}\frac{1-3\xi^2}{1+\xi^2},
\qquad
\sigma_{xy}(x,h)=\frac{2\mu U}{h}\frac{1-\xi^2}{1+\xi^2}.
$$

Thus $p$ is an odd pressure disturbance that vanishes at $x=0$ and at both infinities; its extrema occur at $\xi=\pm1/\sqrt3$. The cylinder shear is positive near the narrowest point, negative in the outer parts of the gap, and vanishes at

$$
\boxed{x=\pm a\sqrt\epsilon.}
$$

The [streamlines](../../../fluid-mechanics.md#streamline) pass through the gap in the wall's direction overall. Pressure-driven backflow bends the interior streamlines and creates the two shear-reversal locations on the cylinder; the streamline sketch is symmetric under a half-turn combined with reversal of the flow direction.

For the final [Couette flow](../../../viscous-fluid-flow.md#couette-flow), the lower and upper minimum gaps are $\epsilon a(1+\lambda)/2$ and $\epsilon a(1-\lambda)/2$. If the cylinder translates at speed $V$, the two leading lubrication drags are proportional to

$$
-\frac{U+V}{\sqrt{1+\lambda}}
\quad\hbox{and}\quad
\frac{U-V}{\sqrt{1-\lambda}}.
$$

The [force-free](../../../stokes-flow.md#force-free) condition gives

$$
\boxed{
V=U\frac{\sqrt{1+\lambda}-\sqrt{1-\lambda}}
{\sqrt{1+\lambda}+\sqrt{1-\lambda}}
=\frac{\lambda U}{1+\sqrt{1-\lambda^2}}.}
$$

For $\lambda=0$, $V=0$ and the streamlines in the two equal gaps are mirror images with opposite directions. The $O(\mu U a)$ subleading wall-driven couple must balance the leading rotational resistance $O(\mu\Omega a^2/\sqrt\epsilon)$, so

$$
\boxed{\Omega=O(\epsilon^{1/2}U/a).}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
