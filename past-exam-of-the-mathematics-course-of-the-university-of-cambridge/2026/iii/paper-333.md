# Paper 333

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20333.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20333.pdf)

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
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
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

↑ **Parent:** [Paper 333](paper-333.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The horizontal velocities $u$ and $v$ point east and north, $\eta$ is the displacement of the free surface from its mean level, $H_0$ is the undisturbed depth, $g$ is gravitational acceleration, and $f$ is the constant [Coriolis parameter](../../../geophysical-fluid-dynamics.md#coriolis-parameter) on an [f-plane](../../../geophysical-fluid-dynamics.md#f-plane). The three [linearized shallow water equations](../../../physics.md#linearized-shallow-water-equations) are horizontal momentum balance and [mass conservation](../../../continuum-mechanics.md#mass-conservation):

$$
u_t-fv=-g\eta_x,\qquad
v_t+fu=-g\eta_y,\qquad
\eta_t+H_0(u_x+v_y)=0.
$$

They follow from the rotating [Navier-Stokes equation](../../../viscous-fluid-flow.md#navier-stokes-equation) by assuming an inviscid homogeneous layer, [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure), horizontal scales much larger than $H_0$, depth-independent horizontal velocity, a flat impermeable bottom, constant $f$, and small surface displacement and velocity so that nonlinear products are neglected.

In a steady state, [geostrophic balance](../../../physics.md#geostrophic-balance) gives

$$
\boxed{u_g=-\frac gf\eta_y},
\qquad
\boxed{v_g=\frac gf\eta_x}.
$$

The relative vorticity is $\zeta=v_x-u_y$. Expanding the [shallow-water potential vorticity](../../../geophysical-fluid-dynamics.md#shallow-water-potential-vorticity) $(f+\zeta)/(H_0+\eta)$ to first order gives

$$
\frac f{H_0}+\frac1{H_0}
\left(\zeta-\frac f{H_0}\eta\right).
$$

Thus one convenient normalization of its disturbance is

$$
\boxed{q=\zeta-\frac f{H_0}\eta}.
$$

Taking the curl of momentum and using continuity shows $q_t=0$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Initially $\zeta=0$, so conservation of the linear [potential vorticity](../../../geophysical-fluid-dynamics.md#potential-vorticity) gives

$$
\zeta_f-\frac f{H_0}\eta_f
=-\frac f{H_0}\eta_i.
$$

The final flow is in [geostrophic balance](../../../physics.md#geostrophic-balance), hence

$$
\zeta_f=\frac gf\nabla^2\eta_f.
$$

Consequently the adjusted height solves the modified Helmholtz equation

$$
\boxed{
\left(\nabla^2-\frac1{L_R^2}\right)\eta_f
=-\frac{\eta_i}{L_R^2}},
\qquad
\boxed{L_R=\frac{\sqrt{gH_0}}{|f|}},
$$

where $L_R$ is the [Rossby deformation radius](../../../physics.md#rossby-deformation-radius).

The initial condition is independent of $x$ and odd in $y$. The bounded solution that is continuously differentiable at $y=0$ is

$$
\boxed{
\eta_f(y)=\eta_0\operatorname{sgn}(y)
\left(1-e^{-|y|/L_R}\right)}.
$$

It gives

$$
\boxed{
u_f(y)=-\frac{g\eta_0}{fL_R}e^{-|y|/L_R}},
\qquad
\boxed{v_f=0}.
$$

During [geostrophic adjustment](../../../geophysical-fluid-dynamics.md#geostrophic-adjustment), the part of the initial energy incompatible with the conserved potential-vorticity distribution radiates away as [inertia-gravity waves](../../../geophysical-fluid-dynamics.md#inertia-gravity-wave). The remaining current has width $O(L_R)$ and is geostrophically balanced.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Set $c=\sqrt{gH_0}$ and seek

$$
\eta=G(x)F(y+\gamma t),\qquad u=0.
$$

The two remaining prognostic equations imply

$$
v=-\frac g\gamma\eta,\qquad
\gamma^2=gH_0=c^2.
$$

The $x$ momentum equation is now geostrophic:

$$
fv=g\eta_x.
$$

Therefore

$$
\frac{G'}G=-\frac f\gamma.
$$

Boundedness for $x>0$ selects $\gamma=\operatorname{sgn}(f)c$ and

$$
\boxed{
G(x)=G(0)e^{-x/L_R}},
\qquad
\boxed{\gamma=\operatorname{sgn}(f)\sqrt{gH_0}}.
$$

Because $F$ depends on $y+\gamma t$, the wave travels with meridional phase speed $-\gamma$. Along this western boundary it travels southward in the Northern Hemisphere and northward in the Southern Hemisphere, keeping the coast on the dynamically required side. This is a coastal [Kelvin wave](../../../geophysical-fluid-dynamics.md#kelvin-wave).

Moreover,

$$
v=-\frac{\gamma}{H_0}\eta,\qquad
v_x=\frac f{H_0}\eta.
$$

Since $u=0$, its linear potential-vorticity disturbance is

$$
\boxed{q=v_x-u_y-\frac f{H_0}\eta=0}.
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Potential-vorticity conservation still determines the final surface through

$$
\left(\nabla^2-L_R^{-2}\right)\eta_f
=-L_R^{-2}\eta_0\operatorname{sgn}(y),
\qquad x>0.
$$

The unbounded problem only required decay or matching as $|y|$ and $x$ become large. The coast adds a boundary condition. In the adjusted geostrophic flow,

$$
u(0,y)=-\frac gf\eta_y(0,y)=0,
$$

so $\eta$ must be constant along the connected wall. Odd symmetry and the arbitrary common height datum set that constant to zero:

$$
\boxed{\eta_f(0,y)=0}.
$$

This is a Dirichlet condition on $\eta$, even though it originated as no normal flow.

The initial disturbance does not instantaneously know this along the whole coast. A southward coastal [Kelvin wave](../../../geophysical-fluid-dynamics.md#kelvin-wave) for $f>0$ carries the pressure signal and establishes the constant wall height behind its wavefront. In the final streamline sketch, the [quasi-geostrophic streamfunction](../../../geophysical-fluid-dynamics.md#quasi-geostrophic-streamfunction) is proportional to $\eta_f$. Far from the wall the contours and current resemble the unbounded east--west front; near $x=0$ those contours bend through a right angle and run along the coast, so the incident geostrophic current turns into a southward boundary current instead of crossing the wall.

## 2

↑ **Parent:** [Paper 333](paper-333.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Assume a steady, small-Rossby-number interior in which drag is negligible and the nonlinear advection of relative vorticity,

$$
J(\psi,\nabla^2\psi),
$$

is small compared with advection of planetary vorticity. The stretching term proportional to $\psi$ has zero Jacobian with $\psi$. On the [beta plane](../../../geophysical-fluid-dynamics.md#beta-plane),

$$
J\left(\psi,\frac f{f_0}\right)
=J\left(\psi,\frac{\beta y}{f_0}\right)
=\frac{\beta}{f_0}\psi_x.
$$

Hence the forced quasi-geostrophic equation reduces to [Sverdrup balance](../../../geophysical-fluid-dynamics.md#sverdrup-balance)

$$
\boxed{
\frac{\beta}{f_0}\psi_x
=\frac1{\rho H_0^2}
(\nabla\times\boldsymbol\tau)\mathbin{\cdot}\hat{\mathbf z}}.
$$

For the zonal [wind stress](../../../geophysical-fluid-dynamics.md#wind-stress) $\boldsymbol\tau=\tau(y)\hat{\mathbf x}$,

$$
(\nabla\times\boldsymbol\tau)\mathbin{\cdot}\hat{\mathbf z}
=-\tau'(y),
$$

so

$$
\boxed{
\psi_x=-\frac{f_0}{\beta\rho H_0^2}\tau'(y)}.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The eastern wall has no normal flow, so the [quasi-geostrophic streamfunction](../../../geophysical-fluid-dynamics.md#quasi-geostrophic-streamfunction) is constant there. Choose $\psi(L,y)=0$. Integrating the Sverdrup relation gives

$$
\boxed{
\psi_{\rm int}(x,y)
=\frac{f_0\tau'(y)}{\beta\rho H_0^2}(L-x)}.
$$

Since [geostrophic balance](../../../physics.md#geostrophic-balance) gives $\psi=g\eta/f_0$,

$$
\boxed{
\eta_{\rm int}(x,y)
=\frac{f_0^2\tau'(y)}
{g\beta\rho H_0^2}(L-x)}.
$$

If this interior solution were extended to both walls, the west-minus-east height difference would be

$$
\boxed{
\eta_{\rm int}(0,y)-\eta_{\rm int}(L,y)
=\frac{f_0^2L}{g\beta\rho H_0^2}\tau'(y)}.
$$

The northward volume transport per unit meridional distance is

$$
T=H_0\int_0^L v\,dx
=H_0\int_0^L\psi_x\,dx
=\frac{gH_0}{f_0}\,[\eta(L,y)-\eta(0,y)].
$$

Thus

$$
\boxed{
T=-\frac{f_0L}{\beta\rho H_0}\tau'(y)}.
$$

This is the basin-integrated form of [Sverdrup balance](../../../geophysical-fluid-dynamics.md#sverdrup-balance).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

In a narrow western layer, $x$ derivatives dominate $y$ derivatives. Subtracting the forced interior balance leaves

$$
\frac{\beta}{f_0}\psi_{{\rm bl},x}
\simeq-\gamma\psi_{{\rm bl},xx}.
$$

If the layer has width $\delta$, then $\psi_x=O(\psi/\delta)$ and $\psi_{xx}=O(\psi/\delta^2)$. Balancing the beta effect with linear bottom drag gives

$$
\frac{\beta}{f_0\delta}
\sim\frac{\gamma}{\delta^2},
$$

and therefore the [Stommel boundary layer](../../../geophysical-fluid-dynamics.md#stommel-boundary-layer) width is

$$
\boxed{\delta=\frac{\gamma f_0}{\beta}}.
$$

This scaling assumes $\delta\ll L$ and that along-boundary variations occur on the basin scale.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

No normal flow makes $\psi$ constant on the connected basin boundary; set that constant to zero. Put

$$
A(y)=\frac{f_0\tau'(y)}{\beta\rho H_0^2}.
$$

The interior solution is $A(L-x)$. The decaying boundary correction that enforces $\psi(0,y)=0$ is

$$
\psi_{\rm bl}=-ALe^{-x/\delta}.
$$

Thus, to leading order in $\delta/L$,

$$
\boxed{
\psi=A\left(L-x-Le^{-x/\delta}\right)},
\qquad
\boxed{
\eta=\frac{f_0A}{g}
\left(L-x-Le^{-x/\delta}\right)}.
$$

If $\delta$ denotes the e-folding width literally, then

$$
\boxed{
\Delta\eta_{\rm WBC}
=\eta(\delta,y)-\eta(0,y)
=\frac{f_0A}{g}
\left[L(1-e^{-1})-\delta\right]}.
$$

Since a boundary-layer width is only defined up to an order-one factor, matching at any point satisfying $\delta\ll x\ll L$ gives the convention-independent leading jump

$$
\boxed{
\Delta\eta_{\rm WBC}
\sim\frac{f_0^2L}{g\beta\rho H_0^2}\tau'(y)}.
$$

It is the height difference needed to return the broad Sverdrup transport in a narrow [western boundary current](../../../geophysical-fluid-dynamics.md#western-boundary-current).

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Because $v=\psi_x=(g/f_0)\eta_x$, the mean boundary-current velocity is exactly related to the height change by

$$
\boxed{
\bar v=\frac1\delta\int_0^\delta v\,dx
=\frac g{f_0\delta}\Delta\eta_{\rm WBC}}.
$$

For the e-folding convention used in part d,

$$
\bar v
=A\left[\frac L\delta(1-e^{-1})-1\right].
$$

Its robust narrow-layer scaling is

$$
\boxed{
\bar v\sim
\frac{L\,\tau'(y)}{\rho H_0^2\gamma}}.
$$

Thus weaker drag makes the current proportionally narrower and faster. Their product is independent of $\gamma$ to leading order:

$$
H_0\delta\bar v
\sim\frac{f_0L}{\beta\rho H_0}\tau'(y)
=-T_{\rm int}.
$$

[Mass conservation](../../../continuum-mechanics.md#mass-conservation) requires the narrow return transport to cancel the broad [Sverdrup balance](../../../geophysical-fluid-dynamics.md#sverdrup-balance) transport. The meridional gradient of planetary [potential vorticity](../../../geophysical-fluid-dynamics.md#potential-vorticity) makes a frictional closure possible on the western side and produces western intensification; bottom drag supplies the vorticity sink that permits fluid parcels to cross potential-vorticity contours there.

## 3

↑ **Parent:** [Paper 333](paper-333.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

In linear [quasi-geostrophic approximation](../../../geophysical-fluid-dynamics.md#quasi-geostrophic-approximation), buoyancy and vertical velocity satisfy

$$
f_0\psi'_{zt}+N^2w'=0.
$$

Impermeability means $w'=0$ at $z=-H$ and $z=0$. For a normal mode with nonzero frequency this is equivalent to the Neumann conditions

$$
\boxed{
\hat\psi'(-H)=0,\qquad
\hat\psi'(0)=0},
$$

where the primes on $\hat\psi$ denote derivatives with respect to $z$. Equivalently, $\psi'_z=0$ at both rigid boundaries.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

Linearizing conservation of [three-dimensional quasi-geostrophic potential vorticity](../../../geophysical-fluid-dynamics.md#three-dimensional-quasi-geostrophic-potential-vorticity) about rest gives

$$
q'_t+\beta\psi'_x=0.
$$

For $K^2=k^2+l^2$, the plane-wave ansatz yields

$$
-\omega\left[
-K^2\hat\psi+\frac{f_0^2}{N^2}\hat\psi''
\right]+\beta k\hat\psi=0.
$$

Thus the vertical structure equation is

$$
\boxed{
\hat\psi''
-\frac{N^2}{f_0^2}
\left(K^2+\frac{\beta k}{\omega}\right)\hat\psi=0}.
$$

The rigid-boundary eigenfunctions are

$$
\hat\psi_n(z)=\cos\frac{n\pi z}{H},
\qquad n=0,1,2,\ldots.
$$

Substitution gives the [Baroclinic Rossby wave](../../../geophysical-fluid-dynamics.md#baroclinic-rossby-wave) dispersion relations

$$
\boxed{
\omega_n(k,l)=
-\frac{\beta k}
{k^2+l^2+
\dfrac{f_0^2}{N^2}\left(\dfrac{n\pi}{H}\right)^2}}.
$$

The $n=0$ member is the [Barotropic Rossby wave](../../../geophysical-fluid-dynamics.md#barotropic-rossby-wave); $n\geq1$ are baroclinic vertical modes.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

At the free surface, the linear [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition) is

$$
w'(0)=\eta_t.
$$

Hydrostatic pressure and geostrophic-streamfunction normalization give

$$
p'(0)=\rho_0f_0\psi'(0)=\rho_0g\eta,
\qquad
\eta=\frac{f_0}{g}\psi'(0).
$$

Combining this with

$$
f_0\psi'_{zt}+N^2w'=0
$$

gives

$$
\frac{\partial}{\partial t}
\left(\psi'_z+\frac{N^2}{g}\psi'\right)=0
\qquad(z=0).
$$

For an oscillatory disturbance with no time-independent boundary offset, the free-surface boundary condition is therefore

$$
\boxed{
\psi'_z+\frac{N^2}{g}\psi'=0
\qquad(z=0)}.
$$

The lower rigid boundary retains $\psi'_z(-H)=0$.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

For

$$
\psi'=A(x,y,t)\cos\frac{n\pi z}{H},
$$

the surface value is simply $\psi'(0)=A$. The dynamic free-surface condition from part i gives

$$
\boxed{
\eta(x,y,t)=\frac{f_0}{g}A(x,y,t)}.
$$

The cosine is the leading small-surface-displacement approximation to the exact [quasi-geostrophic vertical mode](../../../geophysical-fluid-dynamics.md#quasi-geostrophic-vertical-mode); its derivative vanishes at both rigid-boundary locations.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

The [isopycnal displacement](../../../geophysical-fluid-dynamics.md#isopycnal-displacement) is

$$
\xi=-\frac{f_0}{N^2}\psi'_z.
$$

For the $n$th cosine mode,

$$
\xi=
\frac{f_0A}{N^2}\frac{n\pi}{H}
\sin\frac{n\pi z}{H}.
$$

Its maximum magnitude is therefore

$$
\boxed{
|\xi|_{\max}
=\frac{f_0|A|}{N^2}\frac{n\pi}{H}
=\frac{gn\pi}{N^2H}|\eta|_{\max}}.
$$

For $H=3000\ {\rm m}$, $N=10^{-3}\ {\rm s}^{-1}$, and $|\eta|_{\max}=10^{-2}\ {\rm m}$,

$$
|\xi|_{\max}
\simeq
\frac{9.81\,n\pi}{(10^{-3})^2(3000)}
(10^{-2}\ {\rm m})
\simeq103n\ {\rm m}.
$$

The first baroclinic mode therefore displaces interior density surfaces by about $10^2\ {\rm m}$ even though the surface moves only one centimetre.

## 4

↑ **Parent:** [Paper 333](paper-333.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The variables $u,v,w$ are eastward, northward, and upward velocity, $\phi=p'/\rho_0$ is the pressure perturbation divided by reference density, $\sigma$ is buoyancy, $N$ is the constant [buoyancy frequency](../../../gravity-wave.md#buoyancy-frequency), and $\beta y$ is the equatorial approximation to the [Coriolis parameter](../../../geophysical-fluid-dynamics.md#coriolis-parameter). The equations express, respectively:

- zonal momentum balance between acceleration, Coriolis force, and pressure gradient;
- meridional [geostrophic balance](../../../physics.md#geostrophic-balance), with meridional acceleration omitted by the long-wave approximation;
- incompressible [mass conservation](../../../continuum-mechanics.md#mass-conservation);
- adiabatic buoyancy evolution in the background stratification;
- [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure) balance, $\phi_z=\sigma$.

Together they are the hydrostatic [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation) for long [equatorial waves](../../../geophysical-fluid-dynamics.md#equatorial-wave).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Put $v=0$ and use amplitudes proportional to $e^{i(kx+mz-\omega t)}$. Zonal momentum gives

$$
\hat u=\frac{k}{\omega}\hat\phi,
$$

while incompressibility, buoyancy evolution, and hydrostatic balance give

$$
\hat w=-\frac{k}{m}\hat u
=-\frac{\omega m}{N^2}\hat\phi.
$$

Hence

$$
\omega^2=\frac{N^2k^2}{m^2}.
$$

Meridional geostrophic balance requires

$$
\frac{d\hat\phi}{dy}
=-\frac{\beta k}{\omega}y\hat\phi,
$$

so

$$
\boxed{
\hat\phi(y)=\Phi_0
\exp\left(-\frac{\beta k}{2\omega}y^2\right)}.
$$

Decay as $|y|\to\infty$, together with $\beta>0$ and $k>0$, requires $\omega>0$. Therefore

$$
\boxed{\omega=\frac{Nk}{|m|}},
\qquad
\boxed{
\hat\phi(y)=\Phi_0
\exp\left(-\frac{\beta|m|}{2N}y^2\right)}.
$$

The negative-frequency root makes the Gaussian exponent positive and the solution diverge away from the equator. The acceptable branch is the eastward [equatorial Kelvin wave](../../../geophysical-fluid-dynamics.md#equatorial-kelvin-wave).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Let

$$
c=\frac N{|m|},
\qquad
D=\frac{\omega^2}{c^2}-k^2.
$$

Solving zonal momentum and incompressibility for $\hat u$ and $\hat\phi$ in terms of $\hat v$ gives

$$
\boxed{
\hat u
=\frac{i}{D}
\left(\frac{\beta y\omega}{c^2}\hat v
-k\hat v_y\right)},
$$



$$
\boxed{
\hat\phi
=\frac{i}{D}
\left(k\beta y\hat v-\omega\hat v_y\right)}.
$$

Substitution into meridional geostrophic balance cancels the terms involving $D$ and yields

$$
\boxed{
\hat v_{yy}-\frac{\beta^2y^2m^2}{N^2}\hat v
=\frac{k\beta}{\omega}\hat v}.
$$

Set

$$
\xi=\sqrt{\frac{\beta|m|}{N}}\,y.
$$

The equation becomes

$$
\hat v_{\xi\xi}-\xi^2\hat v
=\frac{kN}{\omega|m|}\hat v.
$$

Using the [Hermite polynomial](../../../numerical-analysis.md#hermite-polynomial) eigenvalues gives

$$
\boxed{
\omega_n=-\frac{Nk}{(2n+1)|m|}},
\qquad n=1,2,\ldots,
$$

and

$$
\boxed{
\hat v_n(y)=V_n
H_n(\xi)e^{-\xi^2/2}}.
$$

The associated pressure amplitude is

$$
\boxed{
\hat\phi_n
=\frac{i(k\beta y\hat v_n-\omega_n\hat v_{n,y})}
{\omega_n^2m^2/N^2-k^2}}.
$$

For $n=0$, the denominator used to solve for $\hat u$ and $\hat\phi$ vanishes because $\omega_0^2m^2/N^2=k^2$. The inversion therefore assumed precisely the condition that excludes that degenerate case; it must be analyzed separately and is not a member of this [equatorial Rossby wave](../../../geophysical-fluid-dynamics.md#equatorial-rossby-wave) family.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Every forced propagating mode must have the imposed zonal frequency

$$
\omega=kC.
$$

For $C>0$, only the [equatorial Kelvin wave](../../../geophysical-fluid-dynamics.md#equatorial-kelvin-wave) has the correct sign. Upward group velocity in the fluid $z>0$ selects

$$
m_K=-\frac NC.
$$

With $K(y)=\exp[-\beta y^2/(2C)]$, its pressure field can be written

$$
\boxed{
\phi_K=\operatorname{Re}
\left\{
a_KK(y)e^{i[k(x-Ct)+m_Kz]}
\right\}}.
$$

Here $v_K=0$, $u_K=\phi_K/C$, and the complex vertical-velocity amplitude is

$$
\hat w_K=-\frac{kCm_K}{N^2}a_KK
=\frac kN a_KK.
$$

The lower boundary is matched only if

$$
\boxed{
W(y)=\frac kN a_K
\exp\left(-\frac{\beta y^2}{2C}\right)}
$$

after choosing the phase of $a_K$ to make the prescribed cosine amplitude real.

For $C<0$, the upward-radiating [equatorial Rossby waves](../../../geophysical-fluid-dynamics.md#equatorial-rossby-wave) have

$$
\boxed{
m_n=-\frac{N}{(2n+1)C}>0},
\qquad n=1,2,\ldots.
$$

Choose each pair $(\hat v_n,\hat\phi_n)$ as in part c for this $m_n$. The propagating sum is

$$
\boxed{
v=\operatorname{Re}
\sum_{n=1}^{\infty}
a_n\hat v_n(y)
e^{i[k(x-Ct)+m_nz]}},
$$



$$
\boxed{
\phi=\operatorname{Re}
\sum_{n=1}^{\infty}
a_n\hat\phi_n(y)
e^{i[k(x-Ct)+m_nz]}}.
$$

The other fields follow mode by mode from part c and $\hat w_n=-kCm_n\hat\phi_n/N^2$. Thus the boundary matching condition is

$$
\boxed{
W(y)=
\sum_{n=1}^{\infty}
\frac{k\,a_n}{N(2n+1)}
\hat\phi_n(y)}.
$$

For $C>0$, the space of upward-radiating wave profiles is only the one-dimensional Gaussian Kelvin profile, so a generic $W(y)$ cannot be matched by propagating waves. Its Kelvin projection radiates upward; the remaining forcing produces a balanced, vertically evanescent response trapped near the lower boundary. This is the equatorial analogue of the fact that quasi-geostrophic [Rossby waves](../../../geophysical-fluid-dynamics.md#rossby-wave) have westward rather than eastward phase propagation.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
