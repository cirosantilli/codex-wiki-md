# Paper 78

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper78.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper78.pdf)

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
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 78](paper-78.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For a fixed fluid domain with prescribed [velocity](../../../classical-mechanics.md#velocity) on its whole boundary, the [Minimum-dissipation theorem for Stokes flow](../../../stokes-flow.md#minimum-dissipation-theorem-for-stokes-flow) compares the actual incompressible [Stokes flow](../../../stokes-flow.md) $u$ with every admissible incompressible [velocity](../../../classical-mechanics.md#velocity) field $v$ having the same boundary values. The trial fields need not themselves satisfy the momentum equation. With $e(u)=(\nabla u+\nabla u^T)/2$ and constant [dynamic viscosity](../../../fluid-mechanics.md#dynamic-viscosity) $\mu$, define the [viscous dissipation](../../../stokes-flow.md#viscous-dissipation)

$$
\mathcal D[u]=2\mu\int e(u):e(u)\,dV.
$$

Assume no nonconservative body force, or absorb a conservative force into the [pressure](../../../thermodynamics.md#pressure). Set $w=v-u$, so $\nabla\cdot w=0$ and $w=0$ on the boundary. The Stokes [stress tensor](../../../continuum-mechanics.md#cauchy-stress-tensor) $\sigma=-pI+2\mu e(u)$ obeys $\nabla\cdot\sigma=0$. Because [pressure](../../../thermodynamics.md#pressure) has zero contraction with $e(w)$,

$$
2\mu\int e(u):e(w)\,dV=\int\sigma:\nabla w\,dV=\int_{\partial V}w\cdot\sigma n\,dS-\int_Vw\cdot(\nabla\cdot\sigma)\,dV=0.
$$

Expanding the square proves

$$
\boxed{\mathcal D[v]=\mathcal D[u]+2\mu\int e(w):e(w)\,dV\geq\mathcal D[u].}
$$

Equality requires $e(w)=0$, so $w$ is a rigid motion; the homogeneous boundary values force it to vanish. The theorem concerns fixed boundary velocities, not fixed applied forces or arbitrary comparisons between different fluid domains.

For the concentric-sphere motion, seek $u=F(r)\boldsymbol\Omega\times x$. Incompressibility is automatic. The choice $F=A+B/r^3$ gives a harmonic [velocity](../../../classical-mechanics.md#velocity): the linear term is harmonic, and each component of $x/r^3$ is a derivative of the harmonic function $1/r$. The no-slip conditions $F(a)=1$, $F(b)=0$ give

$$
B=\frac{a^3b^3}{b^3-a^3},\qquad A=-\frac{a^3}{b^3-a^3}.
$$

Thus the [Rotational Stokes flow between concentric spheres](../../../stokes-flow.md#rotational-stokes-flow-between-concentric-spheres) is

$$
\boxed{u(x)=\frac{a^3}{b^3-a^3}\left(\frac{b^3}{r^3}-1\right)\boldsymbol\Omega\times x.}
$$

It satisfies the Stokes equation with constant [pressure](../../../thermodynamics.md#pressure), and the uniqueness implied by the theorem identifies it as the required flow.

In the [Unscaled Papkovich–Neuber representation](../../../stokes-flow.md#unscaled-papkovich-neuber-representation), take $\Phi=-u/2$ and $\chi=0$. Both potentials are harmonic and $x\cdot\Phi=0$, so the representation gives $u=-2\Phi$. Also

$$
\nabla\cdot\Phi=-\tfrac12\{\nabla F\cdot(\boldsymbol\Omega\times x)+F\nabla\cdot(\boldsymbol\Omega\times x)\}=0,
$$

and therefore **$p=0$**, after choosing the arbitrary [pressure](../../../thermodynamics.md#pressure) constant.

This [pressure](../../../thermodynamics.md#pressure) conclusion also follows from symmetry and [Linearity of Stokes flow](../../../stokes-flow.md#linearity-of-stokes-flow). [Pressure](../../../thermodynamics.md#pressure) is a scalar linear in the axial vector $\boldsymbol\Omega$, and isotropy leaves only a possible term proportional to $\boldsymbol\Omega\cdot x$. That is a pseudoscalar, forbidden by reflection symmetry of the concentric spherical domain. Hence the [pressure](../../../thermodynamics.md#pressure) perturbation vanishes. Equivalently, axisymmetry and reflection with flow reversal make the motion purely azimuthal, while its meridional momentum balance has no [pressure](../../../thermodynamics.md#pressure) gradient.

Let $v=\boldsymbol\Omega\times x$ in the following stress calculation. The symmetric [velocity](../../../classical-mechanics.md#velocity) gradient is

$$
e_{ij}=\frac{F'(r)}{2r}(x_jv_i+x_iv_j),\qquad F'=-\frac{3B}{r^4}.
$$

The full [stress tensor](../../../continuum-mechanics.md#cauchy-stress-tensor), in the zero-[pressure](../../../thermodynamics.md#pressure) gauge, is therefore

$$
\boxed{\sigma_{ij}=-\frac{3\mu B}{r^5}(x_jv_i+x_iv_j).}
$$

For $n=x/r$, the traction on a radial surface is $\sigma n=-3\mu B(\boldsymbol\Omega\times n)/r^3$. This completely specifies the stress field; with the polar axis along $\boldsymbol\Omega$, its only nonzero spherical shear component is $\sigma_{r\phi}=-3\mu B\Omega\sin\theta/r^3$.

The fluid couple on the inner sphere is the integral of $x\times\sigma n$ with the normal pointing from the solid into the fluid. Using $\int n_i n_j\,d\omega=(4\pi/3)\delta_{ij}$,

$$
\int_{r=a}x\times\sigma n\,dS=-3\mu B\int\{\boldsymbol\Omega-n(n\cdot\boldsymbol\Omega)\}\,d\omega=-8\pi\mu B\boldsymbol\Omega.
$$

Hence the sustaining applied [Torque in rotational Stokes flow between concentric spheres](../../../stokes-flow.md#torque-in-rotational-stokes-flow-between-concentric-spheres) is

$$
\boxed{\boldsymbol G=\frac{8\pi\mu a^3b^3}{b^3-a^3}\boldsymbol\Omega.}
$$

For $a\ll b$, it approaches the isolated [rotating sphere in Stokes flow](../../../stokes-flow.md#rotating-sphere-in-stokes-flow) result $8\pi\mu a^3\boldsymbol\Omega$. For a narrow gap $d=b-a\ll a$, it becomes $8\pi\mu a^4\boldsymbol\Omega/(3d)$: the divergent resistance is that of a thin Couette shear layer, with speed scale $a\Omega$ and gradient scale $a\Omega/d$.

Now add the force-free, couple-free rigid particles and denote the resulting [velocity](../../../classical-mechanics.md#velocity) by $u_p$. Extend $u_p$ through each particle as its rigid translational and rotational [velocity](../../../classical-mechanics.md#velocity). No slip makes this extension continuous across every particle surface; it is incompressible and has zero [rate-of-strain tensor](../../../viscous-fluid-flow.md#strain-rate-tensor) inside each particle. It therefore gives an admissible trial [velocity](../../../classical-mechanics.md#velocity) in the original particle-free annulus, with exactly the same sphere boundary velocities. Its full-annulus dissipation is the actual fluid dissipation $\mathcal D_p$, since the added interior integrals are zero. The [Minimum-dissipation theorem for Stokes flow](../../../stokes-flow.md#minimum-dissipation-theorem-for-stokes-flow) consequently gives $\mathcal D_p\geq\mathcal D_0$.

The boundary-work identity follows by integrating $\nabla\cdot(\sigma u)$: dissipation equals the mechanical power supplied at all rigid boundaries. The outer sphere is stationary; the inner sphere has no translation, so any force needed to hold its centre does no work; and each added particle contributes zero power because its net force and couple are zero. Thus $\mathcal D_p=\boldsymbol G_p\cdot\boldsymbol\Omega$, while $\mathcal D_0=\boldsymbol G_0\cdot\boldsymbol\Omega$. Therefore

$$
\boxed{(\boldsymbol G_p-\boldsymbol G_0)\cdot\boldsymbol\Omega\geq0.}
$$

For $\boldsymbol\Omega\ne0$ and at least one particle of positive volume in the open annulus, the inequality is strict. Equality would make the extended [velocity](../../../classical-mechanics.md#velocity) identical to the particle-free solution, yet that solution has nonzero strain on every open region away from the rotation axis and cannot be rigid throughout any particle interior. Hence **the applied couple component along the imposed angular [velocity](../../../classical-mechanics.md#velocity) increases**. This is the fixed-[velocity](../../../classical-mechanics.md#velocity) [extra dissipation due to a rigid inclusion](../../../stokes-flow.md#extra-dissipation-due-to-a-rigid-inclusion) argument; it does not assert an increase in every transverse torque component.

## 2

↑ **Parent:** [Paper 78](paper-78.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a [slender viscous bubble](../../../viscous-fluid-flow.md#slender-viscous-bubble), approximate the interface normal by the radial direction and its curvature by $1/a$. Axial curvature and axial derivatives of the leading external motion are smaller by the slenderness factors. The exterior leading [Stokes flow](../../../stokes-flow.md) is locally radial. Incompressibility gives $\partial_r(ru_r)=0$, while the [kinematic boundary condition](../../../fluid-mechanics.md#kinematic-boundary-condition) gives $u_r(a)=a_t$ to leading order, hence

$$
u_r(r,z,t)=\frac{a(z,t)a_t(z,t)}r.
$$

The radial viscous Laplacian of this $1/r$ [velocity](../../../classical-mechanics.md#velocity) vanishes, so exterior [pressure](../../../thermodynamics.md#pressure) is constant to leading order; set its reference value to zero. Its radial [normal stress](../../../continuum-mechanics.md#normal-stress) at the interface is $2\mu\partial_ru_r|_a=-2\mu a_t/a$. Inner viscous [normal stress](../../../continuum-mechanics.md#normal-stress) is smaller by the viscosity ratio $\lambda$, and the bubble's leading [normal stress](../../../continuum-mechanics.md#normal-stress) is $-P$. The [interfacial stress balance with variable surface tension](../../../fluid-mechanics.md#interfacial-stress-balance-with-variable-surface-tension), here with constant $\gamma$, consequently gives

$$
P-\frac{2\mu a_t}a=\frac\gamma a,\qquad\boxed{P=\frac{2\mu a_t}a+\frac\gamma a.}
$$

These are local leading-order relations: the outer axial flow and tangential traction enter at higher slenderness order. The sign also has a useful check: a uniform cylinder with no imposed excess [pressure](../../../thermodynamics.md#pressure) contracts, $a_t=-\gamma/(2\mu)$, under [surface tension](../../../fluid-mechanics.md#surface-tension).

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

When [pressure](../../../thermodynamics.md#pressure) is uniform along the bubble, its normal-stress relation is $2\mu a_t=Pa-\gamma$. Use the PDF's amplitude convention $a=f+\sqrt2\,g\sin kz$; the square root acts on $2$ only, not on $2g$. Comparing constant and sinusoidal terms gives

$$
2\mu\dot f=Pf-\gamma,\qquad 2\mu\dot g=Pg.
$$

The mean cross-sectional area of an incompressible periodic segment is proportional to $\langle a^2\rangle=f^2+g^2$ and is conserved. Thus

$$
\boxed{\alpha_0=f(0)^2+g(0)^2=f(t)^2+g(t)^2.}
$$

Its time derivative vanishes, and substitution of the preceding two equations gives $P\alpha_0=\gamma f$. Therefore the [uniform-pressure evolution of a slender viscous bubble](../../../viscous-fluid-flow.md#uniform-pressure-evolution-of-a-slender-viscous-bubble) is

$$
\boxed{P=\frac{\gamma f}{\alpha_0},\qquad\dot f=-\frac{\gamma g^2}{2\mu\alpha_0},\qquad\dot g=\frac{\gamma fg}{2\mu\alpha_0}.}
$$

For a small disturbance to radius $a_0$, $f=a_0+O(g^2)$ and $\alpha_0=a_0^2+O(g^2)$, so its amplitude grows as $g\propto e^{st}$ with

$$
\boxed{s=\frac\gamma{2\mu a_0}.}
$$

The leading long-wave growth rate is independent of $k$ because axial curvature has been neglected; this is not a finite-wavelength dispersion relation.

While $f>\sqrt2g>0$, the minimum radius is $a_{\min}=f-\sqrt2g$. Its derivative is

$$
\boxed{\dot a_{\min}=-\frac\gamma{2\mu\alpha_0}(g^2+\sqrt2fg)<0.}
$$

Thus the minimum keeps decreasing in the nonlinear uniform-[pressure](../../../thermodynamics.md#pressure) model, with no need to solve $f,g$ explicitly. Finite internal viscosity eventually invalidates this model close enough to the neck.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $s=a_{\min}$ be a small neck radius in the preceding sinusoidal shape. Expanding around a minimum gives $a\simeq s+(gk^2/\sqrt2)(z-z_*)^2$, so its local axial length is $\ell\sim[s/(gk^2)]^{1/2}$. The uniform-[pressure](../../../thermodynamics.md#pressure) model has $|a_t|\sim\gamma/\mu$ near the neck. Local [conservation of mass](../../../continuum-mechanics.md#mass-conservation) therefore demands axial inner flux $Q\sim s(\gamma/\mu)\ell$. Internal [Hagen-Poiseuille flow](../../../viscous-fluid-flow.md#hagen-poiseuille-equation) of viscosity $\lambda\mu$ would require a [pressure](../../../thermodynamics.md#pressure) difference

$$
\Delta P\sim\frac{\lambda\mu Q\ell}{s^4}\sim\frac{\lambda\gamma\ell^2}{s^3},\qquad
\frac{\Delta P}{\gamma/s}\sim\frac{\lambda}{gk^2s}.
$$

If $sk\ll\lambda$, while $gk\ll1$ by slenderness, this ratio is very large. Hence **internal [pressure](../../../thermodynamics.md#pressure) variation certainly cannot be neglected when $a_{\min}k\ll\lambda$**. This is a sufficient breakdown condition; appreciable variation can arise earlier, especially because the radial viscous and capillary terms nearly cancel in the uniform-[pressure](../../../thermodynamics.md#pressure) regime.

For the inner flow, the leading axial [pressure](../../../thermodynamics.md#pressure) is uniform across a section. Neglect the much smaller interfacial axial [velocity](../../../classical-mechanics.md#velocity) relative to the internal [pressure](../../../thermodynamics.md#pressure)-driven motion. The [lubrication approximation](../../../viscous-fluid-flow.md#lubrication-theory) solves $\lambda\mu r^{-1}(ru_{z,r})_r=P_z$, with regularity at zero and $u_z(a)=0$ at leading order. Thus

$$
u_z=\frac{P_z}{4\lambda\mu}(r^2-a^2),\qquad Q=2\pi\int_0^a ru_z\,dr=-\frac{\pi a^4}{8\lambda\mu}P_z.
$$

The area balance $(\pi a^2)_t+Q_z=0$, combined with the exterior normal-stress relation, gives the [lubrication equation for a bubble with viscous exterior](../../../viscous-fluid-flow.md#lubrication-equation-for-a-bubble-with-viscous-exterior):

$$
\boxed{2aa_t=\frac1{8\lambda\mu}\partial_z\left[a^4\partial_z\left(\frac{2\mu a_t}a+\frac\gamma a\right)\right].}
$$

The neglected inner viscous [normal stress](../../../continuum-mechanics.md#normal-stress) is smaller by $\lambda$ in the similarity scales obtained next; the external axial interfacial speed is likewise smaller than the large [pressure](../../../thermodynamics.md#pressure)-driven inner speed.

Put $\tau=t_*-t$, $a\sim\tau^p$ and axial length $\ell\sim\tau^q$. The radial viscous [normal stress](../../../continuum-mechanics.md#normal-stress) scales as $\mu a_t/a\sim\tau^{-1}$ and capillary [pressure](../../../thermodynamics.md#pressure) as $\gamma/a\sim\tau^{-p}$. Retaining both requires $p=1$. The left side $aa_t$ scales as $\tau^{2p-1}$, while the axial-flux divergence scales as $a^4P/\ell^2\sim\tau^{4p-1-2q}$. Equating them gives $q=p=1$. Thus **both local radius and axial length shrink linearly in the remaining time**.

To obtain the specified dimensionless coefficients, choose the [linear pinch-off scaling of a slender viscous bubble](../../../viscous-fluid-flow.md#linear-pinch-off-scaling-of-a-slender-viscous-bubble)

$$
\boxed{a(z,t)=\frac\gamma\mu\tau A(\zeta),\qquad\zeta=\frac{\mu\sqrt\lambda(z-z_*)}{\gamma\tau}.}
$$

Then $a_t=(\gamma/\mu)(\zeta A'-A)$ and

$$
P=\frac\mu\tau\left[\frac{2\zeta A'+1}{A}-2\right].
$$

The constant $-2$ has no axial derivative. Substituting into the flux equation and cancelling its dimensional factor gives

$$
\boxed{\zeta AA'-A^2=\frac1{16}\left\{A^4\left[\frac{2\zeta A'+1}{A}\right]'\right\}'.}
$$

Both axial derivatives on the right are essential; the outer derivative is present in the PDF but lost in the converted TeX expression. The physical slope is $a_z=\sqrt\lambda A'$, so an order-one similarity profile remains slender for $\lambda\ll1$. No solution of this similarity ordinary differential equation is required.

## 3

↑ **Parent:** [Paper 78](paper-78.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

An [insoluble surfactant](../../../fluid-mechanics.md#insoluble-surfactant) is advected with the surface fluid and has no exchange with the bulk. With negligible surface diffusion, its amount on a material surface strip is conserved. Under the small-slope [lubrication approximation](../../../viscous-fluid-flow.md#lubrication-theory), surface arclength equals projected horizontal length to leading order, giving

$$
\boxed{C_t+\partial_x(Cu_s)=0,\qquad u_s=u(x,h(x,t),t).}
$$

This is the leading planar form of [conservation of insoluble surfactant on a moving interface](../../../fluid-mechanics.md#conservation-of-insoluble-surfactant-on-a-moving-interface).

Let $y$ measure height above the substrate. The normal-stress and vertical momentum conditions give $p=p_{\mathrm{atm}}-\gamma h_{xx}+\rho g(h-y)$, so $p_x=\rho gh_x-(\gamma h_{xx})_x$. Horizontal [Stokes flow](../../../stokes-flow.md) obeys $\mu u_{yy}=p_x$, with no slip at $y=0$ and [Marangoni stress](../../../fluid-mechanics.md#marangoni-effect) $\mu u_y(h)=\gamma_x$. Thus

$$
u=\frac{p_x}{2\mu}(y^2-2hy)+\frac{\gamma_x}\mu y,
$$



$$
q=\int_0^hu\,dy=-\frac{h^3}{3\mu}p_x+\frac{h^2}{2\mu}\gamma_x,\qquad
u_s=-\frac{h^2}{2\mu}p_x+\frac h\mu\gamma_x.
$$

Use $h_t+q_x=0$ and $\gamma_x=-AC_x$ to obtain the [thin-film equations with insoluble surfactant](../../../viscous-fluid-flow.md#thin-film-equations-with-insoluble-surfactant):

$$
\boxed{h_t=\frac A{2\mu}(h^2C_x)_x+\frac{\rho g}{3\mu}(h^3h_x)_x-\frac1{3\mu}[h^3(\gamma h_{xx})_x]_x,}
$$



$$
\boxed{C_t=\frac A\mu(hCC_x)_x+\frac{\rho g}{2\mu}(h^2Ch_x)_x-\frac1{2\mu}[h^2C(\gamma h_{xx})_x]_x.}
$$

The differing flux coefficients are essential: the [surfactant](../../../fluid-mechanics.md#surfactant) travels at the surface [velocity](../../../classical-mechanics.md#velocity), not at the depth-averaged liquid [velocity](../../../classical-mechanics.md#velocity).

Neglect the two [pressure](../../../thermodynamics.md#pressure)-gradient terms for the spreading outer region. If its half-length is $\ell$, fixed [surfactant](../../../fluid-mechanics.md#surfactant) mass gives $C\sim M/\ell$, $C_x\sim M/\ell^2$. The surface [velocity](../../../classical-mechanics.md#velocity) is then $u_s\sim AMh_0/(\mu\ell^2)$. Equating this to $\ell/t$ gives **$\ell\propto t^{1/3}$**. For the precise [finite-mass Marangoni spreading on a liquid film](../../../viscous-fluid-flow.md#finite-mass-marangoni-spreading-on-a-liquid-film) solution choose

$$
L(t)=\left(\frac{AMh_0t}\mu\right)^{1/3},\qquad\eta=\frac xL,\qquad h=h_0H(\eta),\quad C=\frac ML\Gamma(\eta),
$$

with symmetry about zero and support $0\leq\eta\leq\eta_N$ on the positive half-line. The reduced differential equations are

$$
\boxed{-\frac13\eta H'=\frac12(H^2\Gamma')',\qquad -\frac13(\eta\Gamma)'=(H\Gamma\Gamma')'.}
$$

Their boundary conditions are zero flux at the centre and zero concentration at the moving front. The two integral constraints express conserved surfactant mass and zero net change of liquid volume relative to the original uniform layer:

$$
\boxed{2\int_0^{\eta_N}\Gamma\,d\eta=1,\qquad\int_0^{\eta_N}(H-1)\,d\eta=0.}
$$

The second follows by integrating $h_t+q_x=0$ across the whole layer: the localized release adds surfactant but no liquid, and the flux vanishes at infinity. Outside the spreading region the leading depth remains $h_0$.

Integrating the concentration equation from the centre gives $H\Gamma\Gamma'=-\eta\Gamma/3$. Where $\Gamma>0$, this is $H\Gamma'=-\eta/3$. Substituting into the height equation gives

$$
-\frac13\eta H'=-\frac16(H+\eta H'),\qquad\eta H'=H.
$$

Therefore $H=c\eta$, and $\Gamma'= -1/(3c)$. With $\Gamma(\eta_N)=0$, the [linear similarity profiles for surfactant spreading](../../../viscous-fluid-flow.md#linear-similarity-profiles-for-surfactant-spreading) are $\Gamma=(\eta_N-\eta)/(3c)$. The liquid-volume constraint gives $c\eta_N=2$, while the surfactant constraint gives $\eta_N^2/(3c)=1$. Thus $\eta_N^3=6$, and

$$
\boxed{x_N=\eta_NL=\left(\frac{6AMh_0t}\mu\right)^{1/3}.}
$$

In physical variables, the leading profiles on the whole line are

$$
\boxed{h(x,t)=2h_0\frac{|x|}{x_N},\qquad C(x,t)=\frac M{x_N}\left(1-\frac{|x|}{x_N}\right),\quad |x|<x_N.}
$$

Outside this interval $h=h_0$ and $C=0$. The formal outer solution reaches zero depth at the central point, and height $2h_0$ immediately inside the front. It is not a microscopic description of the central dry region or of the front transition. As a conservation check, the front [velocity](../../../classical-mechanics.md#velocity) equals both the incoming surface [velocity](../../../classical-mechanics.md#velocity) and the liquid Rankine–Hugoniot speed $q/(2h_0-h_0)=2AMh_0/(\mu x_N^2)=\dot x_N$.

The jump from $2h_0$ to $h_0$ cannot persist as a smooth solution with both hydrostatic and capillary gradients absent. In an edge region of width $\Delta$, a depth change of order $h_0$ produces $h_x\sim h_0/\Delta$ and $h_{xxx}\sim h_0/\Delta^3$. Keep the stipulated concentration-gradient scale $M/x_N^2$. The three liquid-flux scales are

$$
q_M\sim\frac{AMh_0^2}{\mu x_N^2},\qquad q_g\sim\frac{\rho gh_0^4}{\mu\Delta},\qquad q_\gamma\sim\frac{\gamma_0h_0^4}{\mu\Delta^3}.
$$

For $g=0$, balancing $q_M$ and $q_\gamma$ gives the [capillary smoothing of a Marangoni front](../../../viscous-fluid-flow.md#capillary-smoothing-of-a-marangoni-front) width

$$
\boxed{\Delta\sim\left(\frac{\gamma_0h_0^2x_N^2}{AM}\right)^{1/3}\propto t^{2/9}.}
$$

Gravity dominates capillarity when $q_g/q_\gamma\sim\rho g\Delta^2/\gamma_0\gg1$. In physical units the condition is $\Delta^2\gg\gamma_0/(\rho g)$: the printed $\gamma_0/g$ omits density and is dimensionally incomplete unless [surface tension](../../../fluid-mechanics.md#surface-tension) has already been divided by density. Balancing the gravity flux with $q_M$ yields the [gravity smoothing of a Marangoni front](../../../viscous-fluid-flow.md#gravity-smoothing-of-a-marangoni-front):

$$
\boxed{\Delta\sim\frac{\rho gh_0^2x_N^2}{AM}\propto t^{2/3}.}
$$

This layer grows faster than the spreading half-length. It reaches the whole pool when

$$
\boxed{x_N\sim\frac{AM}{\rho gh_0^2},\qquad t_*\sim\frac{\mu(AM)^2}{(\rho g)^3h_0^7}.}
$$

Only scaling constants can be fixed by this balance, so an exact numerical coefficient in $t_*$ is not implied. The gravity-dominant assumption must hold at this crossover as well.

For $t\gg t_*$, the sharp-front linear-depth outer profile is replaced by a [gravity-levelled surfactant film](../../../viscous-fluid-flow.md#gravity-levelled-surfactant-film): the height approaches $h_0$, with a small depression under the surfactant and redistributed liquid outside. The rapid hydrostatic return flow almost cancels the net Marangoni liquid flux. Setting $q\simeq0$ and $h\simeq h_0$ gives $h_x\simeq-3AC_x/(2\rho gh_0)$ and fractional depth variation $O(AM/(\rho gh_0^2x_N))\ll1$. The surface still moves outward, with $u_s\simeq-Ah_0C_x/(4\mu)$, so leveling the bulk liquid does not stop surfactant spreading.

## 4

↑ **Parent:** [Paper 78](paper-78.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Choose transverse $x$ along the cusp from the line of cylinder contact, and $y$ across its narrow gap. Expanding the two circular boundaries for $x\ll a$ gives $y=\pm x^2/(2a)$, so the local full gap is $d(x)=x^2/a$. At the meniscus, $x\simeq w$, a semicircle fits across this gap with radius $d(w)/2=w^2/(2a)$. Thus the leading area and transverse curvature in the [cusp flow between touching cylinders](../../../viscous-fluid-flow.md#cusp-flow-between-touching-cylinders) are

$$
\boxed{\mathcal A=\int_0^w\frac{x^2}a\,dx=\frac{w^3}{3a},\qquad\kappa=\frac{2a}{w^2}.}
$$

The meniscus area correction is $O(w^4/a^2)$ and is small relative to $w^3/a$. The curvature is stated as a positive suction magnitude; the liquid [pressure](../../../thermodynamics.md#pressure) relative to air is $p=-2\gamma a/w^2$. Axial curvature is negligible compared with this transverse curvature under the slow-variation approximation.

At fixed $x$, axial [lubrication theory](../../../viscous-fluid-flow.md#lubrication-theory) gives a local slit [Poiseuille flow](../../../viscous-fluid-flow.md#hagen-poiseuille-equation) between rigid walls $y=\pm d/2$:

$$
u_z=\frac{p_z}{2\mu}\left(y^2-\frac{d^2}4\right),\qquad
\int_{-d/2}^{d/2}u_z\,dy=-\frac{d^3}{12\mu}p_z.
$$

Integrating across the cusp gives

$$
Q=-\frac{p_z}{12\mu a^3}\int_0^wx^6dx=-\frac{w^7}{84\mu a^3}p_z.
$$

The local meniscus edge correction occupies a transverse width small compared with $w$ and does not change this leading flux. Since $p_z=4\gamma a w^{-3}w_z$, the axial [volume flux](../../../fluid-mechanics.md#volumetric-flow-rate) is $Q=-\gamma w^4w_z/(21\mu a^2)$. Area conservation $\mathcal A_t+Q_z=0$ now gives

$$
\boxed{(w^3)_t=\frac\gamma{7\mu a}(w^4w_z)_z.}
$$

Writing $u=w^3$ also puts this in [porous medium equation](../../../diffusion-equation.md#porous-medium-equation) form $u_t=\gamma(u^{5/3})_{zz}/(35\mu a)$, explaining the finite-support spreading profile.

Set $K=\gamma/(7\mu a)$. Fixed volume means $\int w^3dz=3aV$. If $w\propto t^{-\beta}$ and axial extent is proportional to $t^\alpha$, this conservation gives $\alpha=3\beta$. The evolution equation gives $3\beta+1=5\beta+2\alpha$, hence **$\beta=1/8$, $\alpha=3/8$**.

For the symmetric source-type [similarity solution](../../../partial-differential-equation.md#similarity-solution), write $w=t^{-1/8}f(\eta)$, $\eta=z/t^{3/8}$. The differential equation becomes

$$
-\frac38(f^3+\eta(f^3)')=K(f^4f')'.
$$

Integrate from the centre using zero flux and symmetry. This gives $Kf^4f'=-3\eta f^3/8$, so on the positive support $ff'=-3\eta/(8K)$. With $f(\eta_N)=0$,

$$
f^2=\frac3{8K}(\eta_N^2-\eta^2).
$$

Therefore the [fixed-volume capillary spreading in a cylindrical cusp](../../../viscous-fluid-flow.md#fixed-volume-capillary-spreading-in-a-cylindrical-cusp) profile is

$$
\boxed{w(z,t)=\left[\frac{21\mu a}{8\gamma t}(z_N(t)^2-z^2)\right]_+^{1/2}.}
$$

Let $B=21\mu a/(8\gamma t)$. Its volume is

$$
V=\frac1{3a}\int_{-z_N}^{z_N}w^3dz=\frac{B^{3/2}z_N^4}{3a}\int_{-1}^1(1-s^2)^{3/2}ds.
$$

With $s=\sin\theta$, the last integral is $\int_{-\pi/2}^{\pi/2}\cos^4\theta\,d\theta=3\pi/8$, equal to the supplied sine integral by symmetry. Consequently $V=\pi B^{3/2}z_N^4/(8a)$, yielding

$$
\boxed{z_N(t)=\left(\frac{8Va}\pi\right)^{1/4}\left(\frac{8\gamma t}{21\mu a}\right)^{3/8}.}
$$

The other tip is at $-z_N$. The maximum width decays as $t^{-1/8}$. This is the leading slender outer solution: the ideal point injection and the steep microscopic nose require local descriptions outside its uniform lubrication range.

Finally, for vertical cylinders let $\rho$ denote the liquid density, and take the bath [pressure](../../../thermodynamics.md#pressure) at $z=0$ as the air-[pressure](../../../thermodynamics.md#pressure) reference. At rest the liquid [pressure](../../../thermodynamics.md#pressure) is $p(z)=-\rho gz$. Equating hydrostatic suction with the wetting-meniscus [capillary pressure](../../../fluid-mechanics.md#capillary-pressure) gives the [hydrostatic rise in a cylindrical cusp](../../../viscous-fluid-flow.md#hydrostatic-rise-in-a-cylindrical-cusp):

$$
\rho gz=\frac{2\gamma a}{w^2},\qquad\boxed{w(z)\sim\left(\frac{2\gamma a}{\rho gz}\right)^{1/2}\quad(z\text{ large}).}
$$

The cusp can therefore support an indefinitely high, increasingly narrow ideal wetting tail rather than a fixed terminal rise height. Large $z$ makes $w\ll a$ and strengthens the transverse cusp approximation, until microscopic physics limits the continuum description.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
