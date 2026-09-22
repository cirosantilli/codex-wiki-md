# Paper 329

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_329.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_329.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
    - [iii](#1/c/iii)
      - [Solution](#1/c/iii/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 329](paper-329.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the [Papkovich–Neuber representation](../../../stokes-flow.md#papkovich-neuber-representation) in the form

$$
\mu\mathbf u=\boldsymbol\Phi-\frac12\nabla(\mathbf x\mathbin\cdot\boldsymbol\Phi)+\nabla\chi,
\qquad
p=-\nabla\mathbin\cdot\boldsymbol\Phi,
$$

where $\boldsymbol\Phi$ and $\chi$ are [harmonic functions](../../../partial-differential-equation.md#harmonic-function). A torque is a [axial vector](../../../vector-space.md#pseudovector), so rotational covariance and decay select the harmonic vector field

$$
\boldsymbol\Phi=\frac{\mathbf G\times\mathbf x}{8\pi r^3},
\qquad \chi=0.
$$

Here $\mathbf x\cdot\boldsymbol\Phi=0$ and $\nabla\cdot\boldsymbol\Phi=0$, so

$$
\boxed{\mathbf u(\mathbf x)=\frac{\mathbf G\times\mathbf x}{8\pi\mu r^3},\qquad p=0.}
$$

This [rotlet](../../../stokes-flow.md#rotlet) equals the [rotating sphere in Stokes flow](../../../stokes-flow.md#rotating-sphere-in-stokes-flow)

$$
\mathbf u=\frac{a^3}{r^3}\boldsymbol\Omega\times\mathbf x
$$

when $\boldsymbol\Omega=\mathbf G/(8\pi\mu a^3)$. It satisfies the [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) on $r=a$, decays at infinity, and its [Newtonian fluid stress tensor](../../../viscous-fluid-flow.md#newtonian-fluid-stress-tensor) transmits the applied couple $\mathbf G$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put $S(\mathbf x)=\mathbf x\cdot\mathbf A\cdot\mathbf x$. Since $\mathbf u=-Sr^{-5}\mathbf x$ and $\nabla\times\mathbf x=0$, the [product rule](../../../calculus.md#product-rule) gives

$$
\boldsymbol\omega=\nabla\times\mathbf u
=\nabla(-Sr^{-5})\times\mathbf x.
$$

For the symmetric [stresslet](../../../stokes-flow.md#force-dipole-flow) tensor $\mathbf A$,

$$
\nabla(Sr^{-5})=2r^{-5}\mathbf A\cdot\mathbf x-5Sr^{-7}\mathbf x.
$$

The final term is parallel to $\mathbf x$ and drops out of the [cross product](../../../vector-space.md#cross-product), leaving

$$
\boxed{\boldsymbol\omega(\mathbf x)=\frac{2\mathbf x\times(\mathbf A\cdot\mathbf x)}{r^5}.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

The [Linearity of Stokes flow](../../../stokes-flow.md#linearity-of-stokes-flow) makes every velocity linear in $\mathbf G_1$. The only available isotropic polar vector built from the axial vector $\mathbf G_1$ and separation vector $\mathbf R$ is $\mathbf G_1\times\mathbf R$. [Dimensional analysis](../../../physics.md#dimensional-analysis) then gives

$$
\mathbf U_i=\alpha_i(R/a)\frac{\mathbf G_1\times\mathbf R}{\mu a^3}.
$$

An angular velocity is axial, so the two independent isotropic possibilities are $\mathbf G_1$ and $(\mathbf G_1\cdot\mathbf R)\mathbf R$. Hence

$$
\boxed{
\boldsymbol\Omega_i
=\frac1{\mu a^3}\left[
\beta_i(R/a)\mathbf G_1
+\gamma_i(R/a)\frac{(\mathbf G_1\cdot\mathbf R)\mathbf R}{R^2}
\right],}
$$

for dimensionless scalar functions $\beta_i,\gamma_i$.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Write $\boldsymbol\Omega=\mathbf G_1/(8\pi\mu a^3)$. The incident [rotlet](../../../stokes-flow.md#rotlet) of sphere 1 at sphere 2 is

$$
\mathbf u_\infty(\mathbf R)=a^3\frac{\boldsymbol\Omega\times\mathbf R}{R^3},
$$

and it is harmonic away from sphere 1. Since sphere 2 is [force-free](../../../stokes-flow.md#force-free), [Faxén's first law](../../../stokes-flow.md#faxen-s-first-law) therefore gives

$$
\boxed{\mathbf U_2=a^3\frac{\boldsymbol\Omega\times\mathbf R}{R^3}.}
$$

The [vorticity](../../../fluid-mechanics.md#vorticity) of the rotlet is

$$
\boldsymbol\omega_\infty(\mathbf R)
=\frac{a^3}{R^3}\left[
3\frac{(\boldsymbol\Omega\cdot\mathbf R)\mathbf R}{R^2}
-\boldsymbol\Omega
\right].
$$

Because $\mathbf G_2=0$, [Faxén's rotational law](../../../stokes-flow.md#faxen-s-rotational-law) gives

$$
\boxed{\boldsymbol\Omega_2
=\frac{a^3}{2R^3}\left[
3\frac{(\boldsymbol\Omega\cdot\mathbf R)\mathbf R}{R^2}
-\boldsymbol\Omega
\right].}
$$

The symmetric [rate-of-strain tensor](../../../viscous-fluid-flow.md#strain-rate-tensor) of the incident rotlet at sphere 2 is

$$
\mathbf E=-\frac{3a^3}{2R^5}\left[
(\boldsymbol\Omega\times\mathbf R)\mathbf R
+\mathbf R(\boldsymbol\Omega\times\mathbf R)
\right].
$$

After translation and rotation have matched the uniform and antisymmetric parts of the incident flow, the leading perturbation from sphere 2 is the [stresslet](../../../stokes-flow.md#force-dipole-flow) part of the supplied straining-sphere solution:

$$
\boxed{\mathbf u_2'(\mathbf x)
\sim-\frac{5a^3}{2}\frac{(\mathbf x\cdot\mathbf E\cdot\mathbf x)\mathbf x}{r^5}.}
$$

Part b gives its vorticity as

$$
\boldsymbol\omega_2'=5a^3\frac{\mathbf x\times(\mathbf E\cdot\mathbf x)}{r^5}.
$$

At the centre of sphere 1, $\mathbf x=-\mathbf R$, so

$$
\boldsymbol\omega_2'(-\mathbf R)
=-\frac{15a^6}{2R^6}\left[
\boldsymbol\Omega-\frac{(\boldsymbol\Omega\cdot\mathbf R)\mathbf R}{R^2}
\right].
$$

Applying [Faxén's rotational law](../../../stokes-flow.md#faxen-s-rotational-law) to sphere 1 produces half this ambient vorticity and proves

$$
\boxed{
\boldsymbol\Omega_1-\boldsymbol\Omega
=-\frac{15a^6}{4R^6}\left[
\boldsymbol\Omega-\frac{(\boldsymbol\Omega\cdot\mathbf R)\mathbf R}{R^2}
\right].}
$$

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

To hold sphere 2 fixed against the incident angular velocity from part ii, its applied couple must generate the bare rotation

$$
\widetilde{\boldsymbol\Omega}_2
=\frac{\mathbf G_2}{8\pi\mu a^3}
=-\frac{a^3}{2R^3}\left[
3\frac{(\boldsymbol\Omega\cdot\mathbf R)\mathbf R}{R^2}
-\boldsymbol\Omega
\right].
$$

The resulting [rotlet](../../../stokes-flow.md#rotlet) advects the force-free sphere 1. Since the field is harmonic, [Faxén's first law](../../../stokes-flow.md#faxen-s-first-law) gives

$$
\mathbf U_1
=a^3\frac{\widetilde{\boldsymbol\Omega}_2\times(-\mathbf R)}{R^3}
=\boxed{-\frac{a^6}{2R^6}\boldsymbol\Omega\times\mathbf R}.
$$

The returned rotlet has velocity $O(\Omega a^6/R^5)$ and rate of strain $O(\Omega a^6/R^6)$ at sphere 1. That strain induces a [stresslet](../../../stokes-flow.md#force-dipole-flow) of strength $O(\mu\Omega a^9/R^6)$, whose velocity at sphere 2 is $O(\Omega a^9/R^8)$. This [method of reflections for Stokes flow](../../../stokes-flow.md#method-of-reflections-for-stokes-flow) gives the stated order of the next correction to $\mathbf U_2$.

## 2

↑ **Parent:** [Paper 329](paper-329.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Write the perturbation as $\eta e^{ikx+st}$ and use the same factor for all velocity and pressure amplitudes. At the upper interface, the linearized [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition), zero tangential traction, and normal-stress balance are

$$
v=s\eta,
\qquad
u_y+v_x=0,
\qquad
-p+2\mu v_y
=\left(\frac{3V}{h_0^4}-\gamma k^2\right)\eta
\quad(y=h_0).
$$

The first term in the normal stress is the linearization of the attractive [disjoining pressure](../../../viscous-fluid-flow.md#disjoining-pressure) $V/h^3$, while the second is the stabilizing [capillary pressure](../../../fluid-mechanics.md#capillary-pressure). Symmetry about $y=0$ makes $u$ even and $v$ odd, and supplies the lower-interface conditions.

For a two-dimensional Fourier mode, the [Papkovich–Neuber representation](../../../stokes-flow.md#papkovich-neuber-representation) is equivalently expressed by the odd [biharmonic stream function for planar Stokes flow](../../../stokes-flow.md#biharmonic-stream-function-for-planar-stokes-flow)

$$
\psi(y)=A\sinh(ky)+By\cosh(ky),
\qquad
u=\psi_y,
\qquad
v=-ik\psi.
$$

The tangential-stress condition at $y=h_0$, with $K=kh_0$, gives

$$
Ak\sinh K+B(\sinh K+K\cosh K)=0,
$$

whereas the kinematic condition gives $iB\sinh K=s\eta$. The associated normal traction is

$$
-p+2\mu v_y
=\mu k s\eta\frac{2K+\sinh2K}{\sinh^2K}.
$$

Equating this with the linearized interfacial traction yields the [dispersion relation](../../../wave-equation.md#dispersion-relation)

$$
\boxed{
s=\frac{3V}{\mu h_0^3}
\frac{(1-\Gamma K^2)\sinh^2K}
{K(2K+\sinh2K)},
\qquad
\Gamma=\frac{\gamma h_0^2}{3V}.}
$$

This is the [Van der Waals rupture instability of a viscous sheet](../../../viscous-fluid-flow.md#van-der-waals-rupture-instability-of-a-viscous-sheet).

For $\Gamma=0$, the growth rate is positive, starts from $3V/(4\mu h_0^3)$ as $K\to0$, and decreases to zero like $3V/(2\mu h_0^3K)$ as $K\to\infty$. For $\Gamma=1$, it has the same long-wave limit, vanishes at $K=1$, and is negative for $K>1$: [surface tension](../../../fluid-mechanics.md#surface-tension) damps wavelengths shorter than the cutoff. Long waves feel the attractive interaction but require coherent flow over a large distance; at short wavelengths viscous resistance suppresses the clean-film instability, while capillarity adds direct decay. A finite film size, [fluid inertia](../../../viscous-fluid-flow.md#navier-stokes-equation), surrounding-fluid stresses, gravity, surface viscosity, and failure of the continuum [disjoining pressure](../../../viscous-fluid-flow.md#disjoining-pressure) law can shift the observable most unstable wavelength.

During a growing thin spot, interfacial flow stretches the surface and dilutes its [surfactant](../../../fluid-mechanics.md#surfactant), thereby increasing the local surface tension above $\gamma_0$. Adjacent less-stretched regions retain more surfactant and lower tension. The resulting [surface-tension gradient](../../../fluid-mechanics.md#marangoni-effect) pulls toward the thin spot and opposes the outward flow that drives thinning. This is [surfactant stabilization of film rupture](../../../fluid-mechanics.md#surfactant-stabilization-of-film-rupture); in the strong limit the surfaces behave almost as immobile boundaries.

For strong surfactant and $\Gamma\gg1$, instability requires $K=O(\Gamma^{-1/2})$. The [Taylor expansion](../../../calculus.md#taylor-expansion)

$$
\frac{\sinh2K-2K}{4K\cosh^2K}
=\frac{K^2}{3}+O(K^4)
$$

reduces the supplied relation to

$$
s\sim\frac{V}{\mu h_0^3}K^2(1-\Gamma K^2).
$$

It is maximal at

$$
\boxed{K_{\max}^2=\frac1{2\Gamma},
\qquad
s_{\max}=\frac{V}{4\mu h_0^3\Gamma}
=\frac{3V^2}{4\mu\gamma_0h_0^5}.}
$$

Thus the characteristic rupture time is $s_{\max}^{-1}=4\mu\gamma_0h_0^5/(3V^2)$. Surfactant greatly extends the life of a soap bubble while its film is moderately thick, but the $h_0^{-5}$ growth-rate dependence predicts rapid final rupture after drainage has made the film sufficiently thin.

## 3

↑ **Parent:** [Paper 329](paper-329.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Reflect the configuration in a plane perpendicular to the tube axis. The geometry and radial displacement are unchanged, whereas the imposed pressure gradient and every axial velocity reverse. By [kinematic reversibility of Stokes flow](../../../stokes-flow.md#kinematic-reversibility-of-stokes-flow), a radial migration velocity would also have to reverse; the spatial reflection leaves that component unchanged. [Uniqueness of Stokes flow](../../../stokes-flow.md#uniqueness-of-stokes-flow) therefore forces it to vanish. Reflection in the meridional plane through the two axes similarly excludes azimuthal drift, so $c$ remains constant.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Apply axial momentum balance to the fluid between the remote sections $x_1$ and $x_2$. The pressure forces on the end discs, the integrated tube-wall shear, and the force exerted by the sphere are the only resultant axial forces. The sphere is [force-free](../../../stokes-flow.md#force-free), so its contribution vanishes and

$$
\boxed{
a\int_{x_1}^{x_2}\int_0^{2\pi}
\sigma_{rx}(a,\theta,x)\,d\theta\,dx
=\pi a^2[p(x_2)-p(x_1)].}
$$

This is the [wall-shear and pressure-drop balance in a tube](../../../viscous-fluid-flow.md#wall-shear-and-pressure-drop-balance-in-a-tube).

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [nearly occluding sphere in a cylindrical tube](../../../viscous-fluid-flow.md#nearly-occluding-sphere-in-a-cylindrical-tube) has gap thickness $H=O(\epsilon a)$ and axial length $L=O(\sqrt{aH})=O(a\sqrt\epsilon)$. In the gap, [lubrication theory](../../../viscous-fluid-flow.md#lubrication-theory) therefore gives

$$
p_x=O\left(\frac{\mu U}{\epsilon^2a^2}\right),
\qquad
p=O\left(\frac{\mu U}{a\epsilon^{3/2}}\right),
\qquad
\sigma_{xy}=O\left(\frac{\mu U}{\epsilon a}\right).
$$

Far ahead of and behind the sphere, the length and width scales are both $a$, so

$$
p_x=O\left(\frac{\mu U}{a^2}\right),
\qquad
\sigma_{rx}=O\left(\frac{\mu U}{a}\right).
$$

In the sphere frame the tube wall at $y=0$ moves with velocity $-U$ and the sphere surface at $y=h$ is stationary. The local [Couette-Poiseuille flow in a thin gap](../../../viscous-fluid-flow.md#couette-poiseuille-flow-in-a-thin-gap) is

$$
u=-U+\frac Uh y+\frac{p_x}{2\mu}y(y-h).
$$

Its axial [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate) per unit circumferential width is

$$
\boxed{q=-\frac{h^3}{12\mu}p_x-\frac{Uh}{2}.}
$$

Differentiating the profile and eliminating $p_x$ gives the two wall stresses

$$
\boxed{
\left.\frac{\sigma_{xy}}\mu\right|_{y=0}
=\frac{4U}{h}+\frac{6q}{h^2},
\qquad
\left.\frac{\sigma_{xy}}\mu\right|_{y=h}
=-\frac{2U}{h}-\frac{6q}{h^2}.}
$$

The [continuity equation](../../../physics.md#continuity-equation) integrated across the gap says that changes of $q$ along $x$ are balanced by circumferential flux divergence. Circumferential variations occur on scale $a$, much longer than the axial scale $a\sqrt\epsilon$, so $q=q(\theta)$ is independent of $x$ at leading order.

Put $h=h_0(1+\xi^2)$ with $x=\sqrt{2ah_0}\,\xi$. The leading $O(\epsilon^{-3/2})$ pressure jump must vanish in the global balance from part ii. Equivalently, the [pressure recovery condition in lubrication flow](../../../viscous-fluid-flow.md#pressure-recovery-condition-in-lubrication-flow) gives

$$
0=\int_{-\infty}^{\infty}p_x\,dx
=-12\mu q\int h^{-3}\,dx-6\mu U\int h^{-2}\,dx.
$$

Using $I_2=\pi/2$ and $I_3=3\pi/8$,

$$
\frac{\int h^{-2}dx}{\int h^{-3}dx}=\frac43h_0,
\qquad
\boxed{q=-\frac23Uh_0(\theta).}
$$

The total flux through the gap is consequently

$$
Q=a\int_0^{2\pi}q\,d\theta
=-\frac43\pi\epsilon Ua^2.
$$

Far from the sphere, translation of the tube contributes $-\pi a^2U$, while [Hagen-Poiseuille flow](../../../viscous-fluid-flow.md#hagen-poiseuille-equation) contributes $\pi a^4p_x/(8\mu)$. Equating these fluxes gives

$$
\boxed{p_x\sim\frac{8\mu U}{a^2}\left(1-\frac43\epsilon\right).}
$$

At the next order, substitute $q=-2Uh_0/3$ into the tube-wall shear and integrate through the gap:

$$
\int_{-\infty}^{\infty}\sigma_{xy}(x,0)\,dx
=4\mu U\int\left(\frac1h-\frac{h_0}{h^2}\right)dx
=2\pi\mu U\sqrt{\frac{2a}{h_0}}.
$$

The balance in part ii then gives the leading pressure drop

$$
\boxed{
\Delta p
=\sqrt{\frac2\epsilon}\frac{2\mu U}{a}
\int_0^{2\pi}\frac{d\theta}{\sqrt{1+\lambda\cos\theta}}.}
$$

Finally, the shear on the sphere integrates to

$$
\int_{-\infty}^{\infty}\sigma_{xy}(x,h)\,dx
=\mu U\int\left(-\frac2h+\frac{4h_0}{h^2}\right)dx=0,
$$

because $I_1=\pi$ and $I_2=\pi/2$. Thus the narrow gap exerts no net leading axial shear force on the sphere even though its local shear is nonzero; the leading hydrodynamic force transfer to the sphere is through the large lubrication pressure acting on its gently sloping surface.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
