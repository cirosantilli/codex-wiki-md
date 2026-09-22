# Paper 314

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_314.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2018/paper_314.pdf)

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
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)

## 1

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use the [Euler equations for an inviscid fluid](../../../fluid-mechanics.md#euler-equations-for-an-inviscid-fluid) with no magnetic or gravitational force. Let $w$ denote [specific enthalpy](../../../thermodynamics.md#specific-enthalpy). For a [homentropic flow](../../../compressible-flow.md#homentropic-flow), $dw=dp/\rho$, so the pressure acceleration is $-\nabla w$. The velocity identity

$$
(\mathbf u\cdot\nabla)\mathbf u=\nabla\frac{u^2}{2}-\mathbf u\times\boldsymbol\omega,\qquad\boldsymbol\omega=\nabla\times\mathbf u,
$$

therefore gives

$$
\partial_t\mathbf u=\mathbf u\times\boldsymbol\omega-\nabla\mathcal B,\qquad\mathcal B=w+\frac{u^2}{2}.
$$

Taking the [curl](../../../calculus.md#curl), using that the curl of a [gradient](../../../calculus.md#gradient) is zero and that differentiation commutes for smooth fields, proves [barotropic vorticity transport](../../../fluid-mechanics.md#barotropic-vorticity-transport):

$$
\boxed{\partial_t\boldsymbol\omega=\nabla\times(\mathbf u\times\boldsymbol\omega).}
$$

More generally the same proof works for any [barotropic fluid](../../../fluid-mechanics.md#barotropic-fluid), replacing $w$ by a pressure potential $\int^\rho p'(s)\,ds/s$. Here “isentropic” must supply this barotropic closure, for example through one common [specific entropy](../../../thermodynamics.md#specific-entropy) throughout the fluid. Merely imposing [entropy advection equation](../../../astrophysical-fluid-dynamics.md#entropy-advection-equation) $Ds/Dt=0$ allows spatial [specific entropy](../../../thermodynamics.md#specific-entropy) gradients; in that case the [vorticity equation](../../../physics.md#vorticity-equation) contains the additional [baroclinic vorticity generation](../../../physics.md#baroclinic-vorticity-generation) term $\rho^{-2}\nabla\rho\times\nabla p$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write $q=\mathbf u\cdot\boldsymbol\omega$ for the [kinetic helicity density](../../../fluid-mechanics.md#kinetic-helicity-density), and retain $\mathcal B=w+u^2/2$. Since $\boldsymbol\omega$ is a [curl](../../../calculus.md#curl), $\nabla\cdot\boldsymbol\omega=0$. Differentiating the density and using the equations from the preceding part gives

$$
\partial_tq=-\boldsymbol\omega\cdot\nabla\mathcal B+\mathbf u\cdot\nabla\times(\mathbf u\times\boldsymbol\omega).
$$

The [divergence of a cross product](../../../calculus.md#divergence-of-a-cross-product) gives

$$
\nabla\cdot\{\mathbf u\times(\mathbf u\times\boldsymbol\omega)\}=(\mathbf u\times\boldsymbol\omega)\cdot\boldsymbol\omega-\mathbf u\cdot\nabla\times(\mathbf u\times\boldsymbol\omega).
$$

The first term on the right is zero, while $\boldsymbol\omega\cdot\nabla\mathcal B=\nabla\cdot(\mathcal B\boldsymbol\omega)$. Thus the [kinetic helicity conservation law](../../../fluid-mechanics.md#kinetic-helicity-conservation-law) has flux

$$
\boxed{\mathbf F_{H_k}=\mathcal B\boldsymbol\omega+\mathbf u\times(\mathbf u\times\boldsymbol\omega)=q\mathbf u+\left(w-\frac{u^2}{2}\right)\boldsymbol\omega,\qquad\partial_tq+\nabla\cdot\mathbf F_{H_k}=0.}
$$

The last equality for the flux uses the [vector triple product identity](../../../calculus.md#vector-triple-product). Integrating and applying the [divergence theorem](../../../calculus.md#divergence-theorem) gives $d\int_Vq\,dV/dt=-\int_{\partial V}\mathbf F_{H_k}\cdot\mathbf n\,dS$ for a fixed volume. Hence its total [kinetic helicity](../../../fluid-mechanics.md#hydrodynamical-helicity) is conserved when the boundary flux vanishes; for example, tangency of both [velocity field](../../../fluid-mechanics.md#velocity-field) and [vorticity](../../../fluid-mechanics.md#vorticity) to the boundary is sufficient. The local [conservation law](../../../physics.md#conservation-law) does not by itself imply that its density follows each fluid particle unchanged.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Expanding the [kinetic helicity conservation law](../../../fluid-mechanics.md#kinetic-helicity-conservation-law) separates [advection](../../../fluid-mechanics.md#advection) from the other flux:

$$
\boxed{\frac{Dq}{Dt}=\boldsymbol\omega\cdot\nabla\left(\frac{u^2}{2}-w\right)-q\nabla\cdot\mathbf u.}
$$

Thus [material conservation of kinetic helicity density](../../../fluid-mechanics.md#material-conservation-of-kinetic-helicity-density) holds precisely when

$$
\boxed{\boldsymbol\omega\cdot\nabla\left(\frac{u^2}{2}-w\right)=q\nabla\cdot\mathbf u.}
$$

An especially useful sufficient pair of conditions is [incompressible flow](../../../fluid-mechanics.md#incompressible-flow), $\nabla\cdot\mathbf u=0$, and constancy of $w-u^2/2$ along integral curves of the [vorticity](../../../fluid-mechanics.md#vorticity), $\boldsymbol\omega\cdot\nabla(w-u^2/2)=0$. Together these conditions make both terms vanish without cancellation. They are not necessary individually, because the two terms in the displayed balance can cancel. An [irrotational flow](../../../fluid-mechanics.md#irrotational-flow) is a trivial conserved case with $q=0$.

For contrast, combining the balance with [mass conservation](../../../continuum-mechanics.md#mass-conservation) gives

$$
\frac D{Dt}\left(\frac q\rho\right)=-\frac{\boldsymbol\omega}{\rho}\cdot\nabla\left(w-\frac{u^2}{2}\right).
$$

Consequently constancy of $w-u^2/2$ along integral curves of the [vorticity](../../../fluid-mechanics.md#vorticity) makes $q/\rho$ an advected scalar even in [compressible flow](../../../compressible-flow.md); it does not generally make $q$ itself constant.

## 2

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Work in the [shock frame](../../../compressible-flow.md#shock-frame), assume a calorically [perfect gas](../../../thermodynamics.md#ideal-gas) with fixed [specific-heat ratio](../../../thermodynamics.md#heat-capacity-ratio) $\gamma>1$, and neglect magnetic stresses and body forces across the thin shock. The [internal energy](../../../thermodynamics.md#internal-energy) per unit mass is $e=p/[(\gamma-1)\rho]$, and the [specific enthalpy](../../../thermodynamics.md#specific-enthalpy) is $w=\gamma p/[(\gamma-1)\rho]$. Integrating the local [conservation laws](../../../physics.md#conservation-law) across a thin stationary control volume makes the [mass flux](../../../physics.md#mass-flux) $\rho u$, [momentum flux](../../../physics.md#momentum-flux) $p+\rho u^2$, and [energy flux](../../../physics.md#energy-flux) $u(\rho u^2/2+\gamma p/(\gamma-1))$ continuous. Hence the [Rankine-Hugoniot conditions for a perfect gas](../../../compressible-flow.md#rankine-hugoniot-conditions-for-a-perfect-gas) are

$$
\rho_1u_1=\rho_2u_2=m,\qquad p_1+\rho_1u_1^2=p_2+\rho_2u_2^2,\qquad\frac{u_1^2}{2}+\frac{\gamma p_1}{(\gamma-1)\rho_1}=\frac{u_2^2}{2}+\frac{\gamma p_2}{(\gamma-1)\rho_2}.
$$

Multiplication of the last equality by $m$ gives continuity of the stated energy flux. These express that mass, momentum and energy cannot accumulate in an infinitesimally thin steady shock, although [entropy production](../../../thermodynamics.md#entropy-production) occurs on the physical compression branch. The same constant in the [polytropic equation of state](../../../astrophysical-fluid-dynamics.md#polytropic-equation-of-state) $p=K\rho^\gamma$ must therefore not be imposed on both sides. For flow from $z>0$ to $z<0$, both signed velocities are negative; the flux equations and ratios remain valid.

In the [Strong-shock Rankine-Hugoniot conditions](../../../compressible-flow.md#strong-shock-rankine-hugoniot-conditions), $p_1/(\rho_1u_1^2)=1/(\gamma M_1^2)$ tends to zero. Put $r=\rho_2/\rho_1$. The first two flux balances give $u_2=u_1/r$ and $p_2=\rho_1u_1^2(1-1/r)$ to leading order. The energy balance becomes

$$
\frac12=\frac1{2r^2}+\frac{\gamma}{\gamma-1}\frac{1-1/r}{r},\qquad(r-1)\{(\gamma-1)r-(\gamma+1)\}=0.
$$

Discarding the unchanged-state root $r=1$ gives the compressive [shock compression ratio](../../../compressible-flow.md#shock-compression-ratio) and the required limits:

$$
\boxed{\frac{\rho_2}{\rho_1}\longrightarrow\frac{\gamma+1}{\gamma-1},\qquad\frac{u_2}{u_1}\longrightarrow\frac{\gamma-1}{\gamma+1},\qquad\frac{p_2}{\rho_1u_1^2}\longrightarrow\frac2{\gamma+1}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The dimensions of the injected power and ambient [mass density](../../../fluid-mechanics.md#density) are $[\dot E]=ML^2T^{-3}$ and $[\rho_1]=ML^{-3}$. Requiring $\dot E^a\rho_1^bt^c$ to have the dimensions of length gives

$$
a+b=0,\qquad2a-3b=1,\qquad-3a+c=0.
$$

Thus [dimensional analysis](../../../physics.md#dimensional-analysis) gives the [adiabatic superbubble similarity solution](../../../galaxy.md#adiabatic-superbubble-similarity-solution)

$$
\boxed{a=\frac15,\quad b=-\frac15,\quad c=\frac35,\qquad R(t)=\alpha\left(\frac{\dot E}{\rho_1}\right)^{1/5}t^{3/5},\qquad\dot R=\frac{3R}{5t}.}
$$

The dimensionless coefficient $\alpha$ can depend on $\gamma$ and the specified inner structure, but dimensions alone cannot determine it. Constant power differs from a fixed-energy explosion because the energy available at time $t$ is proportional to $t$. This scaling assumes that ambient pressure, gravity, radiative losses and the finite injection radius introduce no relevant competing scale.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

The original PDF supplies the intended profiles $\rho=\rho_1f(\eta)$, $p=\rho_1\dot R^2g(\eta)$ and $u=\dot Rh(\eta)$; the TeX has corrupted the first two. At fixed $r$, $\partial_t\eta=-\eta\dot R/R$, and at fixed $t$, $\partial_r\eta=1/R$. The spherical [continuity equation](../../../physics.md#continuity-equation) is therefore

$$
0=\partial_t\rho+\frac1{r^2}\partial_r(r^2\rho u)=\frac{\rho_1\dot R}{R}\left[-\eta f'+\frac1{\eta^2}(\eta^2fh)'\right].
$$

Since $\dot R/R=3/(5t)$ is nonzero, the [continuity equation for a superbubble similarity solution](../../../galaxy.md#continuity-equation-for-a-superbubble-similarity-solution) is

$$
\boxed{-\eta f'+\frac1{\eta^2}(\eta^2fh)'=0,\qquad\text{or}\qquad(h-\eta)f'+fh'+\frac{2fh}{\eta}=0.}
$$

The ambient gas is at rest. In the locally stationary [shock frame](../../../compressible-flow.md#shock-frame), its velocity is $-\dot R$; the downstream velocity is $u-\dot R$. Using the [shock compression ratio](../../../compressible-flow.md#shock-compression-ratio) from part (a) converts the downstream speed back to the laboratory frame and gives the inner shock boundary conditions

$$
\boxed{f(1^-)=\frac{\gamma+1}{\gamma-1},\qquad g(1^-)=\frac2{\gamma+1},\qquad h(1^-)=\frac2{\gamma+1}.}
$$

Immediately outside the shock, the corresponding unperturbed profiles are $f=1$, $g=0$ and $h=0$, with $g=0$ understood in the negligible-ambient-pressure limit.

The inner boundary must supply the injected power. If the source is idealized as a point and the profiles extend all the way inward, [central energy input in a similarity solution](../../../galaxy.md#central-energy-input-in-a-similarity-solution) requires

$$
\lim_{r\downarrow0}4\pi r^2u\left(\frac{\rho u^2}{2}+\frac{\gamma p}{\gamma-1}\right)=\dot E,
$$

or equivalently $\lim_{\eta\downarrow0}\eta^2h(fh^2/2+\gamma g/(\gamma-1))=125/(108\pi\alpha^5)$. A finite source region or an inner wind/contact region supplies a different matching description. One cannot impose a regular zero-flux centre on a source-free interior and still inject nonzero power.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The [conservation of energy](../../../physics.md#conservation-of-energy) to use here is the total [kinetic energy](../../../classical-mechanics.md#kinetic-energy) plus [internal energy](../../../thermodynamics.md#internal-energy) inside the shock, not just the internal energy of a uniform-pressure core. With no radiative loss and negligible initial ambient energy,

$$
\dot Et=4\pi\int_0^{R(t)}\left(\frac12\rho u^2+\frac{p}{\gamma-1}\right)r^2\,dr.
$$

Substitute the [adiabatic superbubble similarity solution](../../../galaxy.md#adiabatic-superbubble-similarity-solution) and define the finite positive dimensionless integral

$$
I=\int_0^1\left(\frac12f(\eta)h(\eta)^2+\frac{g(\eta)}{\gamma-1}\right)\eta^2\,d\eta.
$$

Then $\dot Et=4\pi\rho_1\dot R^2R^3I$. Since $\dot R=3R/(5t)$ and $R^5=\alpha^5(\dot E/\rho_1)t^3$,

$$
\dot Et=\frac{36\pi}{25}\alpha^5\dot Et\,I,
\qquad\boxed{\alpha=\left(\frac{25}{36\pi I}\right)^{1/5}.}
$$

This is the [energy normalization of a continuously driven spherical shock](../../../galaxy.md#energy-normalization-of-a-continuously-driven-spherical-shock). It fixes $\alpha$ once the similarity profiles are determined. If the profiles describe only the shocked ambient layer, the energy of the interior hot bubble must also be included before using this normalization. A radiatively cooled shell has a different energy budget; its familiar numerical coefficient should not be substituted into this loss-free model.

## 3

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Set $A=\Phi_0R_0^\beta<0$, $q=\lambda^2$ and $s=R^2+qz^2$. The [flattened power-law gravitational potential](../../../classical-mechanics.md#flattened-power-law-gravitational-potential) is $\Phi=As^{-\beta/2}$. In axisymmetric [cylindrical coordinates](../../../calculus.md#cylindrical-coordinate-system), the [Poisson equation for Newtonian gravity](../../../classical-mechanics.md#poisson-equation-for-newtonian-gravity) gives

$$
4\pi G\rho=\frac1R\partial_R(R\partial_R\Phi)+\partial_z^2\Phi.
$$

The first derivatives are $\partial_R\Phi=-\beta ARs^{-(\beta+2)/2}$ and $\partial_z\Phi=-\beta Aqzs^{-(\beta+2)/2}$. Differentiating again and collecting powers gives

$$
\nabla^2\Phi=-\beta As^{-(\beta+4)/2}\left[(2+q)s-(\beta+2)(R^2+q^2z^2)\right].
$$

Therefore the required [mass density](../../../fluid-mechanics.md#density) is

$$
\boxed{\rho(R,z)=-\frac{\beta\Phi_0R_0^\beta}{4\pi G}\frac{(\lambda^2-\beta)R^2+\lambda^2[2-(\beta+1)\lambda^2]z^2}{(R^2+\lambda^2z^2)^{(\beta+4)/2}}.}
$$

This is a formal density for arbitrary $\lambda$, but a physical [dark matter](../../../cosmology.md#dark-matter) distribution must be nonnegative. The [density positivity for a flattened power-law potential](../../../classical-mechanics.md#density-positivity-for-a-flattened-power-law-potential) condition is

$$
\boxed{\beta\leq\lambda^2\leq\frac2{\beta+1}.}
$$

Necessity follows by evaluating on the midplane and symmetry axis; sufficiency follows because both numerator coefficients are then nonnegative. In this range the origin is a locally integrable density cusp: the mass enclosed near radius $r$ scales as $r^{1-\beta}$ and tends to zero, so no point mass needs adding. The scale-free distribution has infinite total mass at large radius and represents an idealized background, not a finite isolated halo.

For the cold, non-self-gravitating disk, radial balance of a [circular orbit](../../../classical-mechanics.md#circular-orbit) is $R\Omega^2=\partial_R\Phi(R,0)$. Thus

$$
\boxed{\Omega^2(R)=-\beta\Phi_0R_0^\beta R^{-\beta-2},\qquad\Omega(R)=\frac{\sqrt{-\beta\Phi_0}}{R_0}\left(\frac R{R_0}\right)^{-(\beta+2)/2}.}
$$

The displayed positive root chooses the rotation orientation; the opposite orientation has the negative of this angular frequency.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Use the [poloidal magnetic flux function](../../../astrophysical-fluid-dynamics.md#poloidal-magnetic-flux-function) convention $\mathbf B_p=R^{-1}\nabla\Psi\times\mathbf e_\phi$, so $2\pi\Psi$ is magnetic flux up to a reference constant. Its [poloidal magnetic field](../../../astrophysical-fluid-dynamics.md#poloidal-magnetic-field) components are

$$
\boxed{B_R=-\frac1R\frac{\partial\Psi}{\partial z},\qquad B_z=\frac1R\frac{\partial\Psi}{\partial R}.}
$$

The prescribed surface flux therefore gives

$$
B_z(R,0)=\frac{\delta\Psi_0}{R_0^\delta}R^{\delta-2},\qquad B_R(R,0)=B_z(R,0)\tan\alpha.
$$

The constant offset $\Psi_1$ does not affect either field component. If instead $\Psi$ denotes the full physical flux rather than flux divided by $2\pi$, both component formulas acquire a common $1/(2\pi)$ factor; the subsequent logarithmic derivative relation is unchanged.

The [Gauss's law for magnetism](../../../electromagnetism.md#gauss-s-law-for-magnetism) constraint is $R^{-1}\partial_R(RB_R)+\partial_zB_z=0$. Since $\alpha$ is constant with radius on the surface, it gives the [power-law poloidal field near a disk surface](../../../astrophysical-fluid-dynamics.md#power-law-poloidal-field-near-a-disk-surface) relation

$$
\boxed{\left.\frac{\partial B_z}{\partial z}\right|_{0}=-\frac{\delta(\delta-1)\Psi_0\tan\alpha}{R_0^\delta}R^{\delta-3}=-\frac{\delta-1}{R}B_z(R,0)\tan\alpha.}
$$

For a smooth one-sided field above the surface, $B_z(R,z)=B_z(R,0)[1-(\delta-1)\tan\alpha\,z/R]+O(z^2)$. Thus the field initially decreases with height if $\delta>1$, increases if $0<\delta<1$, and has zero first height derivative if $\delta=1$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

For local cold [magnetocentrifugal acceleration](../../../astrophysical-fluid-dynamics.md#magnetocentrifugal-acceleration), the field must guide the gas and enforce approximate corotation with its disk footpoint in the sub-Alfvénic launching region. Let that footpoint be $R=R_f$, and keep its [field-line angular velocity](../../../astrophysical-fluid-dynamics.md#field-line-angular-velocity) $\Omega_f=\Omega(R_f)$ constant along the field. In this rotating frame the relevant [effective potential](../../../physics.md#effective-potential) is

$$
V(R,z)=\Phi(R,z)-\frac12\Omega_f^2R^2.
$$

The footpoint is a critical point because $\partial_R\Phi(R_f,0)=R_f\Omega_f^2$ and $\partial_z\Phi(R_f,0)=0$. The meridional [Hessian matrix](../../../calculus.md#hessian-matrix) there is

$$
V_{RR}=-(\beta+2)\Omega_f^2,\qquad V_{zz}=\lambda^2\Omega_f^2,\qquad V_{Rz}=0.
$$

Take distance $\ell$ along a smooth outward [magnetic field line](../../../electromagnetism.md#magnetic-field-line) whose initial tangent is $(\sin\alpha,\cos\alpha)$ in the $(R,z)$ plane. Since the gradient of $V$ vanishes at the footpoint, field-line curvature does not contribute to its second derivative. Consequently

$$
V(\ell)-V(0)=\frac12\Omega_f^2\left[\lambda^2\cos^2\alpha-(\beta+2)\sin^2\alpha\right]\ell^2+O(\ell^3).
$$

A negative quadratic coefficient gives a downhill displacement and acceleration without thermal assistance. The [magnetocentrifugal launching criterion in a flattened power-law potential](../../../astrophysical-fluid-dynamics.md#magnetocentrifugal-launching-criterion-in-a-flattened-power-law-potential) is therefore

$$
\boxed{\tan^2\alpha>\frac{\lambda^2}{\beta+2},\qquad\alpha>\alpha_{\rm crit}=\arctan\left(\frac{|\lambda|}{\sqrt{\beta+2}}\right).}
$$

Angles are measured from the vertical, with $0\leq\alpha<\pi/2$. Below the critical angle the footpoint is a local minimum along the field, so a cold particle cannot cross the initial potential barrier. At equality the quadratic test is marginal; higher derivatives and the unspecified field curvature can decide the outcome. The threshold is a local condition for launch, not proof that the wind escapes along an arbitrary global field geometry. The spherical point-mass limit $\lambda=1$, $\beta\to1$ recovers $\alpha_{\rm crit}=30^\circ$, consistent with [Ogilvie's discussion of cold disk winds, section 9.9](https://arxiv.org/pdf/1604.03835).

## 4

↑ **Parent:** [Paper 314](paper-314.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For an [axisymmetric vector field](../../../calculus.md#axisymmetric-vector-field), write $\mathbf B=B_R\mathbf e_R+B_\phi\mathbf e_\phi+B_z\mathbf e_z$. Pure [differential rotation](../../../astrophysical-fluid-dynamics.md#differential-rotation) gives

$$
\mathbf u\times\mathbf B=R\Omega B_z\mathbf e_R-R\Omega B_R\mathbf e_z.
$$

This vector has no azimuthal component and is independent of $\phi$, so its [curl](../../../calculus.md#curl) has zero radial and vertical components. Its azimuthal component is

$$
\{\nabla\times(\mathbf u\times\mathbf B)\}_\phi=\partial_z(R\Omega B_z)+\partial_R(R\Omega B_R)
=R(B_z\partial_z\Omega+B_R\partial_R\Omega)+\Omega\{R\partial_zB_z+\partial_R(RB_R)\}.
$$

The final braces are $R\nabla\cdot\mathbf B=0$ by [Gauss's law for magnetism](../../../electromagnetism.md#gauss-s-law-for-magnetism). The [ideal magnetohydrodynamic induction equation](../../../astrophysical-fluid-dynamics.md#ideal-magnetohydrodynamic-induction-equation) therefore yields [axisymmetric magnetic winding](../../../astrophysical-fluid-dynamics.md#axisymmetric-magnetic-winding):

$$
\boxed{\partial_t\mathbf B=R(\mathbf B_p\cdot\nabla\Omega)\mathbf e_\phi,\qquad\partial_t\mathbf B_p=0.}
$$

[Differential rotation](../../../astrophysical-fluid-dynamics.md#differential-rotation) creates a [toroidal magnetic field](../../../astrophysical-fluid-dynamics.md#toroidal-magnetic-field) from the fixed [poloidal magnetic field](../../../astrophysical-fluid-dynamics.md#poloidal-magnetic-field). A stationary field under the same purely rotational assumptions requires [Ferraro's law of isorotation](../../../astrophysical-fluid-dynamics.md#ferraro-s-law-of-isorotation), $\mathbf B_p\cdot\nabla\Omega=0$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $M$ be the central stellar mass and take positive [Keplerian rotation](../../../astrophysics.md#keplerian-disk), $\Omega(R)=\sqrt{GM/R^3}$. The initial [poloidal magnetic field](../../../astrophysical-fluid-dynamics.md#poloidal-magnetic-field) stays fixed by part (a), while $R\Omega'(R)=-(3/2)\Omega(R)$. Integrating the toroidal induction equation with $B_\phi(R,0)=0$ gives

$$
\boxed{B_R(R,t)=B_0\frac{R_0}{R},\qquad B_z(R,t)=0,\qquad B_\phi(R,t)=-\frac32\Omega(R)t\,B_0\frac{R_0}{R}.}
$$

The initial field is a [solenoidal vector field](../../../calculus.md#solenoidal-vector-field) on the disk region $R>0$, since $\partial_R(RB_R)=0$. Assuming $B_0\ne0$, the amplitude ratio is

$$
\frac{|B_\phi|}{|\mathbf B_p|}=\frac32\Omega t.
$$

It reaches one at

$$
\boxed{t_{\phi=p}=\frac2{3\Omega(R)}=\frac{P_{\rm orb}(R)}{3\pi},\qquad P_{\rm orb}=\frac{2\pi}{\Omega}.}
$$

Thus the equality time is the same fraction $1/(3\pi)\approx0.106$ of the orbital period at every radius. If “orbital time” instead means $\Omega^{-1}$, the corresponding fraction is $2/3$. These are kinematic solutions with prescribed rotation and the neglected magnetic back-reaction.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

In the Gaussian units of the paper, the total [magnetic pressure](../../../astrophysical-fluid-dynamics.md#magnetic-pressure) is $p_B=(B_R^2+B_\phi^2)/(8\pi)$. Define the initial [plasma beta](../../../astrophysics.md#plasma-beta) $\beta_p=8\pi p_0/B_0^2\gg1$, assuming a nonzero initial field. The solution from part (b) gives

$$
p_B(R,t)=\frac{B_0^2}{8\pi}\left(\frac{R_0}{R}\right)^2\left[1+\frac94\frac{GMt^2}{R^3}\right],\qquad
\frac{p_B}{p}=\frac1{\beta_p}\left[1+\frac{9GMt^2}{4R^3}\right].
$$

For any $t>0$ this ratio decreases strictly with $R$, tends to infinity as $R\downarrow0$ and tends to $1/\beta_p<1$ as $R\to\infty$. The [magnetic-pressure equality radius under Keplerian winding](../../../astrophysical-fluid-dynamics.md#magnetic-pressure-equality-radius-under-keplerian-winding) is therefore unique in the formal profile on $R>0$:

$$
\boxed{R_{\rm eq}(t)=\left[\frac{9GM}{4(\beta_p-1)}\right]^{1/3}t^{2/3},\qquad\zeta=\frac23.}
$$

The same expression proves $p_B>p$ for $R<R_{\rm eq}$ and $p_B<p$ for $R>R_{\rm eq}$. At equality, $|B_\phi|/|B_R|=\sqrt{\beta_p-1}\gg1$, justifying the toroidal-dominated approximation

$$
R_{\rm eq}\simeq\left(\frac{9B_0^2GM}{32\pi p_0}\right)^{1/3}t^{2/3}.
$$

The source's existence claim refers to the indefinitely extended radial profile and the stated neglect of back-reaction. For a disk with a finite inner and outer edge, an equality radius lies in the disk only while the displayed value lies between those edges. If the initial field were zero, no magnetic winding or equality radius would occur.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2018](../../2018.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
