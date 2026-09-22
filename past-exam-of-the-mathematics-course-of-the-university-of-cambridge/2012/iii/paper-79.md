# Paper 79

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_79.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_79.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [a](#3/ii/a)
      - [Solution](#3/ii/a/solution)
    - [b](#3/ii/b)
      - [Solution](#3/ii/b/solution)
    - [c](#3/ii/c)
      - [Solution](#3/ii/c/solution)
    - [d](#3/ii/d)
      - [Solution](#3/ii/d/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 79](paper-79.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Use the horizontal [streamfunction](../../../fluid-mechanics.md#stream-function) convention $(u,v)=(-\psi_y,\psi_x)$, and set $a=\pi/L$, $k_d^2=f_0^2/(gH_0)$. [Geostrophic balance](../../../physics.md#geostrophic-balance) gives $f_0\bar u=-g\bar\eta_y$, hence

$$
\boxed{\bar\eta(y)=\eta_c+\frac{f_0U_0}{ga}\cos ay,\qquad \bar\psi=\frac{g\bar\eta}{f_0}=\psi_c+\frac{U_0}{a}\cos ay.}
$$

The constant is fixed by the total volume or the reference surface height. To obtain [shallow-water quasi-geostrophic potential vorticity](../../../geophysical-fluid-dynamics.md#shallow-water-quasi-geostrophic-potential-vorticity), require a small [Rossby number](../../../geophysical-fluid-dynamics.md#rossby-number), nearly geostrophic horizontal motion and $|\eta|/H_0\ll1$. Expanding the exact [shallow-water potential vorticity](../../../geophysical-fluid-dynamics.md#shallow-water-potential-vorticity) gives

$$
\frac{\zeta+f_0}{H_0+\eta}=\frac{f_0}{H_0}+\frac1{H_0}\left(\zeta-\frac{f_0\eta}{H_0}\right)+\text{higher orders}.
$$

At leading nontrivial order $\zeta=\nabla_h^2\psi$, so after removing the constant background and multiplying by $H_0$,

$$
\boxed{q=\nabla_h^2\psi-k_d^2\psi,\qquad q_t+J(\psi,q)=0,\quad J(A,B)=A_xB_y-A_yB_x.}
$$

The mean [potential vorticity](../../../geophysical-fluid-dynamics.md#potential-vorticity) and its gradient are

$$
\bar q=-\frac{U_0}{a}(a^2+k_d^2)\cos ay-k_d^2\psi_c,\qquad \boxed{\bar q_y=(a^2+k_d^2)\bar u.}
$$

With $\psi=\bar\psi+\psi'$ and $q=\bar q+q'$, expand the Jacobian. Since both mean fields depend only on $y$, their Jacobian vanishes. The two mixed terms are $\bar u q'_x$ and $v'\bar q_y$, giving

$$
\boxed{q'_t+J(\psi',q')+\bar u q'_x+v'\bar q_y=0,\qquad q'=(\nabla_h^2-k_d^2)\psi'.}
$$

The PDF has this correct mean-advection term; the TeX aid incorrectly inserts a division by $\partial x$.

Drop the quadratic perturbation Jacobian. Freeze $\bar u$ and $\bar q_y$ locally for a short-wave [plane wave](../../../quantum-mechanics.md#plane-wave), with $K^2=k^2+l^2$ and $D=K^2+k_d^2$. Then $q'=-D\psi'$, $v'=ik\psi'$, and the [local Rossby-wave dispersion relation in a zonal jet](../../../geophysical-fluid-dynamics.md#local-rossby-wave-dispersion-relation-in-a-zonal-jet) is

$$
\boxed{\omega=k\bar u-\frac{k\bar q_y}{D}=k\bar u\frac{K^2-a^2}{K^2+k_d^2}.}
$$

The intrinsic phase moves against an eastward mean flow because $\omega-k\bar u=-k\bar q_y/D$.

**The printed wavelength bound is not a consequence of these equations.** The local short-wave assumption is $K/a\gg1$, equivalently wavelength $2\pi/K\ll2L$; a particular cutoff $L/2$ is an optional scale-separation criterion, not a universal derived threshold. If one requires the ground-frame phase to follow the mean current, the dispersion relation only gives $K>a$, or wavelength less than $2L$. For example $K=2a,l=0$ has wavelength $L$ and a phase moving with the mean. More decisively, the stationary condition requested next fixes wavelength $2L$, contradicting a bound $L/2$ if both are imposed on the same waves.

For nonzero zonal $k$ and mean velocity, a ground-stationary wave satisfies

$$
\boxed{K=a=\pi/L.}
$$

It has the background length scale, so its existence should not be justified solely by the short-wave approximation. It is nevertheless an exact stationary linear solution of the [Rossby-wave equation for a sheared zonal current](../../../geophysical-fluid-dynamics.md#rossby-wave-equation-for-a-sheared-zonal-current): writing $\psi'=F(y)e^{ikx}$ gives $\bar u[F''-(k^2+k_d^2)F]+\bar q_y F=0$, which reduces to $F''+(a^2-k^2)F=0$. Thus $F=e^{ily}$ with $k^2+l^2=a^2$ works globally. Indeed the total field then has $q=-(a^2+k_d^2)\psi+$ a constant, so its full Jacobian vanishes as well.

Differentiating the local [dispersion relation](../../../wave-equation.md#dispersion-relation) gives

$$
\mathbf c_g=\left(\bar u\left[1-\frac{a^2+k_d^2}{D}+\frac{2(a^2+k_d^2)k^2}{D^2}\right],\frac{2\bar u(a^2+k_d^2)kl}{D^2}\right).
$$

On the stationary circle this becomes

$$
\boxed{\mathbf c_g=\frac{2\bar u k}{K^2+k_d^2}(k,l).}
$$

For a purely zonal wavevector, $l=0$, this is the printed expression $\mathbf c_g=2\bar u K^2\hat{\mathbf x}/(K^2+k_d^2)$. With $l\ne0$ the printed expression needs a directional qualification; the general vector is the one above. Here stationarity means $\omega=0$ in the ground frame, not vanishing intrinsic frequency in the moving fluid.

A stationary obstacle can therefore anchor the phase pattern while wave energy travels away from it. The zonal group component has the mean-flow sign, so an eastward jet carries the stationary wave response downstream; tilted wavevectors also carry energy meridionally. This is the usual stationary [Rossby wave](../../../geophysical-fluid-dynamics.md#rossby-wave) wake distinction between fixed phase crests and propagating wave energy.

## 2

↑ **Parent:** [Paper 79](paper-79.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Let $f(y)$ denote the signed vertical component of the [Coriolis parameter](../../../geophysical-fluid-dynamics.md#coriolis-parameter); it is negative in the southern hemisphere. In the steady, linear, inviscid interior, depth integration of horizontal momentum gives

$$
f\hat{\mathbf z}\times\mathbf U=-\nabla_h\Pi+\boldsymbol\tau^w/\rho_0,
$$

where $\mathbf U=\int_{-H}^0(u,v)dz$ and $\Pi=\int_{-H}^0p\,dz/\rho_0$. Horizontal curl eliminates the pressure. Its left side is $f\nabla_h\cdot\mathbf U+\beta V$. [Incompressibility](../../../fluid-mechanics.md#incompressible-flow) and impermeable flat top and bottom imply $\nabla_h\cdot\mathbf U=w(-H)-w(0)=0$, giving

$$
\boxed{\beta V=(\nabla_h\times\boldsymbol\tau^w)_z/\rho_0.}
$$

This is [Sverdrup balance](../../../geophysical-fluid-dynamics.md#sverdrup-balance). It assumes steady small-amplitude motion, a [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation), negligible nonlinear advection, negligible Rayleigh and bottom/lateral drag in the interior, a flat fixed-depth domain and no normal top/bottom flux. The applied surface wind stress remains a forcing, even though interior friction is neglected. With cooling absent, the steady buoyancy equation additionally requires $B_z=0$, if that equation is imposed; the curl balance itself does not depend on the cooling coefficient. In the closed, $x$-independent channel below, depth-integrated $V=0$, so a nonzero wind-stress curl cannot be balanced by an inviscid interior alone.

**Steady forced channel.** Now take $r>0,\alpha>0$. Put $a=\pi/L$, $s=(z+h)_+=\max(z+h,0)$ and write $\tau_0$ for the positive wind-stress amplitude. The prescribed profiles give

$$
b=\frac{B_z}{\alpha}=\frac{B_0}{\alpha h}\cos ay\quad(-h<z<0),\qquad b=0\quad(-H<z<-h),
$$



$$
F=\tau_{x,z}/\rho_0=\frac{2\tau_0s}{\rho_0h^2}\sin ay.
$$

The buoyancy jumps across the sharp forcing interface in this simplified model; pressure and the circulation below are continuous. Let $P=p_y/\rho_0$, $D=f^2+r^2$, and $b_y^{\rm top}=-aB_0\sin ay/(\alpha h)$. Hydrostatic balance gives $P=C(y)+b_y^{\rm top}s$. The horizontal momentum equations and their solution are

$$
ru-fv=F,\qquad fu+rv=-P,\qquad u=\frac{rF-fP}{D},\quad v=\frac{-fF-rP}{D}.
$$

The no-normal-flow conditions imply $\int_{-H}^0v\,dz=0$: this integral is independent of $y$ by [incompressibility](../../../fluid-mechanics.md#incompressible-flow) and is zero at the meridional walls. It determines the otherwise free depth-uniform pressure gradient,

$$
C(y)=-\frac{f\tau_0}{\rho_0rH}\sin ay-\frac{h^2}{2H}b_y^{\rm top}.
$$

Define

$$
A(y)=\frac{-f(y)\tau_0/\rho_0+r a B_0h/(2\alpha)}{f(y)^2+r^2},\qquad G(z)=\frac{z+H}{H}-\frac{s^2}{h^2}.
$$

A [meridional overturning streamfunction](../../../geophysical-fluid-dynamics.md#meridional-overturning-streamfunction) satisfying $v=-\Psi_z$, $w=\Psi_y$ is

$$
\boxed{\Psi(y,z)=A(y)\sin ay\,G(z),\qquad v=A(y)\sin ay\left(\frac{2s}{h^2}-\frac1H\right),\qquad w=[A(y)\sin ay]_yG(z).}
$$

It vanishes on all four boundaries. Together with the expressions for $b,P,u$, this solves all the steady equations. The formula permits variable $f(y)$; freezing it at a negative $f_0$ gives the simple schematic $w=aA\cos ay\,G(z)$. No unspecified latitude dependence is silently needed for the sketch.

Since $A>0$, upper-layer meridional transport is northward and the deep return is southward. At constant $f$, the circulation rises on the southern side and sinks on the northern side. The meridional velocity changes sign at $z=-h+h^2/(2H)$, slightly above the forcing interface, not exactly at $-h$. The required schematic follows from this derived field:

<a id="2/image-clockwise-deacon-circulation-northward-surface-transport-southward-deep-return-ascent-in-the-south-and-descent-in-the-north"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-79-deacon-cell.png)

**[Figure 1](#2/image-clockwise-deacon-circulation-northward-surface-transport-southward-deep-return-ascent-in-the-south-and-descent-in-the-north). Clockwise Deacon circulation: northward surface transport, southward deep return, ascent in the south and descent in the north**.

**Forcing comparison.** The buoyancy and wind contributions have the same vertical shape and, with these signs, the same circulation sense. Their ratio is

$$
\boxed{\frac{A_B}{A_W}=\frac r\alpha\frac{\pi h}{2L}\frac{B_0}{|f|\tau_0/\rho_0}\simeq\frac{\pi}{2}\,10^{-4}\simeq1.6\times10^{-4}.}
$$

The printed scaling $f\tau_0/\rho_0\simeq B_0$ must be understood in magnitude, since $f<0$ and both forcing amplitudes are positive. Surface confinement supplies the small factor $h/L$, making direct buoyancy forcing negligible in this circulation model.

The missing physical mechanism in the stratified Southern Ocean is [eddy-induced overturning](../../../geophysical-fluid-dynamics.md#eddy-induced-overturning). The wind-driven mean [Deacon cell](../../../geophysical-fluid-dynamics.md#deacon-cell) tilts [isopycnals](../../../fluid-mechanics.md#isopycnal) and builds [available potential energy](../../../classical-mechanics.md#available-potential-energy); [baroclinic instability](../../../hydrodynamic-stability.md#baroclinic-instability) produces mesoscale eddies whose buoyancy transport largely opposes the mean overturning. The residual circulation depends on the small net balance and the diabatic buoyancy transformation. Wind energy also enters mean kinetic energy; eddies redistribute momentum through form stress and transfer energy toward dissipative scales and bottom friction. The displayed linear model already balances its wind input by imposed drag, but omits this mean-advection/eddy buoyancy budget, so the necessity of an opposing eddy circulation is a physical extension, not another mathematical constraint on the four given equations.

## 3

↑ **Parent:** [Paper 79](paper-79.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Define the positive total shear stress by $\tau=\rho[\nu U_z-\overline{u'w'}]$, so the physical wall traction on the fluid opposes the positive flow. The steady mean momentum equation gives

$$
0=-P_x+\tau_z,\qquad\boxed{\tau(z)=\tau_S+P_xz.}
$$

For a driving pressure gradient $P_x<0$, the stress decreases upward. It is approximately constant while

$$
\boxed{z\ll\delta_\tau=\tau_S/|P_x|,\qquad u_*=\sqrt{\tau_S/\rho}.}
$$

An outer boundary-layer height can impose a stricter limit. In the turbulent region outside the viscous or roughness sublayer, the only local neutral scales are $u_*$ and $z$, so $U_z=C u_*/z$. Conventionally write $C=1/\kappa$, where $\kappa$ is the von Kármán constant. Equivalently, a mixing length $\ell=\kappa z$ and stress closure $u_*^2=\ell^2U_z^2$ give the same result. Integration yields the [law of the wall](../../../continuum-mechanics.md#law-of-the-wall)

$$
\boxed{U(z)=\frac{u_*}{\kappa}\log\frac z{z_0}.}
$$

The [roughness length](../../../continuum-mechanics.md#roughness-length) $z_0$ is an extrapolation scale, not a statement that the logarithm is valid at the actual solid surface. For a smooth boundary, the viscous inner scales are $z^+=zu_*/\nu$, $U^+=U/u_*$. The viscous sublayer has $U^+\simeq z^+$; farther out $U^+=\kappa^{-1}\log z^++C_s$, corresponding to $z_0=(\nu/u_*)e^{-\kappa C_s}$. For a fully rough boundary, $z_0$ is proportional to a geometric roughness height and viscosity no longer determines the leading profile. The logarithmic region still needs roughness height $\ll z\ll\delta_\tau$.

In local equilibrium, production of [turbulent kinetic energy](../../../turbulence.md#turbulent-kinetic-energy) by the shear is $P=-\overline{u'w'}U_z\simeq u_*^2U_z$. Neglecting its transport relative to production and [viscous dissipation](../../../stokes-flow.md#viscous-dissipation),

$$
\boxed{\epsilon\simeq\frac{u_*^3}{\kappa z}.}
$$

Dimensional similarity alone gives $\epsilon\propto u_*^3/z$; the displayed coefficient additionally uses the local energy balance and the logarithmic shear.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/a">a</h4>

↑ **Parent:** [Ii](#3/ii)

<h5 id="3/ii/a/solution">Solution</h5>

↑ **Parent:** [A](#3/ii/a)

Let $B_0=\overline{w'b'}$ be the [vertical turbulent buoyancy flux](../../../turbulence.md#vertical-turbulent-buoyancy-flux), positive for heating from below. Its dimensions are length squared per time cubed. The stress velocity and height therefore admit a new dimensionless group $B_0z/u_*^3$. Define the signed [Obukhov length](../../../continuum-mechanics.md#monin-obukhov-length)

$$
\boxed{\ell_O=-\frac{u_*^3}{\kappa B_0},\qquad \zeta=z/\ell_O.}
$$

Stable cooling has $B_0<0,\ell_O>0$; unstable heating has $B_0>0,\ell_O<0$. [Monin-Obukhov similarity theory](../../../continuum-mechanics.md#monin-obukhov-similarity-theory) expresses the mean shear as

$$
\boxed{\frac{dU}{dz}=\frac{u_*}{\kappa z}\phi_m(\zeta),\qquad \phi_m(0)=1.}
$$

The similarity hypothesis assumes approximately steady, horizontally homogeneous, constant-stress and constant-flux conditions, with the observation level outside the inner sublayer but below the outer-layer scales. Dimensional analysis fixes the arguments and prefactor, not the entire function $\phi_m$. A measured or modeled turbulence closure supplies its form.

<h4 id="3/ii/b">b</h4>

↑ **Parent:** [Ii](#3/ii)

<h5 id="3/ii/b/solution">Solution</h5>

↑ **Parent:** [B](#3/ii/b)

For a rough boundary, integrate the similarity shear from the [roughness length](../../../continuum-mechanics.md#roughness-length). A usual moderate-stability closure is

$$
\phi_m(\zeta)=1+c_s\zeta\quad(\zeta\geq0),\qquad \phi_m(\zeta)=(1-c_u\zeta)^{-1/4}\quad(\zeta\leq0),
$$

with positive dimensionless coefficients. These are empirical closures, not quantities determined by similarity alone. An often-used choice is $c_s=5,c_u=16$. The unstable quarter-power relation is tested over approximately $-1\lesssim z/\ell_O\lesssim-0.01$ in [Dyer's flux-gradient study](https://rmets.onlinelibrary.wiley.com/doi/10.1002/qj.49709641012); the stable coefficient convention is recorded in [the surface-flux formulation](https://journals.ametsoc.org/view/journals/apme/36/10/1520-0450_1997_036_1416_iosfci_2.0.co_2.xml). Near neutrality one takes their smooth limits.

For moderate stable conditions, integration gives

$$
\boxed{U(z)=\frac{u_*}{\kappa}\left[\log\frac z{z_0}+c_s\frac{z-z_0}{\ell_O}\right].}
$$

For the unstable closure set $x(\zeta)=(1-c_u\zeta)^{1/4}$ and define

$$
\psi_m(\zeta)=2\log\frac{1+x}{2}+\log\frac{1+x^2}{2}-2\arctan x+\frac\pi2.
$$

Then $1-\zeta\psi_m'(\zeta)=\phi_m(\zeta)$ and

$$
\boxed{U(z)=\frac{u_*}{\kappa}\left[\log\frac z{z_0}-\psi_m(z/\ell_O)+\psi_m(z_0/\ell_O)\right].}
$$

For weak unstable departure, $|c_u z/\ell_O|\ll1$, this reduces to the stable-form expression with $c_s$ replaced by $c_u/4$ and a negative $\ell_O$. The full quarter-power expression is useful for moderately unstable conditions with $|z/\ell_O|$ of order one; it must not be extrapolated automatically to the distinct asymptotic free-convection regime. The stable linear expression similarly describes a continuously turbulent surface layer, rather than guaranteeing validity after strong stratification destroys the constant-flux state. Both profiles require $z_0\ll z\ll\delta_\tau$ and approximately uniform fluxes.

<h4 id="3/ii/c">c</h4>

↑ **Parent:** [Ii](#3/ii)

<h5 id="3/ii/c/solution">Solution</h5>

↑ **Parent:** [C](#3/ii/c)

At fixed [friction velocity](../../../viscous-fluid-flow.md#shear-velocity), unstable heating gives $B_0>0$ and $\zeta<0$. The usual similarity closure has $\phi_m<1$, so it reduces the mean velocity gradient relative to the neutral [law of the wall](../../../continuum-mechanics.md#law-of-the-wall). Rising warm and descending cool parcels mix momentum efficiently; less mean shear is needed to transport the same stress. Relative to a fixed near-wall reference, the speed difference aloft is reduced.

Stable cooling gives $B_0<0,\zeta>0$ and $\phi_m>1$. The restoring buoyancy suppresses vertical parcel excursions and reduces the effective momentum diffusivity, requiring a steeper shear for the same stress. The speed difference from the wall reference is correspondingly larger. These are comparisons at prescribed stress; fixing an outer wind instead would allow $u_*$ and the stress to change, so it would not be the same comparison.

<h4 id="3/ii/d">d</h4>

↑ **Parent:** [Ii](#3/ii)

<h5 id="3/ii/d/solution">Solution</h5>

↑ **Parent:** [D](#3/ii/d)

Write $S=U_z$ and $N^2=d\bar b/dz$. The [gradient Richardson number](../../../gravity-wave.md#gradient-richardson-number) and [Flux Richardson number](../../../gravity-wave.md#flux-richardson-number) are

$$
\boxed{\mathrm{Ri}_g=\frac{N^2}{S^2},\qquad \mathrm{Ri}_f=-\frac{\overline{w'b'}}{-\overline{u'w'}S}=-\frac{B_0}{P}.}
$$

The first compares the restoring buoyancy gradient with mean shear; the second is the fraction of shear production consumed by stable buoyancy work. With this convention, both are positive for stable mixing and negative for unstable stratification. In local steady equilibrium, $\epsilon=P+B_0=P(1-\mathrm{Ri}_f)$, so a positive dissipation requires $\mathrm{Ri}_f<1$. The inviscid [Miles–Howard theorem](../../../gravity-wave.md#miles-howard-theorem) concerning $\mathrm{Ri}_g\geq1/4$ is a linear stability criterion, not a universal equality for turbulent fluxes.

Use the gradient-diffusion closures $-\overline{u'w'}=K_mS$ and $B_0=-K_bN^2$. The [turbulent Prandtl number](../../../turbulence.md#turbulent-prandtl-number) is $\mathrm{Pr}_t=K_m/K_b$, giving

$$
\boxed{\mathrm{Ri}_f=\frac{K_b}{K_m}\mathrm{Ri}_g=\frac{\mathrm{Ri}_g}{\mathrm{Pr}_t}.}
$$

Under the ideal [Reynolds analogy](../../../turbulence.md#reynolds-analogy) $K_m=K_b$, the two Richardson numbers coincide. It is an additional closure, not an automatic consequence of the definitions. If the buoyancy-gradient similarity function is defined by $N^2=-B_0\phi_h/(\kappa zu_*)$, then

$$
\boxed{\mathrm{Ri}_g=\zeta\frac{\phi_h}{\phi_m^2},\qquad \mathrm{Ri}_f=\frac{\zeta}{\phi_m},\qquad \mathrm{Pr}_t=\frac{\phi_h}{\phi_m}.}
$$

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

For lower-boundary heating, forced convection means that mean shear supplies most of the turbulence even though buoyancy assists it, approximately $z\ll|\ell_O|$. Free convection means buoyancy dominates, approximately $z\gg|\ell_O|$ within the constant-flux region. In this limit the local convective speed is

$$
\boxed{w_c\sim(B_0z)^{1/3}.}
$$

It is the velocity whose eddy transport supplies the imposed [vertical turbulent buoyancy flux](../../../turbulence.md#vertical-turbulent-buoyancy-flux). The associated diffusivity is $K_b=C_Kw_cz=C_KB_0^{1/3}z^{4/3}$, with a dimensionless coefficient fixed by a closure. From $B_0=-K_bN^2$,

$$
\boxed{N^2=-C_K^{-1}B_0^{2/3}z^{-4/3},\qquad |N|=C_K^{-1/2}B_0^{1/3}z^{-2/3}.}
$$

Here $N^2<0$: there is no real restoring [buoyancy frequency](../../../gravity-wave.md#buoyancy-frequency). The displayed magnitude is a local overturning/growth rate, or one may write $N=i|N|$. The [Reynolds analogy](../../../turbulence.md#reynolds-analogy) makes $K_m=K_b$ and hence $U_z\sim u_*^2B_0^{-1/3}z^{-4/3}$; the remaining mean shear is weak compared with the convective motion.

The turnover dissipation estimate gives

$$
\boxed{\epsilon\sim\frac{w_c^3}{z}\sim B_0,}
$$

also consistent with the local energy equation $\epsilon=P+B_0$ when $P$ is negligible. Thus free-convection dissipation is height independent to leading scaling order, in contrast with neutral $u_*^3/(\kappa z)$. The constants and detailed profiles are not determined by dimensional analysis. These are local [free-convection surface-layer scalings](../../../fluid-mechanics.md#free-convection-surface-layer-scaling), not a claim that an entire deep convecting layer has a uniform unstable mean buoyancy gradient.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

For very stable continuously turbulent conditions, $z\gg\ell_O>0$, local eddies lose leading dependence on their distance from the wall. In [very stable surface-layer similarity](../../../continuum-mechanics.md#very-stable-surface-layer-similarity), the dimensionless functions must therefore scale as $\phi_m\sim c_m\zeta$ and $\phi_h\sim c_h\zeta$, with positive closure constants. Using $\ell_O=u_*^3/(\kappa|B_0|)$ gives

$$
\boxed{U_z\sim c_m\frac{|B_0|}{u_*^2},\qquad U(z)-U(z_r)\sim c_m\frac{|B_0|}{u_*^2}(z-z_r),\qquad N^2\sim c_h\frac{|B_0|^2}{u_*^4}.}
$$

Thus the mean velocity is approximately linear in height and the real [buoyancy frequency](../../../gravity-wave.md#buoyancy-frequency) is approximately constant, $N\sim\sqrt{c_h}|B_0|/u_*^2$. Under the [Reynolds analogy](../../../turbulence.md#reynolds-analogy), $c_h=c_m$.

The [local turbulent kinetic energy balance](../../../turbulence.md#local-turbulent-kinetic-energy-balance) gives

$$
\boxed{\epsilon=P-|B_0|\sim(c_m-1)|B_0|,\qquad \ell_\epsilon\sim\frac{u_*^3}{\epsilon}=\frac{u_*^3}{(c_m-1)|B_0|}.}
$$

Positive dissipation requires $c_m>1$. The turbulent energy-turnover length is of order $u_*^3/|B_0|$, hence of order the [Obukhov length](../../../continuum-mechanics.md#monin-obukhov-length), independent of observation height. A related buoyancy-limited length is $u_*/N$. The [Ozmidov length](../../../gravity-wave.md#ozmidov-length) follows by equating an eddy turnover time $\ell^{2/3}\epsilon^{-1/3}$ with $N^{-1}$:

$$
\ell_{\rm Oz}=(\epsilon/N^3)^{1/2}\sim\frac{\sqrt{c_m-1}}{c_h^{3/4}}\frac{u_*^3}{|B_0|}.
$$

These are turbulent turnover or buoyancy-transition scales. If “the scale at which dissipation occurs” means the actual viscous cutoff, molecular viscosity is also required: the [Kolmogorov microscales](../../../turbulence.md#kolmogorov-microscales) give

$$
\boxed{\eta_K=(\nu^3/\epsilon)^{1/4}\sim\left[\frac{\nu^3}{(c_m-1)|B_0|}\right]^{1/4}.}
$$

Without $\nu$, the viscous length cannot be fixed by the supplied stress and flux alone. Separating it from the turbulent turnover length avoids confusing an energy-budget estimate with the molecular cutoff.

Finally,

$$
\boxed{\mathrm{Ri}_f\longrightarrow\frac1{c_m},\qquad \mathrm{Ri}_g\longrightarrow\frac{c_h}{c_m^2}.}
$$

They become height-independent constants. The commonly used continuation $c_m=c_h=5$ gives $\mathrm{Ri}_f=\mathrm{Ri}_g\simeq0.2$ and $\epsilon\simeq4|B_0|$. This numerical value is a closure choice, not a deduction from units; setting $c_m=1$ would incorrectly leave zero dissipation. Extremely stable intermittent or collapsed turbulence need not satisfy this local-equilibrium model. The relation between the Obukhov and buoyancy-dissipation lengths in the local regime is also analyzed in [Grachev and colleagues' similarity study](https://arxiv.org/abs/1404.1397).

## 4

↑ **Parent:** [Paper 79](paper-79.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Use a [top-hat plume model](../../../turbulent-plume.md#top-hat-plume-model) per unit span. Define volume and kinematic momentum fluxes $Q=bw$ and $J=bw^2$, and set the pure-ice [reduced gravity](../../../reduced-gravity.md) $g'=g(\rho_0-\rho_s)/\rho_0>0$. The suspension buoyancy is $g'\phi$. The supplied equations express vertical [momentum conservation](../../../classical-mechanics.md#momentum-conservation), conservation of relative enthalpy including latent heat, and conservation of excess salt, respectively. At the release height, prescribe compatible source volume/momentum, salt and enthalpy fluxes, or equivalent source width, velocity, composition and ice fraction; impose ambient entrained water at $(T_0,C_0)$ with no vertical momentum. A pure far-field similarity solution may instead be described using a virtual origin, but its singular near-origin values are not physical inlet conditions.

The missing balance is total mass, equivalently volume under the [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation). In a wall plume, only the exposed outer edge entrains, so the [Batchelor entrainment hypothesis](../../../turbulent-plume.md#batchelor-entrainment-hypothesis) $v_e=e\,w$ gives

$$
\boxed{Q'=e\,w.}
$$

If two free edges are intended, replace $e$ by $2e$ everywhere; the numerical coefficient is a geometry convention. The glacier boundary itself has no normal flow. Local phase conversion does not add volume at retained Boussinesq order, and crystals are assumed to share the liquid velocity.

For a box of height $dz$, the upward momentum flux changes by $\rho_0[J(z+dz)-J(z)]$. The ambient hydrostatic pressure has been subtracted; the remaining force is the suspension buoyancy $\rho_0bg'\phi\,dz$. Entrained ambient water carries no vertical momentum, and drag is neglected, giving $J'=bg'\phi$. Salt entering through the exposed edge is $C_0Q'\,dz$, so $(\bar C Q)'=C_0Q'$ and therefore

$$
\boxed{J'=bg'\phi,\qquad[(\bar C-C_0)Q]'=0.}
$$

These control-volume derivations account for entrainment rather than treating $Q$ as constant.

**Thermodynamic elimination.** Let the conserved excess enthalpy and salt fluxes be $E$ and $S$:

$$
E=[c_p(T-T_0)-L\phi]Q,\qquad S=(\bar C-C_0)Q.
$$

The ambient satisfies $T_0=-mC_0$, while equilibrium in the ice-bearing plume gives

$$
\bar C=C_0+S/Q,\qquad T=-m\frac{C_0+S/Q}{1-\phi}.
$$

Substitute this temperature in the enthalpy invariant. Exact rearrangement gives

$$
\boxed{\phi Q[L+c_pmC_0-L\phi]=-E-c_pmS+E\phi.}
$$

Thus, at dilute-crystal order,

$$
\boxed{\phi Q\simeq I_0=\frac{-E-c_pmS}{L+c_pmC_0},\qquad \mathcal F=g'I_0.}
$$

The [ice-bearing wall-plume thermodynamic invariant](../../../turbulent-plume.md#ice-bearing-wall-plume-thermodynamic-invariant) fixes the leading advected ice volume and buoyancy flux from the source deficits. A rising ice-dominated branch requires $I_0>0$. It is not determined from reduced gravity alone. The small-$\phi$ expansion also presumes finite source fluxes and no cancellation making the discarded terms comparable to $-E-c_pmS$.

The three remaining leading equations are $Q'=e w$, $(Qw)'=\mathcal F/w$, and $\phi=I_0/Q$. Seek a similarity form in $Z=z-z_v>0$ with $Q\propto Z^p$, $w\propto Z^q$. Continuity gives $p=q+1$, while momentum gives $p+2q=1$. Therefore $q=0,p=1$. The coefficients obey $e w^3=\mathcal F$, giving the [self-similar ice-bearing wall plume](../../../turbulent-plume.md#self-similar-ice-bearing-wall-plume)

$$
\boxed{b=eZ,\qquad w=\left(\frac{g'I_0}{e}\right)^{1/3},\qquad Q=e\left(\frac{g'I_0}{e}\right)^{1/3}Z,\qquad\phi=\frac{w^2}{g'Z}=\frac{I_0^{2/3}}{e^{2/3}g'^{1/3}Z}.}
$$

The width grows linearly, the speed approaches a constant, and the crystals dilute inversely with height. This is a buoyancy-conserving [wall line plume](../../../turbulent-plume.md#wall-line-plume), with buoyancy supplied mainly by the ice fraction rather than a temperature anomaly. The dilute-crystal regime requires $Z\gg w^2/g'$ and lies away from the formal virtual-origin singularity. If all source flux deficits vanish, $I_0=0$ and this nontrivial rising branch does not exist. The exact thermodynamic invariants above, rather than their truncated version, are needed near a concentrated source.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
