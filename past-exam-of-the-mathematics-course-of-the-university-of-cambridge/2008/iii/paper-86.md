# Paper 86

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper86.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper86.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 86](paper-86.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Work in the laboratory frame, with fluid at rest at infinity and the instantaneous [sphere](../../../geometry-and-topology.md#sphere) centre at the origin. In the [Unscaled Papkovich–Neuber representation](../../../stokes-flow.md#unscaled-papkovich-neuber-representation), take the harmonic potentials

$$
\mathbf A=-\frac{3a}{4r}\mathbf V,\qquad\phi=\frac{a^3}{4r^3}(\mathbf V\cdot\mathbf x),\qquad r=|\mathbf x|.
$$

Differentiating the two terms gives the [translating sphere in Stokes flow](../../../stokes-flow.md#translating-sphere-in-stokes-flow):

$$
\boxed{\mathbf u=\frac{3a}{4r}(I+\mathbf n\mathbf n)\mathbf V+\frac{a^3}{4r^3}(I-3\mathbf n\mathbf n)\mathbf V,\qquad p-p_\infty=\frac{3\mu a}{2r^2}\mathbf V\cdot\mathbf n.}
$$

Here $\mathbf n=\mathbf x/r$. The potentials are harmonic outside the [sphere](../../../geometry-and-topology.md#sphere), so they satisfy the [Stokes equations](../../../stokes-flow.md#stokes-equation). At $r=a$, the two coefficients of $\mathbf n\mathbf n$ cancel and the coefficient of $I$ is one, proving the [no-slip boundary condition](../../../viscous-fluid-flow.md#no-slip-boundary-condition) $\mathbf u=\mathbf V$; the field decays at infinity. Its leading part is a [Stokeslet](../../../stokes-flow.md#stokeslet) of [force](../../../classical-mechanics.md#force) $6\pi\mu a\mathbf V$ exerted on the fluid.

Let $\widehat{\mathbf z}$ point upwards, $\delta=V_1-V_2$, and $D=a_2V_2-a_1V_1$. Each isolated [sphere](../../../geometry-and-topology.md#sphere) moves with [velocity](../../../classical-mechanics.md#velocity) $-V_i\widehat{\mathbf z}$. To leading order its correction is the other's incident [Stokeslet](../../../stokes-flow.md#stokeslet) [velocity](../../../classical-mechanics.md#velocity):

$$
\dot{\mathbf x}_1=-V_1\widehat{\mathbf z}-\frac{3a_2V_2}{4r}(I+\mathbf n\mathbf n)\widehat{\mathbf z},\qquad\dot{\mathbf x}_2=-V_2\widehat{\mathbf z}-\frac{3a_1V_1}{4r}(I+\mathbf n\mathbf n)\widehat{\mathbf z}.
$$

The [forces](../../../classical-mechanics.md#force) generating these fields are the fixed sedimenting loads, so their leading strengths are set by the isolated speeds. Subtraction yields the [leading interaction of two sedimenting spheres](../../../stokes-flow.md#leading-interaction-of-two-sedimenting-spheres):

$$
\boxed{\dot{\mathbf r}=-\delta\widehat{\mathbf z}-\frac{3D}{4r}(I+\mathbf n\mathbf n)\widehat{\mathbf z}.}
$$

Since $\widehat{\mathbf z}=\cos\theta\,\widehat{\mathbf r}-\sin\theta\,\widehat{\boldsymbol\theta}$, this reduces to

$$
\boxed{\dot r=-\left(\delta+\frac{3D}{2r}\right)\cos\theta,\qquad r\dot\theta=\left(\delta+\frac{3D}{4r}\right)\sin\theta.}
$$

The stipulated higher-order errors can be appended to both equations; they do not enter this leading calculation.

For the same-sign case, interchange labels if necessary to arrange $\delta>0,D>0$, and put $c=3D/4$. The vertical separation $z=r\cos\theta$ satisfies

$$
\dot z=-\delta-\frac c r(1+\cos^2\theta)\leq-\delta.
$$

If [sphere](../../../geometry-and-topology.md#sphere) one is initially above [sphere](../../../geometry-and-topology.md#sphere) two, its vertical order reverses; in every case $z\to-\infty$, implying $r\to\infty$. For a noncollinear trajectory there is no collision in the point-force equations. Indeed, divide the two polar equations and integrate:

$$
\frac{\delta r+c}{r(\delta r+2c)}dr=-\cot\theta\,d\theta,\qquad\boxed{r(\delta r+2c)\sin^2\theta=C>0.}
$$

At side-by-side passage, $\theta=\pi/2$, the closest separation is the positive root of $\delta r^2+2cr=C$. Before passage $\dot r<0$ and after passage $\dot r>0$, proving overtaking and unbounded subsequent separation. This [passing invariant for unequal point-force spheres](../../../stokes-flow.md#passing-invariant-for-unequal-point-force-spheres) describes a physical far-field passage only when the closest separation also greatly exceeds the [sphere](../../../geometry-and-topology.md#sphere) radii. Exactly collinear approach instead reaches the near-contact regime, where this leading approximation cannot describe two finite [spheres](../../../geometry-and-topology.md#sphere) passing through one another.

For opposite signs, choose $\delta>0,D<0$ and consider the invariant configuration with [sphere](../../../geometry-and-topology.md#sphere) one vertically above [sphere](../../../geometry-and-topology.md#sphere) two, $\theta=0$. The radial equation is

$$
\dot r=-\delta+\frac{3|D|}{2r}=\delta\left(\frac{r_*}{r}-1\right),\qquad\boxed{r_*=-\frac{3D}{2\delta}.}
$$

If $r>r_*$, separation decreases; if $r<r_*$, it increases. Thus it approaches this [equilibrium](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) along the vertical line. [Linearization](../../../algebra.md#linearization) gives $\dot{\delta r}=-(\delta/r_*)\delta r$. But a small tilt obeys $\dot\theta=(\delta/(2r_*))\theta$, so the [vertical bound pair in the point-force sedimentation model](../../../stokes-flow.md#vertical-bound-pair-in-the-point-force-sedimentation-model) is stable only against vertical perturbations and is a saddle in the full separation dynamics. The opposite vertical orientation has the reversed stability. Reversing gravity reverses both $\delta$ and $D$, leaves $r_*$ unchanged, and reverses every trajectory; radial attraction becomes repulsion. This is fully consistent with [kinematic reversibility of Stokes flow](../../../stokes-flow.md#kinematic-reversibility-of-stokes-flow).

There is an important restriction in the printed data. Its hierarchy $|D|\ll(a_1+a_2)|\delta|$ implies $r_*\ll a_1+a_2$, so the proposed [equilibrium](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) would overlap the physical [spheres](../../../geometry-and-topology.md#sphere) and lie outside the well-separated approximation. **With that hierarchy there is no justified physical far-field bound pair.** The intended far-field [equilibrium](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) instead requires the first inequality reversed, $|D|\gg(a_1+a_2)|\delta|$. The formal [equilibrium](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) and its vertical stability above show the intended mechanism, while also identifying the missing validity and transverse-stability qualifications.

## 2

↑ **Parent:** [Paper 86](paper-86.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a [force](../../../classical-mechanics.md#force) $\mathbf F\delta(\mathbf x)$ acting on an unbounded incompressible fluid, the [Stokeslet](../../../stokes-flow.md#stokeslet) and its [pressure](../../../thermodynamics.md#pressure) are

$$
\boxed{u_i(\mathbf x)=G_{ij}(\mathbf x)F_j,\quad G_{ij}=\frac1{8\pi\mu}\left(\frac{\delta_{ij}}r+\frac{x_ix_j}{r^3}\right),\quad p=\frac{\mathbf F\cdot\mathbf x}{4\pi r^3}.}
$$

They solve $-\nabla p+\mu\nabla^2\mathbf u+\mathbf F\delta=0$ and $\nabla\cdot\mathbf u=0$. Approximate a slender body by a line distribution of these point [forces](../../../classical-mechanics.md#force) on its centreline. At a point labelled by arclength $s$,

$$
\dot{\mathbf X}(s)\simeq\int G(\mathbf X(s)-\mathbf X(s'))\mathbf f(s')\,ds'.
$$

To extract the large logarithm, write $s'=s+\ell$ and approximate $\mathbf X(s+\ell)-\mathbf X(s)\simeq\ell\mathbf t$, $\mathbf f(s+\ell)\simeq\mathbf f(s)$, where $\mathbf t=\mathbf X'$ is the unit [tangent vector](../../../differential-geometry.md#tangent-vector). The near-line contribution has kernel $(I+\mathbf t\mathbf t)/(8\pi\mu|\ell|)$. Cut it off at the wire radius $R$ and a macroscopic length $L$. The two sides of the line give

$$
\dot{\mathbf X}\sim\frac{\ln(L/R)}{4\pi\mu}(I+\mathbf t\mathbf t)\mathbf f.
$$

The far contribution and changes in the cutoff add terms without the leading logarithm. Since $(I+\mathbf t\mathbf t)^{-1}=I-\mathbf t\mathbf t/2$, inversion proves the leading [slender-body force density](../../../stokes-flow.md#slender-body-force-density)

$$
\boxed{\mathbf f\sim\frac{2\pi\mu}{\ln(L/R)}(2I-\mathbf t\mathbf t)\dot{\mathbf X}.}
$$

This is [force](../../../classical-mechanics.md#force) on the fluid; the fluid's [force](../../../classical-mechanics.md#force) on the wire has the opposite sign. It gives twice the resistance to transverse motion as to tangential motion at this order.

The stated arclength describes the circular [helix](../../../topology.md#helix) $\mathbf X=(a\cos\theta,a\sin\theta,b\theta)$. The PDF omits the second $a$ in the coordinates, so the literal printed curve and its arclength are inconsistent unless $a=1$. First use the circular interpretation consistent with the given arclength. Put $q=\sqrt{a^2+b^2}$ and $c=2\pi\mu/\ln(L/R)$. Then

$$
\mathbf t=\frac{(-a\sin\theta,a\cos\theta,b)}q,\qquad ds=q\,d\theta.
$$

Rotation about $z$ has [velocity](../../../classical-mechanics.md#velocity) $\mathbf v=\Omega(-a\sin\theta,a\cos\theta,0)$, so $\mathbf t\cdot\mathbf v=\Omega a^2/q$. The axial [force](../../../classical-mechanics.md#force) density is $f_z=-c\Omega a^2b/q^2$. Integrating over one turn gives

$$
\boxed{F_z^{\rm rotation}=-\frac{4\pi^2\mu a^2b}{\ln(L/R)\sqrt{a^2+b^2}}\,\Omega.}
$$

For translation, $\mathbf v=W\widehat{\mathbf z}$ and $\mathbf f=cW(2\widehat{\mathbf z}-(b/q)\mathbf t)$. Only the tangential term contributes to axial couple. Since $(\mathbf X\times\mathbf t)_z=a^2/q$, its density is $-cWa^2b/q^2$, giving

$$
\boxed{G_z^{\rm translation}=-\frac{4\pi^2\mu a^2b}{\ln(L/R)\sqrt{a^2+b^2}}\,W.}
$$

These are the off-diagonal coefficients of the [axial resistance matrix of a slender helix](../../../stokes-flow.md#axial-resistance-matrix-of-a-slender-helix). Their equality does not depend on this particular geometry: with symmetric local resistance $D=c(2I-\mathbf t\mathbf t)$, the rotation-induced axial [force](../../../classical-mechanics.md#force) is $\int\widehat{\mathbf z}\cdot D(\widehat{\mathbf z}\times\mathbf X)ds$, whereas the translation-induced axial [torque](../../../classical-mechanics.md#torque) is $\int(\widehat{\mathbf z}\times\mathbf X)\cdot D\widehat{\mathbf z}\,ds$. They agree pointwise by [symmetry](../../../physics.md#symmetry-physics) of $D$. The full Stokes-flow statement is the [Lorentz reciprocal theorem](../../../stokes-flow.md#lorentz-reciprocal-theorem-for-stokes-flow).

For completeness, retaining the literal elliptic [helix](../../../topology.md#helix) instead gives $s'=\sqrt{a^2\sin^2\theta+\cos^2\theta+b^2}$ and the [axial coupling of an elliptic helix](../../../stokes-flow.md#axial-coupling-of-an-elliptic-helix)

$$
\boxed{\frac{F_z}{\Omega}=\frac{G_z}{W}=-\frac{2\pi\mu ab}{\ln(L/R)}\int_{-\pi}^{\pi}\frac{d\theta}{\sqrt{a^2\sin^2\theta+\cos^2\theta+b^2}}.}
$$

Thus reciprocity holds for the literal curve as well; only the geometric coefficient and arclength change. In all these formulas the equal and opposite [force](../../../classical-mechanics.md#force) or couple on the wire reverses the displayed sign.

## 3

↑ **Parent:** [Paper 86](paper-86.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The leading disturbance in [sphere](../../../geometry-and-topology.md#sphere) [Stokes flow](../../../stokes-flow.md) has size $u\sim Ua/r$. Consequently viscous [diffusion](../../../thermodynamics.md#diffusion) has size $\nu u/r^2$, background [advection](../../../fluid-mechanics.md#advection) has size $Uu/r$, and their ratio is $Ur/\nu$. Even if the [sphere](../../../geometry-and-topology.md#sphere) [Reynolds number](../../../fluid-mechanics.md#reynolds-number) $Ua/\nu$ is small, this ratio becomes order one at $r\sim\nu/U$. Thus **the Stokes approximation is nonuniform at distances of order $\nu/U$**. At that outer distance the disturbance itself is small relative to $U$, so self-convection is smaller than background [advection](../../../fluid-mechanics.md#advection) and the [Oseen approximation](../../../stokes-flow.md#oseen-approximation) is appropriate:

$$
\boxed{\rho\mathbf U\cdot\nabla\mathbf u=-\nabla p+\mu\nabla^2\mathbf u,\qquad\nabla\cdot\mathbf u=0.}
$$

Write $\mathbf u=\nabla\phi+\nu\nabla\chi-\mathbf U\chi$. It is sufficient outside the origin to impose $\Delta\phi=0$ and $(\nu\Delta-\mathbf U\cdot\nabla)\chi=0$: these give zero [divergence](../../../calculus.md#divergence), and substitution into [momentum](../../../classical-mechanics.md#momentum) gives $p=-\rho\mathbf U\cdot\nabla\phi$. With $\chi=h e^{\mathbf U\cdot\mathbf x/(2\nu)}$, differentiation yields

$$
(\nu\Delta-\mathbf U\cdot\nabla)\chi=\nu e^{\mathbf U\cdot\mathbf x/(2\nu)}\left(\Delta h-\frac{U^2}{4\nu^2}h\right),\qquad U=|\mathbf U|.
$$

A decaying radial choice is $h=C e^{-Ur/(2\nu)}/r$. Therefore

$$
\chi=\frac C r\exp\left(\frac{\mathbf U\cdot\mathbf x-Ur}{2\nu}\right).
$$

The exponent is nonpositive, so this scalar decays at infinity, including as $1/r$ directly downstream. In the overlap $a\ll r\ll\nu/U$,

$$
\chi=\frac C r+\frac C{2\nu}\frac{\mathbf U\cdot\mathbf x}{r}-\frac{CU}{2\nu}+\cdots.
$$

Choosing $\phi=-\nu C/r$ cancels the first term's [gradient](../../../calculus.md#gradient) in $\nabla\phi+\nu\nabla\chi$. The remaining leading [velocity](../../../classical-mechanics.md#velocity) is

$$
\mathbf u\sim\frac C2\nabla\left(\frac{\mathbf U\cdot\mathbf x}{r}\right)-\frac C r\mathbf U=-\frac C{2r}\left[\mathbf U+\mathbf n(\mathbf U\cdot\mathbf n)\right].
$$

Matching fixes $C=3a/2$. Thus the [potential-source and wake decomposition of sphere Oseen flow](../../../stokes-flow.md#potential-source-and-wake-decomposition-of-sphere-oseen-flow) is

$$
\boxed{\phi=-\frac{3a\nu}{2r},\qquad\chi=\frac{3a}{2r}e^{(\mathbf U\cdot\mathbf x-Ur)/(2\nu)},\qquad\mathbf u=\nabla\phi+\nu\nabla\chi-\mathbf U\chi.}
$$

Its [pressure](../../../thermodynamics.md#pressure) is $p=-3\mu a(\mathbf U\cdot\mathbf x)/(2r^3)$, the sign appropriate to a fixed [sphere](../../../geometry-and-topology.md#sphere) in an incident flow. The [velocity](../../../classical-mechanics.md#velocity) decays in every direction and matches the requested leading inner disturbance; the [sphere](../../../geometry-and-topology.md#sphere)'s potential-dipole term enters a higher matching order.

The scalar potential is a [point source](../../../fluid-mechanics.md#point-source): $\nabla\phi=(3a\nu/2)\mathbf x/r^3$, so [integration](../../../calculus.md#integral) over a centred [sphere](../../../geometry-and-topology.md#sphere) gives

$$
\boxed{Q_{\rm source}=\int\nabla\phi\cdot\mathbf n\,dS=6\pi\nu a,\qquad\dot M_{\rm source}=\rho Q_{\rm source}=6\pi\mu a.}
$$

To see the [fluid wake](../../../fluid-mechanics.md#wake-physics), take $z$ downstream along $\mathbf U$ and transverse radius $R_\perp$. For $z\gg\nu/U$, $r-z\simeq R_\perp^2/(2z)$, giving

$$
\chi\simeq\frac{3a}{2z}\exp\left(-\frac{UR_\perp^2}{4\nu z}\right),\qquad u_z\simeq-U\chi.
$$

The [fluid wake](../../../fluid-mechanics.md#wake-physics) is concentrated within $R_\perp=O(\sqrt{\nu z/U})$. Its integrated mass deficit is $\rho U\int\chi\,dA\simeq6\pi\mu a$, balancing the outward potential-source [mass flux](../../../physics.md#mass-flux). The corresponding [momentum](../../../classical-mechanics.md#momentum) deficit is

$$
\boxed{\rho U^2\int\chi\,dA\simeq6\pi\mu aU,}
$$

which equals the leading [sphere](../../../geometry-and-topology.md#sphere) drag. The [Gaussian integral](../../../calculus.md#gaussian-integral) used here is $\int_0^\infty e^{-UR_\perp^2/(4\nu z)}2\pi R_\perp dR_\perp=4\pi\nu z/U$.

The PDF labels $6\pi\mu aU$ as the mass-source strength, but this has dimensions of [force](../../../classical-mechanics.md#force). **The actual mass-source strength is $6\pi\mu a$; $6\pi\mu aU$ is the [momentum](../../../classical-mechanics.md#momentum) deficit or drag.** The decomposition above supplies both quantities and identifies the printed normalization error.

## 4

↑ **Parent:** [Paper 86](paper-86.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

First solve the hinted fixed-gap problem. Let $y$ measure distance across the gap and $H(x)=h+x^2/(2a)$ be its leading local height. The [lubrication approximation](../../../viscous-fluid-flow.md#lubrication-theory) gives $\mu u_{yy}=p_x$, with $u=0$ at $y=0,H$, so

$$
u=-\frac{p_x}{2\mu}y(H-y),\qquad q=\int_0^H u\,dy=-\frac{H^3p_x}{12\mu}.
$$

The constant flux per unit transverse length is $q$. Integrating its [pressure](../../../thermodynamics.md#pressure) [gradient](../../../calculus.md#gradient) gives the [pressure-driven flux through a parabolic lubrication gap](../../../viscous-fluid-flow.md#pressure-driven-flux-through-a-parabolic-lubrication-gap):

$$
\Delta p=12\mu q\int_{-\infty}^{\infty}\frac{dx}{(h+x^2/(2a))^3}.
$$

With $x=\sqrt{2ah}\,t$, the [integral](../../../calculus.md#integral) is $\sqrt{2a}\,h^{-5/2}\int_{-\infty}^{\infty}(1+t^2)^{-3}dt$. The substitution $t=\tan\chi$ gives $\int_{-\pi/2}^{\pi/2}\cos^4\chi\,d\chi=3\pi/8$, and therefore

$$
\boxed{\Delta p=\frac{9\pi\mu q\sqrt{2a}}{2h^{5/2}}.}
$$

Now take the [sphere](../../../geometry-and-topology.md#sphere) speed to be $U>0$ downwards and assume zero net liquid through-flow, so the displaced liquid must pass through the annular gap. Near the equator, the [sphere](../../../geometry-and-topology.md#sphere)'s surface radius is $R-z^2/(2R)+\cdots$, giving $H(z)=d+z^2/(2R)$. In the [sphere](../../../geometry-and-topology.md#sphere) frame the relative [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate) is $U\pi(R+d)^2$; dividing by circumference $2\pi R$ gives $q\simeq UR/2$. The Couette contribution from the moving tube wall is only order $Ud$, smaller by $d/R$, so the fixed-gap [pressure](../../../thermodynamics.md#pressure) result gives

$$
\Delta p\simeq\frac{9\pi\mu UR\sqrt{2R}}{4d^{5/2}}.
$$

The [pressure](../../../thermodynamics.md#pressure) changes principally within axial distance $\sqrt{Rd}$ around the equator. It is nearly constant on each hemisphere, so its leading [force](../../../classical-mechanics.md#force) is the [pressure](../../../thermodynamics.md#pressure) difference times projected area, $F_p\simeq\pi R^2\Delta p$. Direct viscous shear contributes a relative order $d/R$ and is smaller. Balance with the buoyant weight:

$$
\frac{4\pi R^3}{3}\Delta\rho g\simeq\pi R^2\frac{9\pi\mu UR\sqrt{2R}}{4d^{5/2}}.
$$

Thus the [settling speed of a nearly occluding sphere without through-flow](../../../viscous-fluid-flow.md#settling-speed-of-a-nearly-occluding-sphere-without-through-flow) is

$$
\boxed{U\sim\frac{8\sqrt2\,\Delta\rho g d^2}{27\pi\mu}\left(\frac dR\right)^{1/2}.}
$$

The printed speed lacks the factor $1/\pi$. The parabolic-gap [integral](../../../calculus.md#integral) above fixes the normalization: its $3\pi/8$ cannot be dropped. With standard [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity) and [Stokes drag law](../../../stokes-flow.md#stokes-s-law) conventions, **the requested coefficient must be corrected by dividing the printed expression by $\pi$**. Also, the bypass result assumes no net through-flow; allowing a piston-like displacement of the entire fluid column would require specifying tube end conditions and a different resistance balance.

A [sphere](../../../geometry-and-topology.md#sphere) of radius $d$ in an unbounded fluid has sedimentation speed $U_d=2\Delta\rho gd^2/(9\mu)$. Therefore

$$
\boxed{\frac U{U_d}\sim\frac{4\sqrt2}{3\pi}\left(\frac dR\right)^{1/2}\ll1.}
$$

The large confined [sphere](../../../geometry-and-topology.md#sphere) falls much more slowly even than this much smaller unconfined [sphere](../../../geometry-and-topology.md#sphere).

For radial offset $e<d$, let $\epsilon=e/d$. To leading order the narrowest gap varies as $d(\phi)=d(1+\epsilon\cos\phi)$. All circumferential strips share the same [pressure](../../../thermodynamics.md#pressure) drop and act as parallel channels. Inverting the gap-resistance formula shows that each carries flux proportional to $d(\phi)^{5/2}\Delta p$. At fixed buoyant load, the leading [pressure](../../../thermodynamics.md#pressure) drop is fixed, so the speed ratio is

$$
\boxed{\frac{U(e)}{U(0)}\simeq\frac1{2\pi}\int_0^{2\pi}(1+\epsilon\cos\phi)^{5/2}d\phi>1\quad(0<\epsilon<1).}
$$

The [eccentricity increases narrow-gap bypass mobility](../../../viscous-fluid-flow.md#eccentricity-increases-narrow-gap-bypass-mobility) result holds because the gain through the wider side outweighs the loss through the narrower side. Strict [convexity](../../../real-analysis.md#convex-function) of $x^{5/2}$ and the zero mean of cosine prove the inequality. Pairing the positive- and negative-cosine contributions in the derivative proves monotonicity with offset. The broader hint's assertion for every exponent $\alpha>0$ is not correct for $0<\alpha<1$, when [concavity](../../../real-analysis.md#concave-function) reverses the inequality; the required exponent $5/2$ is in the valid convex range.

## 5

↑ **Parent:** [Paper 86](paper-86.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

Let $\rho$ be the liquid density and neglect atmospheric shear. The shallow-channel [lubrication approximation](../../../viscous-fluid-flow.md#lubrication-theory) makes the surface nearly horizontal in each cross-section, at $z=h(x,t)$, with [hydrostatic pressure](../../../fluid-mechanics.md#hydrostatic-pressure) $p=p_{\rm atm}+\rho g(h-z)$. At fixed $y$, the floor is $z_b=\alpha|y|$ and the local liquid thickness is $H_y=h-z_b$. Axial [momentum](../../../classical-mechanics.md#momentum) and [boundary conditions](../../../differential-equation.md#boundary-condition) are

$$
\mu u_{zz}=\rho g h_x,\qquad u(z_b)=0,\qquad u_z(h)=0.
$$

Writing $\zeta=z-z_b$, [integration](../../../calculus.md#integral) gives

$$
u=-\frac{\rho gh_x}{2\mu}(2H_y\zeta-\zeta^2),\qquad q(y)=\int_{z_b}^h u\,dz=-\frac{\rho g}{3\mu}H_y^3h_x.
$$

The wetted interval is $|y|<h/\alpha$. Its cross-sectional area and total axial flux are

$$
A=2\int_0^{h/\alpha}(h-\alpha y)dy=\frac{h^2}{\alpha},\qquad Q=-\frac{2\rho gh_x}{3\mu}\int_0^{h/\alpha}(h-\alpha y)^3dy=-\frac{\rho g}{6\mu\alpha}h^4h_x.
$$

The [shallow V-channel lubrication flux](../../../reduced-gravity.md#shallow-v-channel-lubrication-flux) and [volume conservation](../../../physics.md#volume-conservation) $A_t+Q_x=0$ therefore give

$$
\boxed{(h^2)_t=C(h^4h_x)_x,\qquad C=\frac{\rho g}{6\mu},\qquad\frac1\alpha\int_{\mathbb R}h^2dx=V.}
$$

The slope $\alpha\ll1$ makes transverse shear small relative to vertical shear; the longitudinal current must also be slender for this reduction.

For typical height $H$ and axial length $L$, fixed volume gives $H^2L\sim\alpha V$, while the equation gives $L^2\sim CH^3t$. Eliminating either scale yields

$$
\boxed{H\sim\left(\frac{\alpha^2V^2}{Ct}\right)^{1/7},\qquad L\sim(Ct)^{2/7}(\alpha V)^{3/7}.}
$$

Thus the current grows in length like $t^{2/7}$ and thins like $t^{-1/7}$. Equivalently, the [porous-medium transformation of V-channel spreading](../../../reduced-gravity.md#porous-medium-transformation-of-v-channel-spreading) sets $w=h^2$ and gives $w_t=(C/5)(w^{5/2})_{xx}$ with constant mass $\alpha V$.

Seek a symmetric solution $h=t^{-1/7}f(\xi)$ with $\xi=x/t^{2/7}$. Substitution into the conservative depth equation gives

$$
-\frac27 f^2-\frac27\xi(f^2)'=C(f^4f')'.
$$

The left side is $-(2/7)(\xi f^2)'$. [Symmetry](../../../physics.md#symmetry-physics) sets the [integration](../../../calculus.md#integral) constant to zero, so $Cf^4f'=-(2/7)\xi f^2$ within the [support](../../../function.md#support). Integrating $f^2f'=-2\xi/(7C)$ gives $f^3=3(\xi_0^2-\xi^2)/(7C)$. In physical variables the [constant-volume similarity in a V-shaped channel](../../../reduced-gravity.md#constant-volume-similarity-in-a-v-shaped-channel) is

$$
\boxed{h(x,t)=\left[\frac{3(X(t)^2-x^2)}{7Ct}\right]_+^{1/3},}
$$

where $X(t)$ is the half-length of its [support](../../../function.md#support) and the [positive part](../../../function.md#positive-part-of-a-real-valued-function) makes $h=0$ outside it.

Define the positive normalization

$$
J=\int_{-1}^1(1-s^2)^{2/3}ds=\int_0^\pi\sin^{7/3}\theta\,d\theta=\frac{\sqrt\pi\,\Gamma(5/3)}{\Gamma(13/6)}.
$$

The first substitution is $s=\cos\theta$; the gamma form follows from the [beta function](../../../complex-analysis.md#beta-function) [integral](../../../calculus.md#integral). Conservation of volume now gives

$$
\alpha V=\left(\frac3{7Ct}\right)^{2/3}X^{7/3}J,
$$

and consequently

$$
\boxed{X(t)=\left(\frac{\alpha V}{J}\right)^{3/7}\left(\frac{7Ct}{3}\right)^{2/7},\qquad h(0,t)=\left(\frac{\alpha V}{J}\right)^{2/7}\left(\frac3{7Ct}\right)^{1/7}.}
$$

The full current length is $2X(t)$. Its flux vanishes at the two noses, since the integrated similarity equation gives $Ch^4h_x=-2xh^2/(7t)$ there, so no volume is lost at the [support](../../../function.md#support) boundary. A shifted origin or a positive shift of time gives the corresponding translated similarity family.

In an intended trigonometric $I(\beta)$ notation, $J=I(7/3)$ requires either cosine integrated over $[-\pi/2,\pi/2]$ or absolute cosine over $[0,\pi]$. The printed $\cos^\beta\theta$ on $[0,\pi]$ is not a positive real normalization for the required fractional exponent: with a real cube-root interpretation at $\beta=7/3$, its two halves cancel, while the principal complex power is not real. **The similarity normalization uses the positive sine [integral](../../../calculus.md#integral) $J$ above.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
