# Paper 333

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_333.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_333.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
  - [v](#1/v)
    - [Solution](#1/v/solution)
  - [vi](#1/vi)
    - [Solution](#1/vi/solution)
  - [vii](#1/vii)
    - [Solution](#1/vii/solution)
  - [viii](#1/viii)
    - [Solution](#1/viii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)

## 1

↑ **Parent:** [Paper 333](paper-333.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

The first two equations are horizontal momentum balances: local acceleration plus the [Coriolis acceleration](../../../physics.md#coriolis-acceleration) equals the pressure-gradient force. The third is linearized [mass conservation](../../../continuum-mechanics.md#mass-conservation): convergence raises the free surface, represented by $\phi$, while divergence lowers it. The constant $c$ is the long-wave gravity-wave speed.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

Differentiate the second momentum equation in $x$, the first in $y$, subtract, and use continuity:

$$
(v_x-u_y)_t=-f(u_x+v_y)=\frac f{c^2}\phi_t.
$$

Hence the linear [shallow-water potential vorticity](../../../geophysical-fluid-dynamics.md#shallow-water-potential-vorticity)

$$
\boxed{P=v_x-u_y-\frac f{c^2}\phi}
$$

satisfies $P_t=0$.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Substitution of $e^{i(kx+ly-\omega t)}$ gives a homogeneous three-by-three system. Its determinant is

$$
\boxed{\omega[\omega^2-f^2-c^2(k^2+l^2)]=0,}
$$

so

$$
\boxed{\omega=0,\qquad \omega=\pm\Omega,qquad
\Omega=(f^2+c^2K^2)^{1/2},\quad K=(k^2+l^2)^{1/2}.}
$$

The zero-frequency component is in [geostrophic balance](../../../physics.md#geostrophic-balance) and carries all conserved $P$. The oscillatory components are [inertia-gravity waves](../../../geophysical-fluid-dynamics.md#inertia-gravity-wave) with zero $P$. For $K\ll|f|/c$, $\Omega\sim|f|$ and rotation produces an [inertial oscillation](../../../geophysical-fluid-dynamics.md#inertial-oscillation); for $K\gg|f|/c$, $\Omega\sim cK$ and surface gravity dominates. The crossover length $c/|f|$ is the [barotropic deformation radius](../../../geophysical-fluid-dynamics.md#barotropic-deformation-radius).

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

Initially $P=-f\phi_0\operatorname{sgn}(x)/c^2$. In the final steady state,

$$
u=-\frac1f\Phi_y,
\qquad v=\frac1f\Phi_x.
$$

Equating its potential vorticity to the initial value gives

$$
\boxed{\Phi_{xx}+\Phi_{yy}-\frac{f^2}{c^2}\Phi
=-\frac{f^2}{c^2}\phi_0\operatorname{sgn}(x).}
$$

This is [geostrophic adjustment](../../../geophysical-fluid-dynamics.md#geostrophic-adjustment): inertia-gravity waves remove the unbalanced part. Their group speed is at most $c$, so at any finite time only a region whose distance from the initial jump is $O(ct)$ can have reached the steady state.

<h3 id="1/v">v</h3>

↑ **Parent:** [1](#1)

<h4 id="1/v/solution">Solution</h4>

↑ **Parent:** [V](#1/v)

No normal flow at $y=0,L$ requires $v=0$. Geostrophic balance therefore gives $\Phi_x=0$ on both walls. These conditions do not fix the $x$-independent nullspace: if

$$
\boxed{\Psi''-\frac{f^2}{c^2}\Psi=0,}
$$

then $\Phi+\Psi(y)$ satisfies both the adjusted equation and $\Phi_x=0$. Thus $\Psi=Ae^{fy/c}+Be^{-fy/c}$ supplies two undetermined amplitudes.

<h3 id="1/vi">vi</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#1/vi)

Set $v=0$. For $F_+(x+ct)$ the equations require $\widetilde\phi_+=-c\widetilde u_+$ and $\widetilde u_+'=(f/c)\widetilde u_+$; for $F_-(x-ct)$ they require $\widetilde\phi_-=c\widetilde u_-$ and $\widetilde u_-'=-(f/c)\widetilde u_-$. Hence the channel supports the [Kelvin waves](../../../geophysical-fluid-dynamics.md#kelvin-wave)

$$
\boxed{
\widetilde u_\pm=C_\pm e^{\pm fy/c},
\qquad
\widetilde\phi_\pm=\mp c\widetilde u_\pm.}
$$

Each wave propagates along one wall and is exponentially trapped toward that wall on the deformation scale $c/|f|$.

<h3 id="1/vii">vii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/vii/solution">Solution</h4>

↑ **Parent:** [Vii](#1/vii)

Form the $x$-momentum equation plus $1/c$ times continuity, multiply by $e^{\mp fy/c}$, and integrate across the channel. Integration by parts makes the $v_y$ term cancel the Coriolis term, and $v=0$ removes the endpoint contribution. The result is the pair of [Kelvin-wave channel invariants](../../../geophysical-fluid-dynamics.md#kelvin-wave-channel-invariant)

$$
\boxed{
\left(\frac\partial{\partial t}\pm\frac1c\frac\partial{\partial x}\right)
\int_0^Le^{\mp fy/c}\left(u+\frac\phi c\right)dy=0.}
$$

<h3 id="1/viii">viii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/viii/solution">Solution</h4>

↑ **Parent:** [Viii](#1/viii)

For the initial data, the two weighted integrals equal $(\phi_0/c)\operatorname{sgn}(x)\int_0^Le^{\mp fy/c}dy$. Following their opposite characteristics to large time at fixed $x$ gives the additional final-state conditions

$$
\boxed{
\int_0^Le^{-fy/c}\left(-\frac{\Phi_y}{f}+\frac\Phi c\right)dy
=-\frac{\phi_0}{c}\int_0^Le^{-fy/c}dy,}
$$



$$
\boxed{
\int_0^Le^{fy/c}\left(-\frac{\Phi_y}{f}+\frac\Phi c\right)dy
=\frac{\phi_0}{c}\int_0^Le^{fy/c}dy.}
$$

These two scalar constraints determine the two coefficients $A,B$ in the nullspace from part v and therefore make the adjusted solution unique.

## 2

↑ **Parent:** [Paper 333](paper-333.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Assume $f>0$; replacing it by $|f|$ gives the thickness for either hemisphere. With $W=(u-U)+iv$, the steady anomaly equations reduce to

$$
\nu W''=ifW,
\qquad W(0)=-U,
\qquad W(\infty)=0.
$$

Thus the [Bottom Ekman layer](../../../geophysical-fluid-dynamics.md#bottom-ekman-layer) has

$$
\boxed{\delta=\left(\frac{2\nu}{f}\right)^{1/2},quad
u=U[1-e^{-z/\delta}\cos(z/\delta)],quad
v=Ue^{-z/\delta}\sin(z/\delta).}
$$

Its integrated anomalous transport is

$$
\boxed{\mathbf u_T=\frac\delta2(-\mathbf U_g+\widehat{\mathbf z}\times\mathbf U_g).}
$$

It is the transport required by the vertically integrated momentum balance between Coriolis acceleration and bottom stress. For slowly varying geostrophic flow, $\nabla\cdot\mathbf U_g=0$ and $\nabla\cdot(\widehat z\times\mathbf U_g)=-\zeta_g$, so

$$
\nabla\cdot\mathbf u_T=-\frac\delta2\zeta_g.
$$

Mass conservation therefore gives the interior [Ekman pumping](../../../geophysical-fluid-dynamics.md#ekman-pumping) condition

$$
\boxed{w(0^+)=\frac\delta2\zeta_g=\frac\delta2\nabla_h^2\psi.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

In the [quasi-geostrophic approximation](../../../geophysical-fluid-dynamics.md#quasi-geostrophic-approximation), buoyancy is proportional to $f\psi_z$ and its material equation gives

$$
w=-\frac f{N^2}\frac{D_g\psi_z}{Dt}.
$$

The governing interior and boundary equations are consequently

$$
\boxed{\frac{D_g}{Dt}\left(\nabla_h^2\psi+\frac{f^2}{N^2}\psi_{zz}\right)=0\quad(z>0),}
$$



$$
\boxed{\frac{D_g\psi_z}{Dt}=-\frac{N^2\delta}{2f}\nabla_h^2\psi\quad(z=0).}
$$

After linearization about rest, put $m=Nk/|f|$ and $r=Nk\delta/2$. The initial PV is $-k^2\psi_0\sin kx$, and the decaying homogeneous vertical solution gives

$$
\boxed{psi=\psi_0\left[1-(1-e^{-rt})e^{-mz}\right]\sin kx.}
$$

The boundary current decays on time $r^{-1}=2/(Nk\delta)$, while the original current survives aloft. The boundary influence penetrates only

$$
\boxed{m^{-1}=\frac{|f|}{Nk}.}
$$

Stronger stratification or shorter horizontal scale confines the adjustment more tightly; rotation communicates it farther upward. This is [quasi-geostrophic Ekman spin-down](../../../geophysical-fluid-dynamics.md#quasi-geostrophic-ekman-spin-down).

## 3

↑ **Parent:** [Paper 333](paper-333.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Multiply the perturbation PV equation by $q'/\beta$ and take an $x$ average. Periodicity makes averages of $x$ derivatives vanish, while integration by parts gives

$$
\overline{\psi_xq'}
=\partial_y(-\overline{u'v'})
+\partial_z\left(\frac{f_0^2}{N^2}\overline{\psi_x'\psi_z'}\right).
$$

Using $\rho'=-f_0\rho_0\psi_z'/g$ proves the [quasi-geostrophic wave-activity conservation law](../../../geophysical-fluid-dynamics.md#quasi-geostrophic-wave-activity-conservation-law)

$$
\boxed{A_t+\nabla\cdot\mathbf F=\frac{\overline{Q'q'}}\beta,\quad
A=\frac{\overline{q'^2}}{2\beta},\quad
\mathbf F=\left(0,-\overline{u'v'},-\frac{gf_0}{\rho_0N^2}\overline{v'\rho'}\right).}
$$

$A_t$ is local wave-activity storage, $\nabla\cdot\mathbf F$ is propagation and mean-flow forcing, and $\overline{Q'q'}/\beta$ creates or destroys wave activity. A steady unforced wave has both $A_t=0$ and $Q'=0$, hence $\nabla\cdot\mathbf F=0$ and exerts no mean force.

For $K^2=k^2+l^2$, substitution of $\widehat\psi(z)e^{ikx}\sin ly$ gives

$$
\boxed{
\frac{f_0^2}{N^2}\widehat\psi''-K^2\widehat\psi+\frac\beta U\widehat\psi
=\frac{i\alpha}{kU}\frac{f_0^2}{N^2}\widehat\psi''.}
$$

Write $(1-i\alpha/(kU))^{-1/2}=\gamma_r+i\gamma_i$, where both parts are positive. If $D=\beta/U-K^2>0$, define $M=N\sqrt D/f_0$; the decaying propagating solution is

$$
\widehat\psi=Ae^{iM(\gamma_r+i\gamma_i)z}.
$$

If $D<0$, define $M=N\sqrt{-D}/f_0$; the decaying evanescent solution is

$$
\widehat\psi=Ae^{-M(\gamma_r+i\gamma_i)z}.
$$

The boundary condition fixes $A$ from $\widehat\psi'(0)=C\widehat h$. Thermal damping therefore selects decay for either sign of $D$, producing a [thermally damped quasi-geostrophic mountain wave](../../../geophysical-fluid-dynamics.md#thermally-damped-quasi-geostrophic-mountain-wave).

Since $u'=-\psi_y'$ and $v'=\psi_x'$, quadrature in $x$ gives $\boxed{F^{(y)}=0}$. Also

$$
F^{(z)}=\frac{f_0^2}{2N^2}\operatorname{Re}(ik\widehat\psi\widehat\psi'^*).
$$

Consequently

$$
\boxed{F^{(z)}=\frac{f_0^2kM\gamma_r}{2N^2}|\widehat\psi|^2>0\quad(D>0),}
$$



$$
\boxed{F^{(z)}=-\frac{f_0^2kM\gamma_i}{2N^2}|\widehat\psi|^2<0\quad(D<0).}
$$

Both fluxes tend to zero aloft. Their vertical divergence is respectively westward and eastward wave force; the equal and opposite integrated force is exerted by the flow on the lower topography. Damping thus permits topographic drag even for the evanescent regime and reverses its sign across the stationary-wave threshold.

## 4

↑ **Parent:** [Paper 333](paper-333.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Put $A=\gamma-i\omega$ and $B=\alpha-i\omega$. For $\widehat v=0$,

$$
\widehat u=-\frac{ik}{A}\widehat\phi,
\qquad
\widehat\phi=\phi_0\exp\left(\frac{i\beta k}{2A}y^2\right).
$$

Continuity gives the damped [equatorial Kelvin wave](../../../geophysical-fluid-dynamics.md#equatorial-kelvin-wave) dispersion relation

$$
\boxed{(\gamma-i\omega)(\alpha-i\omega)+c^2k^2=0.}
$$

Only roots satisfying $\operatorname{Re}(i\beta k/A)<0$ are trapped; for weak damping this is the eastward branch $k\operatorname{Re}\omega>0$. The other algebraic root makes the Gaussian grow with $|y|$ and must be rejected.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Elimination of $\widehat u$ and $\widehat\phi$ gives

$$
\widehat v_{yy}-\frac{\beta^2B}{c^2A}y^2\widehat v
+\frac{i\beta k}{A}\widehat v=0.
$$

Choose $\sigma^2=(\beta/c)(B/A)^{1/2}$ with $\operatorname{Re}\sigma^2>0$ and set $Y=\sigma y$. The Hermite eigenvalue condition gives, for $n=1,2,\ldots$,

$$
\boxed{\widehat v=V_n(\sigma y)=H_n(\sigma y)e^{-\sigma^2y^2/2},}
$$



$$
\boxed{(\gamma-i\omega)(\alpha-i\omega)+\frac{c^2k^2}{(2n+1)^2}=0.}
$$

Squaring the eigenvalue condition introduces an extraneous branch, so one must also impose $ikc/\sqrt{AB}=2n+1$ and $\operatorname{Re}\sigma^2>0$. For real $k$, trapped propagating roots exist when

$$
\boxed{|k|>\frac{(2n+1)|\alpha-\gamma|}{2c},}
$$

and the accepted root propagates westward, $k\operatorname{Re}\omega<0$. The other root has an outward-growing meridional structure.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

At $\omega=0$, the Kelvin relation gives $k=\pm i\sqrt{\alpha\gamma}/c$. Meridional trapping accepts only

$$
\boxed{k_K=+\frac{i\sqrt{\alpha\gamma}}c,}
$$

which is the response east of the forcing and has zonal decay length $c/\sqrt{\alpha\gamma}$. The Rossby relations give

$$
k=\pm\frac{i(2n+1)\sqrt{\alpha\gamma}}c.
$$

Trapping now accepts only

$$
\boxed{k_{R,n}=-\frac{i(2n+1)\sqrt{\alpha\gamma}}c,}
$$

so the response west of the forcing is a sum of [equatorial Rossby waves](../../../geophysical-fluid-dynamics.md#equatorial-rossby-wave); its longest zonal scale is $c/(3\sqrt{\alpha\gamma})$ for $n=1$.

Both families have

$$
\boxed{\sigma^2=\frac\beta c\sqrt{\frac\alpha\gamma},
\qquad
L_y=\sigma^{-1}=\left(\frac c\beta\sqrt{\frac\gamma\alpha}\right)^{1/2}.}
$$

**Thus the [damped equatorial Kelvin and Rossby response](../../../geophysical-fluid-dynamics.md#damped-equatorial-kelvin-and-rossby-response) extends farther east than west. Increasing either damping rate shortens the zonal tails, while their ratio controls the common meridional trapping width.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
