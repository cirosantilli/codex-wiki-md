# Paper 76

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_76.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_76.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
- [3](#3)
  - [Solution](#3/solution)

## 1

↑ **Parent:** [Paper 76](paper-76.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For the [long-wave convection equation with broken Boussinesq symmetry](../../../fluid-mechanics.md#long-wave-convection-equation-with-broken-boussinesq-symmetry), use a sufficiently smooth real temperature field. To make the spatial average and integrations meaningful, take a periodic pattern, or an existing long-interval average with bounded derivatives and vanishing averaged endpoint fluxes. Boundedness of the temperature alone does not guarantee all those averaging properties. Multiply the evolution equation by $\Theta$ and average. [Integration by parts](../../../calculus.md#integration-by-parts) gives

$$
\langle\Theta\Theta_{xx}\rangle=-\langle\Theta_x^2\rangle,\qquad
\langle\Theta\Theta_{xxxx}\rangle=\langle\Theta_{xx}^2\rangle,
$$

and $\langle\Theta(\Theta_x^j)_x\rangle=-\langle\Theta_x^{j+1}\rangle$. Thus the [energy method](../../../numerical-analysis.md#energy-method) yields

$$
\boxed{\frac12\frac d{dt}\langle\Theta^2\rangle
=-\langle\Theta^2\rangle+\mu\langle\Theta_x^2\rangle
-\langle\Theta_{xx}^2\rangle+s\langle\Theta_x^3\rangle
-\langle\Theta_x^4\rangle.}
$$

The [energy square completion for long-wave convection](../../../fluid-mechanics.md#energy-square-completion-for-long-wave-convection) starts from

$$
\langle(\Theta+\Theta_{xx})^2\rangle
=\langle\Theta^2\rangle-2\langle\Theta_x^2\rangle
+\langle\Theta_{xx}^2\rangle\geq0.
$$

Put $v=\Theta_x$. The energy identity becomes

$$
\frac12\frac d{dt}\langle\Theta^2\rangle
=-\langle(\Theta+\Theta_{xx})^2\rangle
+\langle(\mu-2)v^2+sv^3-v^4\rangle.
$$

Since $sv-v^2=s^2/4-(v-s/2)^2\leq s^2/4$ pointwise,

$$
\boxed{\frac12\frac d{dt}\langle\Theta^2\rangle
\leq\langle(\mu-2)\Theta_x^2+s\Theta_x^3-\Theta_x^4\rangle
\leq(\mu-2+s^2/4)\langle\Theta_x^2\rangle.}
$$

Therefore **$\mu<2-s^2/4$ excludes growth of the mean-square temperature**, for arbitrary amplitude within this smooth averaging class. This is a nonlinear energy-stability criterion, not a proof of pointwise monotonicity at each position. A spatially constant component instead decays through the $-\Theta$ term. The criterion is sufficient; it need not coincide with the linear instability threshold.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

For the [second-harmonic feedback in a long-wave convection amplitude equation](../../../fluid-mechanics.md#second-harmonic-feedback-in-a-long-wave-convection-amplitude-equation), at $\mu=2$ the linear steady operator is $L_0=-(1+\partial_x^2)^2$. Its [eigenvalue](../../../linear-operator-theory.md#eigenvalue) on $e^{inx}$ is $-(1-n^2)^2$, so the critical [Fourier modes](../../../fourier-analysis.md#fourier-mode) are $n=\pm1$. More generally the linear [dispersion relation](../../../wave-equation.md#dispersion-relation) is $\lambda(k)=-1+\mu k^2-k^4$, giving first onset at $\mu=2,k=1$.

At order $\epsilon^2$, the [weakly nonlinear expansion](../../../differential-equation.md#weakly-nonlinear-expansion) gives

$$
L_0\Theta_2=s(\Theta_{1x}^2)_x.
$$

With $\Theta_1=Ae^{ix}+\overline A e^{-ix}$,

$$
\Theta_{1x}^2=-A^2e^{2ix}-\overline A^{\,2}e^{-2ix}+2|A|^2.
$$

The constant part disappears under differentiation. Inverting $L_0$ on the second harmonic, whose [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is $-9$, gives

$$
\boxed{\Theta_2=\frac{2is}{9}A^2e^{2ix}+\mathrm{c.c.}}
$$

up to a critical-harmonic correction absorbed into the definition of $A$. At order $\epsilon^3$,

$$
0=L_0\Theta_3-\mu_2\Theta_{1xx}
-2s(\Theta_{1x}\Theta_{2x})_x+(\Theta_{1x}^3)_x.
$$

The coefficient of $e^{ix}$ in the last three terms is respectively

$$
\mu_2A,\qquad \frac{8s^2}{9}|A|^2A,\qquad -3|A|^2A.
$$

The [Fredholm solvability condition](../../../analysis.md#fredholm-solvability-condition) requires their sum to vanish, because $L_0$ annihilates the critical [Fourier mode](../../../fourier-analysis.md#fourier-mode). For a nonzero amplitude,

$$
\boxed{|A|^2=p(s)\mu_2,\qquad p(s)=\frac9{27-8s^2}.}
$$

This requires $\mu_2/(3-8s^2/9)>0$. The cubic amplitude coefficient is positive for $s^2<27/8$, yielding a small-amplitude branch in a [supercritical bifurcation](../../../dynamical-systems.md#supercritical-bifurcation); it is negative for $s^2>27/8$, yielding a [subcritical bifurcation](../../../dynamical-systems.md#subcritical-bifurcation) branch in this leading approximation. At **$s^2=27/8$**, the cubic coefficient vanishes and the quoted relation is singular: higher-order nonlinear terms and a different detuning balance are needed. One must not assert a finite $p$ there.

If a term $\epsilon\mu_1$ were included in $\mu$, order $\epsilon^2$ would also contain $-\mu_1\Theta_{1xx}=\mu_1\Theta_1$. The quadratic nonlinearity produces only the zeroth and second harmonics, with the zeroth differentiated away, so it cannot balance a first-harmonic contribution at that order. Solvability would give $\mu_1A=0$. Hence **a nontrivial critical-mode expansion forces $\mu_1=0$** and first balances detuning against cubic amplitude effects at order $\epsilon^3$.

## 2

↑ **Parent:** [Paper 76](paper-76.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

The unforced onset is a stationary pattern-forming instability. Under a horizontal translation, the critical [Fourier mode](../../../fourier-analysis.md#fourier-mode) transforms as $A\mapsto e^{i\phi}A$. A cubic [amplitude equation](../../../dynamical-systems.md#amplitude-equation) without forcing must have the same phase weight: its leading terms are $\widetilde\mu A-c|A|^2A$. Reflection of the unforced spatial pattern conjugates $A$, permitting real coefficients in this stationary problem. They are determined by a [weakly nonlinear expansion](../../../differential-equation.md#weakly-nonlinear-expansion) and projection onto the [adjoint eigenfunction](../../../linear-operator-theory.md#adjoint-eigenfunction); symmetry alone does not calculate their values or guarantee a nonzero coupling.

Represent the third-harmonic forcing by a complex coefficient $F$ multiplying $e^{3ik_cx}$, whose phase weight is three. The product $F\overline A^{\,2}$ has weight $3-2=1$ and therefore resonates with the critical positive harmonic. Neither a direct third-harmonic term nor $F\overline A$ has the required [wavenumber](../../../wave-equation.md#wavenumber) balance. A travelling boundary pattern makes

$$
F(T)=\widetilde\epsilon\,e^{3i(\widetilde\Omega T+\delta)}.
$$

A response phase and the sign of its coefficient can be incorporated into $\delta$. The resulting [three-to-one spatially forced amplitude equation](../../../dynamical-systems.md#three-to-one-spatially-forced-amplitude-equation) is

$$
\boxed{A_T=\widetilde\mu A-c|A|^2A
+\widetilde\epsilon\,\overline A^{\,2}e^{3i(\widetilde\Omega T+\delta)}.}
$$

This retains the leading resonant forcing term, linear detuning and cubic saturation, while dropping higher powers and nonresonant harmonics. The forcing is weak, the unforced critical [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is near zero, and the amplitude varies on a slow time; very high forcing frequency outside that slow scaling would require a different averaging argument. Reduction to the specific saturating canonical form in part (i) additionally assumes $c>0$ and nonzero forcing.

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

For the [rotating-frame normalization of resonant amplitude forcing](../../../dynamical-systems.md#rotating-frame-normalization-of-resonant-amplitude-forcing), use a rotating phase, $A=B\exp[i(\widetilde\Omega T+\delta)]$. The real $\delta$ must occur inside the factor of $i$; the printed change of variables omits that $i$ on the phase constant. The correctly phased substitution gives

$$
B_T+i\widetilde\Omega B=\widetilde\mu B-c|B|^2B
+e\,\overline B^{\,2},\qquad e=\widetilde\epsilon>0.
$$

A negative real forcing coefficient can be made positive by changing the forcing phase. Assuming $c>0$, set

$$
B=\frac ec C,\qquad \mathcal T=\frac{e^2}{c}T,\qquad
\mu=\frac{c\widetilde\mu}{e^2},\qquad
\omega=\frac{c\widetilde\Omega}{e^2}.
$$

All three terms then have the same coefficient scale, giving

$$
\boxed{C_{\mathcal T}+i\omega C
=\mu C-|C|^2C+\overline C^{\,2}.}
$$

Renaming $\mathcal T$ as $T$ gives the requested canonical equation. This rescaling preserves forward time. If $c<0$, a forward-time normalization instead leaves a positive cubic term, and if $c=0$ a cubic normalization is impossible. If $e=0$, the unforced [Landau amplitude equation](../../../dynamical-systems.md#landau-amplitude-equation) must be treated separately. Thus the printed canonical form implicitly concerns saturation in a [supercritical bifurcation](../../../dynamical-systems.md#supercritical-bifurcation) with nonzero forcing.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

To find the [threefold phase-locked equilibria](../../../dynamical-systems.md#threefold-phase-locked-equilibria), write $C=Re^{i\theta}$ with $R>0$; separating real and imaginary parts gives

$$
\boxed{R_T=R(\mu-R^2)+R^2\cos3\theta,\qquad
\theta_T=-\omega-R\sin3\theta.}
$$

A steady state satisfies

$$
\cos3\theta_0=\frac{R_0^2-\mu}{R_0},\qquad
\sin3\theta_0=-\frac{\omega}{R_0},
$$

so

$$
\boxed{(\mu-R_0^2)^2+\omega^2=R_0^2.}
$$

Writing $y=R_0^2$ and $D=1+4\mu-4\omega^2$, the amplitude branches are

$$
\boxed{y_\pm=\mu+\frac12\pm\frac12\sqrt D.}
$$

There are two distinct positive roots for **$\mu>\omega^2-1/4$**, except at $(\mu,\omega)=(0,0)$, where $y_-=0$ and only the upper root is nonzero. Indeed their sum is positive in this range and their product is $\mu^2+\omega^2$. Below the fold condition there are none. At equality, there is one positive repeated root $y=\omega^2+1/4$, the [saddle-node bifurcation](../../../dynamical-systems.md#saddle-node-bifurcation) limit.

For each positive amplitude, the sine and cosine determine $3\theta_0$ modulo $2\pi$, giving three phases separated by $2\pi/3$. Thus the source's “two states” means **two amplitude branches modulo the threefold spatial symmetry**. Generically there are six nonzero complex equilibria, three on each branch, not literally two.

The polar [Jacobian matrix](../../../calculus.md#jacobian-matrix) at an equilibrium is

$$
J=\begin{pmatrix}
-\mu-y&3\omega R_0\\
\omega/R_0&3\mu-3y
\end{pmatrix},
\quad
\operatorname{tr}J=2\mu-4y,\quad
\det J=3y(2y-2\mu-1).
$$

On the lower branch, $\det J=-3y_-\sqrt D<0$, so it is a [saddle equilibrium](../../../dynamical-systems.md#saddle-equilibrium) and unstable. On the upper branch, $\det J=3y_+\sqrt D>0$ and

$$
\operatorname{tr}J=-2(\mu+1+\sqrt D)<0,
$$

because existence implies $\mu>-1/4$. Therefore **every upper-branch equilibrium is [asymptotically stable](../../../dynamical-systems.md#asymptotic-stability), and every lower-branch equilibrium is a [saddle equilibrium](../../../dynamical-systems.md#saddle-equilibrium)**, away from the degenerate endpoints. The [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are unchanged by the smooth polar coordinate transformation at $R_0>0$. The origin, not covered by those coordinates, has [eigenvalues](../../../linear-operator-theory.md#eigenvalue) $\mu\pm i\omega$ and is stable for $\mu<0$ and unstable for $\mu>0$.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

For $\omega\ne0$, put $\mu=\widehat\mu\omega^2$, $C=\omega z$ and $\tau=\omega T$, where $z=\widehat C$. Then $C_T=\omega^2z_\tau$ and division by $\omega^2$ gives

$$
\boxed{z_\tau+iz=\overline z^{\,2}
+\omega(\widehat\mu z-|z|^2z).}
$$

We may take $\omega>0$ without loss of the dynamics by conjugating the original equation if necessary; otherwise $\tau$ reverses the time orientation. The scaling is singular at $\omega=0$ and is not a transformation for that exactly zero-frequency case.

The [Hamiltonian limit of three-to-one forcing](../../../dynamical-systems.md#hamiltonian-limit-of-three-to-one-forcing) drops the terms proportional to $\omega$. For $z=x+iy$ the remaining real system is

$$
x_\tau=y+x^2-y^2,\qquad y_\tau=-x-2xy.
$$

The proposed [first integral](../../../differential-equation.md#first-integral) is

$$
\boxed{H=x^2+y^2+2x^2y-\frac23y^3
=|z|^2+\frac{z^3-\overline z^{\,3}}{3i}.}
$$

Indeed $x_\tau=H_y/2$ and $y_\tau=-H_x/2$, hence $H_\tau=0$. The unperturbed equation is a planar [Hamiltonian system](../../../classical-mechanics.md#hamiltonian-system), with a [center equilibrium](../../../dynamical-systems.md#center-equilibrium) at the origin and three [saddle equilibria](../../../dynamical-systems.md#saddle-equilibrium) at

$$
(x,y)=(0,1),\quad(\sqrt3/2,-1/2),\quad(-\sqrt3/2,-1/2).
$$

All [saddle equilibria](../../../dynamical-systems.md#saddle-equilibrium) have $H=1/3$. The factorization

$$
H-\frac13=(1+2y)\left[x^2-\frac{(y-1)^2}{3}\right]
$$

shows that their central separatrix consists of the three sides of an equilateral triangle. Each level **$0<H<1/3$ inside this triangle is a closed [periodic orbit](../../../dynamical-systems.md#periodic-orbit)**. Indeed, inside the triangle $0<r<1$ and $\partial_rH=2r(1+r\sin3\theta)>0$. Each ray from the origin therefore meets each such level once, giving a compact simple closed contour with no [equilibrium point](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) on it. The nonzero vector field traverses this contour periodically; the period grows without bound as the separatrix is approached. This supplies an infinite family, not a claim that every level outside the central region is closed.

<a id="2/iii/image-periodic-orbits-inside-the-triangular-heteroclinic-cycle-of-a-hamiltonian-system"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-76-hamiltonian-orbits.png)

**[Figure 1](#2/iii/image-periodic-orbits-inside-the-triangular-heteroclinic-cycle-of-a-hamiltonian-system). Periodic orbits inside the triangular heteroclinic cycle of a Hamiltonian system**.

Restore the small radial perturbation. Its exact effect on the [first integral](../../../differential-equation.md#first-integral) is

$$
H_\tau=\omega(\widehat\mu-r^2)(xH_x+yH_y)
=2\omega(\widehat\mu-r^2)r^2(1+r\sin3\theta),\qquad r=|z|.
$$

Consequently the continuum of [Hamiltonian system](../../../classical-mechanics.md#hamiltonian-system) orbits generally does not persist. The origin becomes a weak attracting focus for $\widehat\mu<0$ or a repelling focus for $\widehat\mu>0$, and the three hyperbolic [saddle equilibria](../../../dynamical-systems.md#saddle-equilibrium) persist with perturbed [stable manifold](../../../dynamical-systems.md#stable-manifold) and [unstable manifold](../../../dynamical-systems.md#unstable-manifold). For a small positive $\widehat\mu$, outward drift on very small orbits balances cubic damping on somewhat larger ones, selecting a stable [limit cycle](../../../dynamical-systems.md#limit-cycle) rather than an arbitrary energy level. Near the [center equilibrium](../../../dynamical-systems.md#center-equilibrium) $H\simeq r^2$, so its leading radius is $r\simeq\sqrt{\widehat\mu}$ when $\widehat\mu$ is also small.

For a more general closed unperturbed orbit $\Gamma_h$, the [averaged area criterion for perturbed Hamiltonian cycles](../../../dynamical-systems.md#averaged-area-criterion-for-perturbed-hamiltonian-cycles) says that persistence requires the averaged energy drift $\oint_{\Gamma_h}H_\tau\,d\tau$ to vanish. Since the unperturbed speed is $|\nabla H|/2$, the planar [divergence theorem](../../../calculus.md#divergence-theorem) converts this leading drift to

$$
\oint_{\Gamma_h}H_\tau\,d\tau
=4\omega\left[\widehat\mu\,|\mathcal D_h|
-2\int_{\mathcal D_h}r^2\,dA\right],
$$

where $\mathcal D_h$ is the enclosed region. Isolated zeros select candidate [periodic orbits](../../../dynamical-systems.md#periodic-orbit); a drift changing from positive inside to negative outside gives an attracting [limit cycle](../../../dynamical-systems.md#limit-cycle). The separatrix triangle has mean $r^2=1/4$, so its leading flux changes sign at $\widehat\mu=1/2$. This marks the leading possible heteroclinic transition, with higher-order corrections needed to locate it precisely.

As a cycle approaches the [saddle equilibria](../../../dynamical-systems.md#saddle-equilibrium), long residence times and splitting of the [heteroclinic cycle](../../../dynamical-systems.md#heteroclinic-cycle) become important. Orbits can instead drift inward to the [equilibrium point](../../../dynamical-systems.md#equilibrium-point-of-a-dynamical-system) at the origin or leave the periodic island and approach one of the stable states with [phase locking](../../../dynamical-systems.md#phase-locking) of the full canonical equation. Those upper-branch [threefold phase-locked equilibria](../../../dynamical-systems.md#threefold-phase-locked-equilibria) have $C=O(1)$, so they lie outside the local $C=O(\omega)$ scaling. Thus the small perturbation gives energy selection, attracting or repelling oscillations, and possible switching/locking transitions; it does not preserve a conserved $H$ or an infinite family of neutral periodic solutions. This qualitative picture does not assume all global parameter values have the same attractor.

## 3

↑ **Parent:** [Paper 76](paper-76.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

[Rotating Rayleigh-Bénard convection](../../../viscous-fluid-flow.md#rotating-rayleigh-benard-convection) combines buoyancy-driven instability with the [Coriolis force](../../../physics.md#coriolis-force). Consider a plane layer of depth $d$ rotating uniformly about the vertical axis, heated from below. Adopt the [Boussinesq approximation](../../../geophysical-fluid-dynamics.md#boussinesq-approximation), fixed boundary temperatures and, for explicit formulas, impermeable [stress-free boundary conditions](../../../viscous-fluid-flow.md#stress-free-boundary-condition). The [conductive state of Rayleigh-Bénard convection](../../../viscous-fluid-flow.md#conductive-state-of-rayleigh-benard-convection) is motionless with a linear temperature profile. The dimensionless controls are the [Rayleigh number](../../../geophysics.md#rayleigh-number), [Prandtl number](../../../thermodynamics.md#prandtl-number) and [Taylor number](../../../geophysical-fluid-dynamics.md#taylor-number):

$$
\operatorname{Ra}=\frac{g\alpha_T\Delta T\,d^3}{\nu\kappa},\qquad
P=\operatorname{Pr}=\frac{\nu}{\kappa},\qquad
\operatorname{Ta}=\left(\frac{2\Omega d^2}{\nu}\right)^2.
$$

Here $\nu$ is [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity) and $\kappa$ [thermal diffusivity](../../../thermodynamics.md#thermal-diffusivity). In thermal-diffusion time units, linear perturbations satisfy

$$
P^{-1}\boldsymbol u_t+\sqrt{\operatorname{Ta}}\,\boldsymbol e_z\times\boldsymbol u
=-\nabla p+\nabla^2\boldsymbol u+\operatorname{Ra}\,\theta\boldsymbol e_z,
\qquad
\theta_t=w+\nabla^2\theta,\qquad\nabla\cdot\boldsymbol u=0.
$$

Rotation does no direct mechanical work, since $\boldsymbol u\cdot(\boldsymbol e_z\times\boldsymbol u)=0$, but couples vertical motion to vertical [vorticity](../../../fluid-mechanics.md#vorticity) and changes the damping and oscillation balance.

For horizontal [wavenumber](../../../wave-equation.md#wavenumber) $k$ and vertical mode $n$, put $m=n^2\pi^2$ and $a=k^2+m$. Use $w=W\sin(n\pi z)$, $\theta=\Theta\sin(n\pi z)$ and vertical [vorticity](../../../fluid-mechanics.md#vorticity) $\zeta=Z\cos(n\pi z)$ with growth rate $\sigma$. Curling the momentum equation and eliminating pressure gives

$$
a(\sigma/P+a)W+\sqrt{\operatorname{Ta}}\,n\pi Z
=\operatorname{Ra}k^2\Theta,\quad
(\sigma/P+a)Z=\sqrt{\operatorname{Ta}}\,n\pi W,\quad
(\sigma+a)\Theta=W.
$$

Their determinant, without dividing by a possibly zero factor, is the [rotating-convection growth-rate polynomial](../../../viscous-fluid-flow.md#rotating-convection-growth-rate-polynomial)

$$
(\sigma+a)\left[a(\sigma/P+a)^2+\operatorname{Ta}m\right]
-\operatorname{Ra}k^2(\sigma/P+a)=0.
$$

This makes the [linear stability analysis](../../../dynamical-systems.md#linear-stability) question precise: onset occurs when a root reaches zero real part and all other modes still decay.

A stationary neutral root has $\sigma=0$, giving

$$
\boxed{R_s(k,n)=\frac{a^3+\operatorname{Ta}m}{k^2}.}
$$

Rotation raises this stationary threshold. An oscillatory neutral root has $\sigma=i\varpi$ with $\varpi\ne0$. Real-imaginary separation gives the [oscillatory neutral curve of rotating convection](../../../viscous-fluid-flow.md#oscillatory-neutral-curve-of-rotating-convection)

$$
\boxed{\varpi^2=P^2\left[
\frac{1-P}{1+P}\frac{\operatorname{Ta}m}{a}-a^2\right],\qquad
R_o(k,n)=\frac{2(1+P)a^3+2P^2\operatorname{Ta}m/(1+P)}{k^2}.}
$$

This branch is admissible only when $\varpi^2>0$, requiring $P<1$ and sufficiently strong rotation. The restoring [Coriolis force](../../../physics.md#coriolis-force) coupling permits an inertial/thermal oscillation whose phase-lagged buoyancy can overcome dissipation. At large $P$, temperature and momentum diffusion do not permit that overstability mechanism at primary onset, so the exchange of stabilities is stationary. The actual threshold is the minimum of the stationary and admissible oscillatory curves over all allowed modes, not an arbitrary formal value of $R_o$. Rigid plates require a different vertical eigenproblem and [Ekman layers](../../../geophysical-fluid-dynamics.md#ekman-layer), so the explicit free-slip numbers are not universal.

At large [Taylor number](../../../geophysical-fluid-dynamics.md#taylor-number), the first vertical mode is selected in the ideal plane layer. Let $t=k^2,m=\pi^2$. Minimizing the stationary curve gives

$$
(t+m)^2(2t-m)=\operatorname{Ta}m.
$$

Thus the [stationary neutral curve of rotating convection](../../../viscous-fluid-flow.md#stationary-neutral-curve-of-rotating-convection) has

$$
\boxed{k_{s,c}\sim(\operatorname{Ta}\pi^2/2)^{1/6},\qquad
R_{s,c}\sim3(\operatorname{Ta}\pi^2/2)^{2/3}.}
$$

The physical horizontal wavelength is $2\pi d/k_c$, hence decreases as $\operatorname{Ta}^{-1/6}$; its prefactor depends on the boundary convention. Thin nearly vertical cells reconcile the strong [Coriolis force](../../../physics.md#coriolis-force) constraint with viscous and thermal diffusion. The oscillatory minimization replaces the right side of the [wavenumber](../../../wave-equation.md#wavenumber) equation by $P^2\operatorname{Ta}m/(1+P)^2$, giving the same [Taylor number](../../../geophysical-fluid-dynamics.md#taylor-number) exponent at fixed positive $P$. Where its frequency remains admissible,

$$
\frac{R_{o,c}}{R_{s,c}}\sim\frac{2P^{4/3}}{(1+P)^{1/3}}.
$$

Equality is $8P^4-P-1=0$, whose positive root is approximately **$P_*=0.6766$**. Accordingly, for sufficiently rapid rotation in this free-slip problem, $P<P_*$ selects oscillatory onset and $P>P_*$ stationary onset. The weaker condition $P<1$ is only necessary for an oscillatory neutral mode; it does not by itself identify the first instability. Finite [Taylor number](../../../geophysical-fluid-dynamics.md#taylor-number), finite lateral geometry, allowed discrete wave numbers and plate conditions change the selection.

For the [counterpropagating Hopf amplitudes in rotating convection](../../../viscous-fluid-flow.md#counterpropagating-hopf-amplitudes-in-rotating-convection) near a simple oscillatory onset, the [Hopf bifurcation](../../../dynamical-systems.md#hopf-bifurcation) produces slow complex amplitudes for counterpropagating roll waves. After separating the fast carrier oscillation, symmetry permits the cubic equations

$$
\dot Z_\pm=rZ_\pm-
\left(g_s|Z_\pm|^2+g_c|Z_\mp|^2\right)Z_\pm,
$$

with generally complex coefficients; an $i\omega_0 Z_\pm$ term restores the fast frequency if desired. The real parts govern amplitude saturation and the imaginary parts give nonlinear frequency shifts. Write $a_s=\operatorname{Re}g_s$, $a_c=\operatorname{Re}g_c$. For a [travelling wave](../../../analysis.md#travelling-wave) from a [supercritical bifurcation](../../../dynamical-systems.md#supercritical-bifurcation) with only one amplitude nonzero, $|Z_\pm|^2=r/a_s$ with $r,a_s>0$, and the competing wave's growth rate is $r(1-a_c/a_s)$. It is amplitude-stable against that competitor when $a_c>a_s$. A [standing wave](../../../physics.md#standing-wave) has equal intensities $r/(a_s+a_c)$; provided this is positive, its intensity-difference mode is stable when $a_s>a_c$. Temporal and spatial phase symmetries leave neutral phase directions, so these are orbital/amplitude stability statements, not decay of every phase displacement.

These coefficients follow from nonlinear interactions and the [Fredholm solvability condition](../../../analysis.md#fredholm-solvability-condition) obtained by projection onto an [adjoint eigenfunction](../../../linear-operator-theory.md#adjoint-eigenfunction); symmetry alone cannot decide their signs. A negative saturating coefficient gives [subcritical bifurcation](../../../dynamical-systems.md#subcritical-bifurcation) behavior requiring higher-order terms. Spatial modulation leads to coupled [complex Ginzburg–Landau equations](../../../partial-differential-equation.md#complex-ginzburg-landau-equation) with [group velocities](../../../wave-equation.md#group-velocity) and diffusion; phase instabilities, mean-flow coupling and differently oriented rolls can destabilize a wave stable in the restricted two-amplitude system. A [weakly nonlinear expansion](../../../differential-equation.md#weakly-nonlinear-expansion) of oscillations therefore predicts [travelling waves](../../../analysis.md#travelling-wave) or [standing waves](../../../physics.md#standing-wave), frequency shifts, modulation and possible secondary mode competition, not a unique universal periodic state.

The [Küppers–Lortz instability](../../../viscous-fluid-flow.md#kuppers-lortz-instability) is a different route to time dependence: it destabilizes steady saturated rolls against oblique roll perturbations. For stationary-roll amplitudes of orientations $\phi_j$, a leading competition system has

$$
\dot A_i=rA_i-g_0|A_i|^2A_i
-\sum_{j\ne i}g(\phi_j-\phi_i)|A_j|^2A_i.
$$

A pure roll has $|A_i|^2=r/g_0$ with $g_0>0$. An infinitesimal new roll at relative angle $\vartheta$ grows at

$$
\boxed{\lambda_{\rm inv}=r\left[1-\frac{g(\vartheta)}{g_0}\right].}
$$

For sufficiently strong rotation in appropriate boundary and [Prandtl number](../../../thermodynamics.md#prandtl-number) regimes, some finite oblique angle has $g(\vartheta)<g_0$, so a steady roll is unstable arbitrarily close above its stationary onset. Rotation is handed and allows $g(\vartheta)\ne g(-\vartheta)$, so replacement of one roll by another can favor a definite cyclic sense. Three or more competing orientations can form a [heteroclinic cycle](../../../dynamical-systems.md#heteroclinic-cycle); whether it attracts depends on contraction/expansion rates and other modes. Noise, spatially varying domains and modulation can turn this competition into repeated orientation switching and irregular patterns.

The invading rolls are three-dimensional disturbances even when the original straight roll is described by a two-dimensional section. The finite-angle [Küppers–Lortz instability](../../../viscous-fluid-flow.md#kuppers-lortz-instability) mechanism should also be distinguished from the [small-angle instability of rotating convection rolls](../../../viscous-fluid-flow.md#small-angle-instability-of-rotating-convection-rolls) mediated by large-scale mean flow at finite [Prandtl number](../../../thermodynamics.md#prandtl-number). Numerical thresholds and favored angles depend on mechanical boundaries and material parameters; the essential criterion is the cross-coupling relative to self-saturation. **Rotation both changes primary onset and wavelength, and can prevent the resulting steady roll pattern from remaining a stable nonlinear state.**

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
