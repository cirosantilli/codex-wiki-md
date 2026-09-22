# Paper 66

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper66.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper66.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Work in the frame in which the distant fluid is stationary, and take the [pressure](../../../thermodynamics.md#pressure) at infinity as zero. In the [Unscaled Papkovich–Neuber representation](../../../stokes-flow.md#unscaled-papkovich-neuber-representation), choose the harmonic potentials

$$
\boldsymbol\Phi=-\frac{3a}{4r}\mathbf V,\qquad
\chi=\frac{a^3}{4}\frac{\mathbf V\cdot\mathbf x}{r^3}.
$$

Both are harmonic away from the sphere's centre: $1/r$ is harmonic there and $\mathbf V\cdot\mathbf x/r^3=-\mathbf V\cdot\nabla(1/r)$. Substitution into $\mathbf u=\nabla(\mathbf x\cdot\boldsymbol\Phi+\chi)-2\boldsymbol\Phi$, $p=2\mu\nabla\cdot\boldsymbol\Phi$, gives the [translating sphere in Stokes flow](../../../stokes-flow.md#translating-sphere-in-stokes-flow):

$$
\boxed{\mathbf u=\left[\frac{3a}{4r}(\mathbf I+\mathbf n\mathbf n)+\frac{a^3}{4r^3}(\mathbf I-3\mathbf n\mathbf n)\right]\mathbf V,\qquad
p=\frac{3\mu a}{2r^2}\mathbf V\cdot\mathbf n.}
$$

Here $\mathbf n=\mathbf x/r$. At $r=a$ the coefficients of $\mathbf I$ sum to one and those of $\mathbf n\mathbf n$ sum to zero, so the [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) is satisfied. The field decays at infinity. The [Papkovich–Neuber representation](../../../stokes-flow.md#papkovich-neuber-representation) enforces the [Stokes equation](../../../stokes-flow.md#stokes-equation) and [incompressibility](../../../fluid-mechanics.md#incompressible-flow), and [Uniqueness of Stokes flow](../../../stokes-flow.md#uniqueness-of-stokes-flow) identifies the physical solution.

Differentiate radially at fixed direction $\mathbf n$:

$$
\left.\partial_r\mathbf u\right|_{a}
=\left[-\frac{3}{4a}(\mathbf I+\mathbf n\mathbf n)-\frac{3}{4a}(\mathbf I-3\mathbf n\mathbf n)\right]\mathbf V
=\boxed{\frac{3}{2a}(\mathbf n\mathbf n-\mathbf I)\mathbf V.}
$$

On the surface, multiplying the specified [Newtonian fluid stress tensor](../../../viscous-fluid-flow.md#newtonian-fluid-stress-tensor) by the outward normal from the solid gives

$$
\boldsymbol\sigma\mathbf n=\frac{3\mu}{2a}\left[(\mathbf V\cdot\mathbf n)\mathbf n-\mathbf V-\mathbf n(\mathbf V\cdot\mathbf n)\right]
=-\frac{3\mu}{2a}\mathbf V.
$$

Thus the [surface traction in translating-sphere Stokes flow](../../../stokes-flow.md#surface-traction-in-translating-sphere-stokes-flow) is uniform and the fluid's [force](../../../classical-mechanics.md#force) on the sphere is

$$
\boxed{\mathbf F_{\rm fluid}=\int_{r=a}\boldsymbol\sigma\mathbf n\,dS=-6\pi\mu a\mathbf V.}
$$

This is the [Stokes drag law](../../../stokes-flow.md#stokes-s-law); an external [force](../../../classical-mechanics.md#force) of the opposite sign maintains the motion.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $\mathbf F$ denote the applied [force](../../../classical-mechanics.md#force), and take the normal $\mathbf n_S$ outward from the solid. At leading order the [Stokes drag law](../../../stokes-flow.md#stokes-s-law) and the [torque](../../../classical-mechanics.md#torque) on a [rotating sphere in Stokes flow](../../../stokes-flow.md#rotating-sphere-in-stokes-flow) give

$$
\boxed{\mathbf U_0=\frac{\mathbf F}{6\pi\mu a},\qquad\boldsymbol\Omega_0=\mathbf0.}
$$

The exact [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) and the exact resultant-load conditions are

$$
\begin{gathered}
\mathbf u(\mathbf x)=\mathbf U+\boldsymbol\Omega\times\mathbf x\quad(\mathbf x\in S),\qquad\mathbf u\to\mathbf0\quad(r\to\infty),\\
\int_S\boldsymbol\sigma\mathbf n_S\,dS=-\mathbf F,\qquad
\int_S\mathbf x\times(\boldsymbol\sigma\mathbf n_S)\,dS=\mathbf0.
\end{gathered}
$$

The [stress](../../../continuum-mechanics.md#stress) condition specifies the total [force](../../../classical-mechanics.md#force) and [torque](../../../classical-mechanics.md#torque), not a pointwise prescribed [traction](../../../continuum-mechanics.md#traction).

For the [boundary perturbation of a nearly spherical particle](../../../stokes-flow.md#boundary-perturbation-of-a-nearly-spherical-particle), evaluate the no-slip condition at $\mathbf x=(a+\varepsilon f)\mathbf n$. Taylor expansion gives

$$
\mathbf u_0(a\mathbf n)+\varepsilon\left[\mathbf u_1(a\mathbf n)+f\partial_r\mathbf u_0(a\mathbf n)\right]
=\mathbf U_0+\varepsilon\left[\mathbf U_1+\boldsymbol\Omega_1\times(a\mathbf n)\right]+O(\varepsilon^2).
$$

There is no $f\boldsymbol\Omega_0\times\mathbf n$ term because $\boldsymbol\Omega_0=0$. Therefore

$$
\boxed{\mathbf u_1=\mathbf U_1+\boldsymbol\Omega_1\times\mathbf x-f\partial_r\mathbf u_0\quad(r=a).}
$$

To expand the integral conditions correctly, use [surface independence of Stokes force and torque integrals](../../../stokes-flow.md#surface-independence-of-stokes-force-and-torque-integrals). The [Stokes equation](../../../stokes-flow.md#stokes-equation) implies $\nabla\cdot\boldsymbol\sigma=0$, and symmetry of the [stress tensor](../../../continuum-mechanics.md#cauchy-stress-tensor) implies that the angular-momentum flux is divergence-free as well. Evaluate the exact [force](../../../classical-mechanics.md#force) and [torque](../../../classical-mechanics.md#torque) on a fixed sphere of radius $R$ enclosing the perturbed particle. There are then no geometric terms: the $O(\varepsilon)$ integrals of $\boldsymbol\sigma_1$ on that fixed sphere vanish because the external [force](../../../classical-mechanics.md#force) and [torque](../../../classical-mechanics.md#torque) have no $O(\varepsilon)$ corrections. Each perturbation field solves the homogeneous exterior Stokes equations, so the [divergence theorem](../../../calculus.md#divergence-theorem) transfers those integrals back to $r=a$. Hence

$$
\boxed{\int_{r=a}\boldsymbol\sigma_1\mathbf n\,dS=\mathbf0,\qquad
\int_{r=a}\mathbf x\times(\boldsymbol\sigma_1\mathbf n)\,dS=\mathbf0.}
$$

If the integrals are expanded directly on the displaced surface, terms involving the displaced evaluation of $\boldsymbol\sigma_0$, the changed normal and the changed area do appear individually. Their sum vanishes by the same surface-independence identity. Thus their absence in the final equations is a cancellation, not permission to omit geometric terms independently.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Write the first-order surface [velocity](../../../classical-mechanics.md#velocity) as $\mathbf u_1=\mathbf U_1+\boldsymbol\Omega_1\times\mathbf x+\mathbf g$, where the previous derivative gives

$$
\mathbf g=\frac{3f}{2a}(\mathbf I-\mathbf n\mathbf n)\mathbf U_0.
$$

As a test field, choose a sphere translating with arbitrary [velocity](../../../classical-mechanics.md#velocity) $\widehat{\mathbf V}$. Its surface [velocity](../../../classical-mechanics.md#velocity) is $\widehat{\mathbf V}$ and its [traction](../../../continuum-mechanics.md#traction) is $\widehat{\boldsymbol\sigma}\mathbf n=-3\mu\widehat{\mathbf V}/(2a)$. The [Lorentz reciprocal theorem for Stokes flow](../../../stokes-flow.md#lorentz-reciprocal-theorem-for-stokes-flow) gives

$$
\int_{r=a}\mathbf u_1\cdot\widehat{\boldsymbol\sigma}\mathbf n\,dS
=\int_{r=a}\widehat{\mathbf V}\cdot\boldsymbol\sigma_1\mathbf n\,dS=0.
$$

Terms at infinity vanish because both [velocities](../../../classical-mechanics.md#velocity) decay. Since $\int\mathbf n\,dS=0$, the rotation term has zero surface average. The arbitrary test [velocity](../../../classical-mechanics.md#velocity) therefore gives the [first-order mobility of a nearly spherical particle](../../../stokes-flow.md#first-order-mobility-of-a-nearly-spherical-particle):

$$
\boxed{\mathbf U_1=-\frac1{4\pi a^2}\int_{r=a}\mathbf g\,dS
=\frac{3}{8\pi a^3}\int_{r=a}f(\mathbf n)(\mathbf n\mathbf n-\mathbf I)\mathbf U_0\,dS.}
$$

For the ellipsoidal perturbation, the second spherical moment gives $\int f\,dS=(4\pi a^3/3)\operatorname{tr}\mathbf D=0$. The supplied fourth moment gives, componentwise,

$$
\int f n_i n_j\,dS
=\frac{4\pi a^3}{15}\left(\delta_{ij}\operatorname{tr}\mathbf D+D_{ij}+D_{ji}\right)
=\frac{8\pi a^3}{15}D_{ij}.
$$

Substitution yields

$$
\boxed{\mathbf U_1=\frac15\mathbf D\mathbf U_0=\frac15\mathbf U_0\cdot\mathbf D,}
$$

where the last notation uses symmetry of the [tensor](../../../linear-algebra.md#tensor).

One can also use a rotating-sphere test with surface [traction](../../../continuum-mechanics.md#traction) $-3\mu\widehat{\boldsymbol\Omega}\times\mathbf n$. Its reciprocal integral, together with zero first-order [torque](../../../classical-mechanics.md#torque), gives

$$
\boldsymbol\Omega_1=-\frac{3}{8\pi a^3}\int_{r=a}\mathbf n\times\mathbf g\,dS
=-\frac{9}{16\pi a^4}\int_{r=a}f(\mathbf n)\mathbf n\times\mathbf U_0\,dS.
$$

Here $f(-\mathbf n)=f(\mathbf n)$, so the last integrand is odd and its integral vanishes. Thus **$\boldsymbol\Omega_1=0$**. Inversion symmetry forbids a translation-to-rotation coupling for this centred ellipsoidal perturbation.

## 2

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

First estimate transverse relaxation without assuming a thin cross-section. With both depth and width of order $h_0$, a transverse surface-height variation of order $h_0$ gives a [pressure gradient](../../../fluid-mechanics.md#pressure-gradient) of order $\rho g$. The [Stokes equation](../../../stokes-flow.md#stokes-equation) then gives transverse horizontal and vertical [velocities](../../../classical-mechanics.md#velocity) of order $gh_0^2/\nu$. Moving the surface through distance $h_0$ takes

$$
\boxed{\tau_y\sim\frac{\nu}{gh_0}.}
$$

For longitudinal variations over $L\gg h_0$, the hydrostatic [pressure](../../../thermodynamics.md#pressure) gradient is of order $\rho gh_0/L$, so the longitudinal [velocity](../../../classical-mechanics.md#velocity) is $u\sim gh_0^3/(\nu L)$. [Incompressibility](../../../fluid-mechanics.md#incompressible-flow) gives a vertical [velocity](../../../classical-mechanics.md#velocity) $w\sim h_0u/L$, hence

$$
\boxed{\tau_x\sim\frac{h_0}{w}\sim\frac{\nu L^2}{gh_0^3},\qquad
\frac{\tau_y}{\tau_x}\sim\frac{h_0^2}{L^2}\ll1.}
$$

Thus cross-channel variations relax rapidly compared with the longitudinal evolution. These are viscous estimates, requiring inertial relaxation to be negligible; the slow-flow regime in particular excludes a large transverse inertial response. After that initial relaxation the [free surface](../../../fluid-mechanics.md#free-surface) is nearly horizontal across the channel, so its height is $h_0(x,t)$ and its local vertical depth is $h_0-|y|\cot\alpha$.

Retain the full cross-sectional geometry for a fixed $0<\alpha<\pi/2$; no small-angle approximation is used. With $|h_{0x}|\ll1$, the leading [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure) is $p=p_a+\rho g(h_0-z)$. Axial viscous derivatives are small relative to cross-sectional ones. The axial [Stokes equation](../../../stokes-flow.md#stokes-equation) is therefore

$$
\nu(u_{yy}+u_{zz})=g h_{0x}.
$$

Introduce $Y=y/h_0$, $Z=z/h_0$, and the triangular domain

$$
\mathcal D_\alpha=\{(Y,Z): |Y|\cot\alpha<Z<1\}.
$$

Let the dimensionless cross-sectional [Poisson equation](../../../partial-differential-equation.md#poisson-equation) be

$$
\phi_{YY}+\phi_{ZZ}=-1\quad\hbox{in }\mathcal D_\alpha,\qquad
\phi=0\quad(Z=|Y|\cot\alpha),\qquad
\phi_Z=0\quad(Z=1).
$$

The two lower sloping sides impose the [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition); the upper horizontal side imposes the [stress-free boundary condition](../../../viscous-fluid-flow.md#stress-free-boundary-condition). Symmetry would additionally give $\phi_Y=0$ at $Y=0$ if only half the domain were used. The full domain needs no extra midline boundary condition. Define $Q(\alpha)=\int_{\mathcal D_\alpha}\phi\,dY\,dZ$. Then

$$
u=-\frac{g}{\nu}h_0^2h_{0x}\phi(Y,Z),\qquad
q=\int u\,dy\,dz=-\frac{gQ(\alpha)}{\nu}h_0^4h_{0x}.
$$

The cross-sectional area is $A=h_0^2\tan\alpha$. [Conservation of mass](../../../continuum-mechanics.md#mass-conservation), $A_t+q_x=0$, gives the [V-shaped channel gravity current](../../../reduced-gravity.md#v-shaped-channel-gravity-current) equation

$$
\boxed{\tan\alpha\,(h_0^2)_t=\frac{gQ(\alpha)}{\nu}(h_0^4h_{0x})_x.}
$$

In particular, neither replacing this triangular Poisson problem by a vertically parabolic film nor taking an extreme angle is necessary.

Put $C=gQ(\alpha)/(\nu\tan\alpha)$. For a symmetric fixed-volume [similarity solution](../../../partial-differential-equation.md#similarity-solution), write $h_0=t^{-b}f(xt^{-d})$. Volume conservation gives $d=2b$, and balancing $(h_0^2)_t=C(h_0^4h_{0x})_x$ gives $2b+1=5b+2d$. Hence $b=1/7$, $d=2/7$. Integrating the similarity equation once, with zero flux at the centre, yields

$$
Ch_0^4h_{0x}=-\frac{2x}{7t}h_0^2.
$$

Integrating again and imposing $h_0=0$ at $x=\pm X(t)$ gives

$$
\boxed{h_0(x,t)=\left[\frac{3}{7Ct}(X^2-x^2)\right]^{1/3}\quad(|x|<X),\qquad h_0=0\quad(|x|\geq X).}
$$

The [constant-volume similarity in a V-shaped channel](../../../reduced-gravity.md#constant-volume-similarity-in-a-v-shaped-channel) has a compact support. If $H(t)=h_0(0,t)$, its volume is

$$
V=\tan\alpha\,H^2X I,\qquad
I=\int_{-1}^{1}(1-s^2)^{2/3}\,ds,\qquad
H^3=\frac{3X^2}{7Ct}.
$$

Eliminating $H$ therefore gives

$$
\boxed{x_N(t)=X(t)=\left(\frac{V}{I\tan\alpha}\right)^{3/7}
\left(\frac{7gQ(\alpha)t}{3\nu\tan\alpha}\right)^{2/7}.}
$$

This describes the large-time spreading from a localized release; the point-release profile is singular at $t=0$, and the idealized front has a narrow region where its divergent slope violates the long-wave approximation. Neither feature changes the leading bulk similarity law.

At a fixed nonzero $x^*$, the depth is initially zero until $X(t)=|x^*|$. After arrival it rises and then falls. Because $X^2\propto t^{4/7}$, differentiation of $h_0(x^*,t)^3=3(X^2-x^{*2})/(7Ct)$ gives

$$
\frac{d}{dt}h_0^3=\frac{3}{7Ct^2}\left(x^{*2}-\frac37X^2\right).
$$

Thus its unique maximum occurs at **$X^2=7x^{*2}/3$**; thereafter the depth tends to zero as $t^{-1/7}$. If $t_a$ is the arrival time, $t_{\max}/t_a=(7/3)^{7/4}$. At the singular release point $x^*=0$, the point-source similarity profile instead decreases from the start; a finite initial release regularizes its early behaviour.

<a id="2/image-depth-history-at-a-fixed-channel-station-and-residual-wall-films-after-the-bulk-level-falls-to-half-its-maximum"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-66-channel.png)

**[Figure 1](#2/image-depth-history-at-a-fixed-channel-station-and-residual-wall-films-after-the-bulk-level-falls-to-half-its-maximum). Depth history at a fixed channel station and residual wall films after the bulk level falls to half its maximum**.

The right-hand sketch shows the triangular bulk at half its previous maximum depth, with thin draining films on the previously wetted portions of both walls. These [residual wall films in a receding gravity current](../../../viscous-fluid-flow.md#residual-wall-films-in-a-receding-gravity-current) are not captured by a perfectly dry-wall triangular section. They drain rapidly compared with bulk longitudinal spreading. For an order-one angle, a wall film of thickness $b$ and wetted length $\ell$ has speed $O(gb^2/\nu)$ by [falling film flow](../../../viscous-fluid-flow.md#falling-film-flow); its drainage time gives $b\sim(\nu\ell/(gt))^{1/2}$. At a fixed nonzero station the previous maximum wetted height is finite, so film area decays as $t^{-1/2}$, faster than the bulk area $h_0^2\sim t^{-2/7}$. In stations whose arrival and peak times are of order the observation time, the typical residual film fraction is $O(\sqrt{\tau_y/t})\to0$. Therefore the films modify the detailed receding cross-section but do not hold a leading-order fraction of the volume or invalidate the large-time nose law. Microscopic contact-line physics is beyond this ideal viscous model.

## 3

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Let the longitudinal variation scale be $\ell\gg h$. The [stress-free boundary condition](../../../viscous-fluid-flow.md#stress-free-boundary-condition) gives $\mu(u_z+w_x)=0$ at each face. [Incompressibility](../../../fluid-mechanics.md#incompressible-flow) implies $w=O(hu/\ell)$, so $w_x$ is smaller than a putative $u_z=O(u/h)$ by $O(h^2/\ell^2)$. The leading [Stokes equation](../../../stokes-flow.md#stokes-equation) and the two shear-free conditions therefore make $u$ independent of $z$; its thickness-dependent correction is smaller-order. Symmetry gives $w=0$ at $z=0$, and incompressibility integrates to

$$
\boxed{w=-zu_x.}
$$

Vertical momentum makes the leading normal [stress](../../../continuum-mechanics.md#stress) independent of $z$. With the normal directed from liquid into gas, the upper-face curvature is $-h_{xx}/2$ to leading order. The [Young–Laplace equation](../../../fluid-mechanics.md#young-laplace-equation) gives

$$
\boxed{\sigma_{zz}=-p_a+\frac\gamma2h_{xx}.}
$$

The [Newtonian fluid stress tensor](../../../viscous-fluid-flow.md#newtonian-fluid-stress-tensor) also gives $\sigma_{zz}=-p+2\mu w_z=-p-2\mu u_x$. Hence $p=p_a-\gamma h_{xx}/2-2\mu u_x$ and

$$
\boxed{\sigma_{xx}=-p_a+\frac\gamma2h_{xx}+4\mu u_x.}
$$

The factor four is the planar extension factor: both the longitudinal viscous [stress](../../../continuum-mechanics.md#stress) and the [pressure](../../../thermodynamics.md#pressure) adjustment from transverse contraction contribute.

<a id="3/image-end-tractions-ambient-pressure-and-the-four-surface-tension-pulls-on-a-planar-liquid-sheet-slice"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-66-sheet-forces.png)

**[Figure 2](#3/image-end-tractions-ambient-pressure-and-the-four-surface-tension-pulls-on-a-planar-liquid-sheet-slice). End tractions, ambient pressure and the four surface-tension pulls on a planar liquid-sheet slice**.

For [force balance](../../../classical-mechanics.md#force-balance) on the illustrated slice, the vertical cuts give $(h\sigma_{xx})_x\,\delta x$. [Pressure](../../../thermodynamics.md#pressure) on the sloping broad faces gives $p_a h_x\,\delta x$ horizontally. Each of the two interfaces exerts a tangential [surface tension](../../../fluid-mechanics.md#surface-tension) pull at each cut, with horizontal component $\gamma\cos\theta$, where $\tan\theta=h_x/2$. Thus the horizontal [force](../../../classical-mechanics.md#force) balance is the derivative of the effective tension

$$
\mathcal T=h(\sigma_{xx}+p_a)+2\gamma\cos\theta
=4\mu h u_x+\frac\gamma2hh_{xx}+2\gamma-\frac\gamma4h_x^2
$$

to the retained small-slope order. The ambient-pressure contributions cancel in this excess tension. Differentiating cancels the two $h_xh_{xx}$ terms, leaving the [planar viscous-sheet stretching equations](../../../viscous-fluid-flow.md#planar-viscous-sheet-stretching-equations)

$$
\boxed{(4\mu h u_x)_x+\frac\gamma2h h_{xxx}=0.}
$$

The upper-face kinematic condition is $w(x,h/2,t)=(h_t+uh_x)/2$. Combining it with $w=-zu_x$ gives the second equation,

$$
\boxed{h_t+(hu)_x=0,}
$$

which is [conservation of mass](../../../continuum-mechanics.md#mass-conservation) per unit transverse width.

For the two bubbles, let $p_g$ be the common gas [pressure](../../../thermodynamics.md#pressure) and $p_e$ the surrounding liquid [pressure](../../../thermodynamics.md#pressure) away from the sheet. A cylindrical bubble has one nonzero principal curvature, so the [Young–Laplace equation](../../../fluid-mechanics.md#young-laplace-equation) gives $p_g-p_e\simeq\gamma/a$. In the nearly flat sheet the normal [stress](../../../continuum-mechanics.md#stress) is $-p_g$, giving liquid [pressure](../../../thermodynamics.md#pressure) $p_{\rm film}=p_g-2\mu u_x$. The extensional correction is small compared with $\gamma/a$ because the transition scale will satisfy $\sqrt{ah_0}/L\ll1$. Thus $p_{\rm film}\simeq p_g>p_e$, and this capillary [pressure](../../../thermodynamics.md#pressure) difference drives liquid out through both ends.

For a spatially uniform flat sheet, $h_x=h_{xxx}=0$, so the longitudinal equation gives $u_{xx}=0$. Reflection symmetry at $x=0$ selects

$$
\boxed{u(x,t)=\frac{U(t)}Lx.}
$$

Here $U$ is the outward speed at the positive end. The mass equation then gives $h_t=-Uh/L$, independent of $x$, so initially uniform thickness remains uniform. Writing it as $h_0(t)$,

$$
\boxed{\dot h_0=-\frac{U(t)}Lh_0.}
$$

The end transitions determine $U$, as derived in the following parts.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

In the short end transition, the full thickness changes by $O(h_0)$ while the curvature of each interface changes to $O(1/a)$. Since each interface has height $h/2$, the curvature scale is $O(h_0/\delta^2)$, with order-one factors irrelevant to this estimate. Therefore

$$
\boxed{\delta\sim\sqrt{ah_0}.}
$$

This is the geometric scale of the [capillary drainage of a film between two bubbles](../../../viscous-fluid-flow.md#capillary-drainage-of-a-film-between-two-bubbles). The assumed regime additionally requires $h_0\ll a$ and $\sqrt{ah_0}\ll L$, so the transition is long compared with its thickness and short compared with the flat sheet length.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Balance the two terms in the [planar viscous-sheet stretching equations](../../../viscous-fluid-flow.md#planar-viscous-sheet-stretching-equations) over the transition. The [velocity](../../../classical-mechanics.md#velocity) changes by $O(U)$ on length $\delta$, and $h_{xxx}=O(h_0/\delta^3)=O(1/(a\delta))$. Thus

$$
\frac{\mu h_0U}{\delta^2}\sim\frac{\gamma h_0}{a\delta}.
$$

Using the geometric transition length gives

$$
\boxed{U\sim\frac\gamma\mu\frac\delta a
\sim\frac\gamma\mu\sqrt{\frac{h_0}a}.}
$$

This balances capillary forcing with planar extensional [viscous stress](../../../fluid-mechanics.md#viscous-stress-tensor), not the no-slip Poiseuille resistance appropriate to a film bounded by rigid walls.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

The [conservation of mass](../../../continuum-mechanics.md#mass-conservation) equation is $h_t+(uh)_x=0$. The flat region changes on time scale $L/U$, whereas a transition has advection time $\delta/U$. Hence $h_t=O(Uh_0/L)$, and its flux change across the transition is $O(Uh_0\delta/L)$, small compared with the entering flux $Uh_0$. To leading order the transition is quasisteady and

$$
\boxed{uh=q(t)=U(t)h_0(t).}
$$

Eliminate $u=q/h$ in the longitudinal equation. Then $hu_x=-q(\log h)_x$, so

$$
hh_{xxx}=\frac{8\mu q}{\gamma}(\log h)_{xx}.
$$

Use $\xi=(x-L)/\delta$, with $\delta=\sqrt{ah_0}$, and use a prime for differentiation with respect to $\xi$. This gives the third-order equation

$$
\boxed{hh'''=B(\log h)'',\qquad B=\frac{8\mu Uh_0\sqrt{ah_0}}\gamma.}
$$

Here $h$ remains a dimensional thickness; only the longitudinal coordinate is scaled.

Match at the inner end to $h\to h_0$, $h'\to0$, $h''\to0$. Since $(hh''-h'^2/2)'=hh'''$, the first integral is

$$
hh''-\frac12h'^2=B\frac{h'}h.
$$

Divide by $h^{3/2}$ to obtain $(h'/\sqrt h)'=Bh'/h^{5/2}$. Its second integral, using the flat-film limit to fix the constant, is

$$
\boxed{h^{-1/2}\frac{dh}{d\xi}
=\frac{2B}{3h_0^{3/2}}\left[1-\left(\frac{h_0}h\right)^{3/2}\right]
=\frac{16\mu U\sqrt a}{3\gamma}\left[1-\left(\frac{h_0}h\right)^{3/2}\right].}
$$

Let $A=16\mu U\sqrt a/(3\gamma)>0$. In the overlap $h\gg h_0$, the equation gives $h'\sim A\sqrt h$, hence $h''\sim A^2/2$. The curvature of each physical interface is $h_{xx}/2\sim A^2/(4ah_0)$. Matching to the outer bubble curvature $1/a$ therefore requires $A=2\sqrt{h_0}$ and fixes the numerical coefficient:

$$
\boxed{U=\frac{3\gamma}{8\mu}\sqrt{\frac{h_0}a}.}
$$

Finally the uniform-film evolution becomes $\dot h_0=-3\gamma h_0^{3/2}/(8\mu L\sqrt a)$. If $h_0(0)=h_i$ at the start of the drainage regime, its solution is

$$
\boxed{h_0(t)=\left[h_i^{-1/2}+\frac{3\gamma}{16\mu L\sqrt a}t\right]^{-2}.}
$$

Thus [capillary drainage of a film between two bubbles](../../../viscous-fluid-flow.md#capillary-drainage-of-a-film-between-two-bubbles) gives an algebraic $t^{-2}$ decrease, and the two bubbles do not touch in finite time in this ideal model. As $h_0$ decreases, $h_0/\delta$ and $\delta/L$ become still smaller, so the geometric scale separation improves. At molecular thicknesses, [disjoining pressure](../../../viscous-fluid-flow.md#disjoining-pressure) and changes in the assumed [stress-free boundary condition](../../../viscous-fluid-flow.md#stress-free-boundary-condition) can invalidate the clean continuum-sheet description; the algebraic law alone makes no claim about that physical endpoint.

## 4

↑ **Parent:** [Paper 66](paper-66.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Take $p$ as excess [pressure](../../../thermodynamics.md#pressure) relative to the fluid far from the gap, and let $\dot h_0<0$ for approach. The lower surface of the sphere is $h_0+a-\sqrt{a^2-r^2}$ above the plane. In the dominant region $r=O(\sqrt{ah_0})\ll a$, this is the [parabolic lubrication gap](../../../viscous-fluid-flow.md#parabolic-lubrication-gap)

$$
h(r,t)=h_0+\frac{r^2}{2a}+O(r^4/a^3).
$$

Its slope is $O(\sqrt{h_0/a})\ll1$, justifying [lubrication theory](../../../viscous-fluid-flow.md#lubrication-theory). Both rigid surfaces have zero radial [velocity](../../../classical-mechanics.md#velocity), so the [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) and radial [Stokes equation](../../../stokes-flow.md#stokes-equation) give the radial [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate) per unit circumference

$$
q=-\frac{h^3}{12\mu}p_r.
$$

Axisymmetric [conservation of mass](../../../continuum-mechanics.md#mass-conservation) gives $h_t+r^{-1}(rq)_r=0$. Symmetry at $r=0$ therefore yields $q=-r\dot h_0/2$, hence $p_r=6\mu\dot h_0r/h^3$. Matching to $p\to0$ outside the pressure-bearing region gives

$$
\boxed{p=-3\mu a\dot h_0\left(h_0+\frac{r^2}{2a}\right)^{-2}.}
$$

Extending the parabolic profile to infinity in this integral is a leading-order matching device; the main [pressure](../../../thermodynamics.md#pressure) and [force](../../../classical-mechanics.md#force) come from $r=O(\sqrt{ah_0})$.

The radial scale $\sqrt{a\widehat h}$ balances the two contributions to the gap. The time scale $\widehat h/\widehat v$ is the time for a typical gap change, and the [lubrication pressure](../../../viscous-fluid-flow.md#lubrication-pressure) scale $\mu a\widehat v/\widehat h^2$ follows either from the formula above or from $p\sim\mu\widehat v\ell^2/\widehat h^3$ with $\ell^2=a\widehat h$. The elastic surface's upward displacement is $-\eta p$, so the actual gap is increased by $+\eta p$. Thus the dimensionless gap in [weakly compliant sphere-plane squeeze flow](../../../viscous-fluid-flow.md#weakly-compliant-sphere-plane-squeeze-flow) is

$$
\mathcal H=H_0+\frac{R^2}{2}+\varepsilon P,\qquad
\boxed{\varepsilon=\frac{\eta\mu a\widehat v}{\widehat h^3}.}
$$

A dot now means differentiation with respect to $T$. The dimensionless [Reynolds lubrication equation](../../../viscous-fluid-flow.md#reynolds-equation) is

$$
12\mathcal H_T=\frac1R\partial_R(R\mathcal H^3P_R).
$$

Even without fluid inertia, the elastic surface has a pressure-dependent normal [velocity](../../../classical-mechanics.md#velocity), so $\mathcal H_T$ includes $\varepsilon P_T$; omitting it would wrongly discard the acceleration term below.

Write $d=H_0+R^2/2$ and abbreviate $H=H_0$, $v=\dot H_0$, $b=\ddot H_0$ during the calculation. The rigid term is

$$
\boxed{P_0=-\frac{3v}{d^2}.}
$$

At first order the Reynolds equation gives

$$
\frac1R(Rd^3P_{1R})_R
=12P_{0T}-\frac1R(3Rd^2P_0P_{0R})_R
=-\frac{36b}{d^2}-\frac{144v^2}{d^3}+\frac{324Hv^2}{d^4}.
$$

Because $R\,dR=dd$, one integration gives

$$
Rd^3P_{1R}=2k(T)+\frac{36b}{d}+\frac{72v^2}{d^2}-\frac{108Hv^2}{d^3}.
$$

Set $\xi=R^2/(2H)$, so $d=H(1+\xi)$. Dividing and changing variables yields

$$
P_{1\xi}=\frac{k}{H^3\xi(1+\xi)^3}
+\frac{18b}{H^4\xi(1+\xi)^4}
-\frac{18v^2}{H^5\xi(1+\xi)^5}
+\frac{54v^2}{H^5(1+\xi)^6}.
$$

The first three terms are derivatives of $I_3,I_4,I_5$, respectively. Integrating from infinity to enforce $P_1\to0$ gives

$$
P_1=\frac{k}{H^3}I_3(\xi)+\frac{18b}{H^4}I_4(\xi)
-\frac{18v^2}{H^5}I_5(\xi)-\frac{54v^2}{5H^5}(1+\xi)^{-5}.
$$

The rational expansion of $I_n$ follows by differentiating $\log[\xi/(1+\xi)]+\sum_{j=1}^{n-1}[j(1+\xi)^j]^{-1}$, obtaining $1/[\xi(1+\xi)^n]$, and fixing its value to zero at infinity.

Near $\xi=0$ every $I_n$ has the same singular term $\log\xi$. Its coefficient must vanish to keep the [pressure](../../../thermodynamics.md#pressure) regular, so

$$
\frac{k}{H^3}+\frac{18b}{H^4}-\frac{18v^2}{H^5}=0,
\qquad
\boxed{k=18\left(\frac{v^2}{H^2}-\frac bH\right).}
$$

Equivalently, the integrated radial flux above must vanish at $R=0$; otherwise $P_{1R}$ would have a $1/R$ singularity. Using $I_4=I_3+[3(1+\xi)^3]^{-1}$ and $I_5=I_4+[4(1+\xi)^4]^{-1}$ cancels all logarithms and gives the simplified regular expression

$$
\boxed{P_1=\frac{6\ddot H_0}{H_0^4}(1+\xi)^{-3}
-\frac{\dot H_0^2}{H_0^5}\left[6(1+\xi)^{-3}+\frac92(1+\xi)^{-4}+\frac{54}{5}(1+\xi)^{-5}\right].}
$$

The upward hydrodynamic [force](../../../classical-mechanics.md#force) has scale $\mu a^2\widehat v/\widehat h$. Its leading contribution is [pressure](../../../thermodynamics.md#pressure) integrated over horizontal projected area; vertical shear [forces](../../../classical-mechanics.md#force) are smaller in the lubrication limit. Thus $F=2\pi\int_0^\infty(P_0+\varepsilon P_1+\cdots)R\,dR$. Use $R\,dR=H_0\,d\xi$ and $\int_0^\infty(1+\xi)^{-n}\,d\xi=1/(n-1)$. The two contributions are

$$
2\pi\int P_0R\,dR=-\frac{6\pi\dot H_0}{H_0},\qquad
2\pi\int P_1R\,dR=6\pi\left(\frac{\ddot H_0}{H_0^3}-\frac{12}{5}\frac{\dot H_0^2}{H_0^4}\right).
$$

Therefore

$$
\boxed{F=6\pi\left[-\frac{\dot H_0}{H_0}+\varepsilon\left(\frac{\ddot H_0}{H_0^3}-\frac{12}{5}\frac{\dot H_0^2}{H_0^4}\right)+\cdots\right].}
$$

For weight-controlled sedimentation, let the fixed effective load be $F=6\pi A$, $A>0$, and neglect particle inertia as well as fluid inertia. At leading order $\dot H_0=-AH_0$ and $\ddot H_0=A^2H_0$. The first-order bracket evaluated on this trajectory is $-(7/5)A^2/H_0^2$. Solving the [force](../../../classical-mechanics.md#force) balance perturbatively therefore gives

$$
\boxed{\dot H_0=-AH_0-\varepsilon\frac{7A^2}{5H_0}+O(\varepsilon^2).}
$$

Hence **weak compliance initially increases the sedimentation speed** in the regime where the perturbation is valid. The squeeze [pressure](../../../thermodynamics.md#pressure) indents the coating away from the sphere, widens the flow passage and lowers resistance. This is a load-controlled conclusion on the slow sedimenting branch, not a claim about an arbitrary externally imposed acceleration at startup.

The [load-controlled breakdown of weak squeeze-flow compliance](../../../viscous-fluid-flow.md#load-controlled-breakdown-of-weak-squeeze-flow-compliance) occurs when the relative correction $O(\varepsilon A/H_0^2)$ becomes order one:

$$
\boxed{H_0^*\sim\sqrt{\varepsilon A},\qquad H_0^*\sim\sqrt\varepsilon\ \hbox{for }A=O(1).}
$$

The central rigid [pressure](../../../thermodynamics.md#pressure) has size $P_0(0)\sim A/H_0$, so the relative elastic gap change is also $\varepsilon P_0(0)/H_0\sim\varepsilon A/H_0^2$. Thus breakdown means that elastic deflection is comparable with the nominal undeformed gap. The regular expansion about a rigid plane then ceases to be uniform and the coupled elastic-lubrication problem must be retained. It does not by itself imply contact, fluid inertia or failure of the thin-gap geometry.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
