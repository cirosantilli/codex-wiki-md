# Paper 77

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_77.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2012/paper_77.pdf)

**Table of contents**

- [Section I](#section-i)
  - [1](#1)
    - [Solution](#1/solution)
  - [2](#2)
    - [i](#2/i)
      - [Solution](#2/i/solution)
    - [ii](#2/ii)
      - [Solution](#2/ii/solution)
    - [iii](#2/iii)
      - [Solution](#2/iii/solution)
- [Section II](#section-ii)
  - [3](#3)
    - [a](#3/a)
      - [Solution](#3/a/solution)
    - [b](#3/b)
      - [Solution](#3/b/solution)
  - [4](#4)
    - [Solution](#4/solution)
- [Section III](#section-iii)
  - [5](#5)
    - [i](#5/i)
      - [Solution](#5/i/solution)
    - [ii](#5/ii)
      - [Solution](#5/ii/solution)
    - [iii](#5/iii)
      - [Solution](#5/iii/solution)

## Section I

↑ **Parent:** [Paper 77](paper-77.md)

### 1

↑ **Parent:** [Section I](#section-i)

<h4 id="1/solution">Solution</h4>

↑ **Parent:** [1](#1)

Use the layer depth $d$, the thermal diffusion time $d^2/\kappa$, velocity $\kappa/d$, and the imposed temperature difference $\Delta T$ as scales. Let $\theta$ be the temperature departure from the conductive profile, $\mathbf u$ the velocity, $w=\mathbf u\cdot\hat{\mathbf z}$, and let pressure absorb hydrostatic terms. The dimensionless [Boussinesq equations](../../../geophysical-fluid-dynamics.md#boussinesq-equations) for [Rayleigh-Bénard convection](../../../viscous-fluid-flow.md#rayleigh-benard-convection) are

$$
\nabla\cdot\mathbf u=0,\qquad \frac1\sigma(\partial_t\mathbf u+\mathbf u\cdot\nabla\mathbf u)=-\nabla p+R\theta\hat{\mathbf z}+\nabla^2\mathbf u,\qquad \partial_t\theta+\mathbf u\cdot\nabla\theta=w+\nabla^2\theta.
$$

The [Prandtl number](../../../thermodynamics.md#prandtl-number) and [Rayleigh number](../../../geophysics.md#rayleigh-number) are $\sigma=\nu/\kappa$ and $R=g\alpha_T\Delta T d^3/(\nu\kappa)$, with [kinematic viscosity](../../../fluid-mechanics.md#kinematic-viscosity) $\nu$, [thermal diffusivity](../../../thermodynamics.md#thermal-diffusivity) $\kappa$ and [coefficient of thermal expansion](../../../thermodynamics.md#coefficient-of-thermal-expansion) $\alpha_T$. At $z=0,1$, the [stress-free boundary condition](../../../viscous-fluid-flow.md#stress-free-boundary-condition) and [perfectly conducting thermal boundary condition](../../../differential-equation.md#perfectly-conducting-thermal-boundary-condition) give $w=0$, $\partial_z u_x=\partial_z u_y=0$, and $\theta=0$.

For the fundamental vertical [normal mode](../../../wave-equation.md#normal-mode), take $w=W\sin(\pi z)e^{i\mathbf k\cdot\mathbf x+\lambda t}$ and $\theta=\vartheta\sin(\pi z)e^{i\mathbf k\cdot\mathbf x+\lambda t}$. Here $k=|\mathbf k|>0$ is the horizontal [wavenumber](../../../wave-equation.md#wavenumber). With $s=k^2+\pi^2$, projection onto [incompressible flow](../../../fluid-mechanics.md#incompressible-flow) eliminates pressure and gives

$$
(\lambda/\sigma+s)sW=Rk^2\vartheta,\qquad (\lambda+s)\vartheta=W.
$$

Thus the [stress-free convection growth-rate polynomial](../../../viscous-fluid-flow.md#stress-free-convection-growth-rate-polynomial) is $(\lambda+\sigma s)(\lambda+s)=\sigma Rk^2/s$.

For the infinite-[Prandtl number](../../../thermodynamics.md#prandtl-number) limit, the finite thermal growth rate is

$$
\boxed{\lambda_\infty(k)=\frac{Rk^2}{(k^2+\pi^2)^2}-(k^2+\pi^2).}
$$

The other, viscously damped root tends to $-\sigma s$. For $\sigma=1$, both roots are explicit:

$$
\boxed{\lambda_\pm(k)=-s\pm\sqrt{\frac{Rk^2}{s}}.}
$$

The plus root determines instability. A higher vertical harmonic replaces $\pi^2$ by $n^2\pi^2$; the fundamental is the most favorable one.

For the large-$R$ maximum in the infinite-[Prandtl number](../../../thermodynamics.md#prandtl-number) limit, put $x=k^2$ and $p=\pi^2$. Differentiating gives $d\lambda_\infty/dx=R(p-x)/(p+x)^3-1$. The unique maximum for sufficiently large $R$ therefore satisfies $R(p-x)=(p+x)^3$, whence

$$
\boxed{k_{\rm max}^2=p-\frac{8p^3}{R}+O(R^{-2})\simeq\pi^2,\qquad \lambda_{\rm max}=\frac{R}{4\pi^2}-2\pi^2+O(R^{-1})\simeq\frac{R}{4\pi^2}.}
$$

This is [fastest growth in infinite-Prandtl convection](../../../viscous-fluid-flow.md#fastest-growth-in-infinite-prandtl-convection). The large-$R$ expansion is taken after the infinite-[Prandtl number](../../../thermodynamics.md#prandtl-number) limit; at finite $\sigma$, neglecting inertia additionally requires $|\lambda|\ll\sigma s$. It selects the fastest growing mode far above onset, rather than the neutral-curve minimum $k^2=\pi^2/2$.

### 2

↑ **Parent:** [Section I](#section-i)

<h4 id="2/i">i</h4>

↑ **Parent:** [2](#2)

<h5 id="2/i/solution">Solution</h5>

↑ **Parent:** [I](#2/i)

The [Lorenz model of thermosolutal convection](../../../fluid-mechanics.md#lorenz-model-of-thermosolutal-convection) is a [Galerkin method](../../../partial-differential-equation.md#galerkin-method) truncation retaining a roll velocity and the leading temperature and concentration modes. The variable $a$ measures the roll velocity; $b$ is the temperature mode correlated with the vertical motion, while $c$ is the horizontally averaged temperature-profile distortion generated by that motion. The corresponding concentration modes are $d$ and $e$. The symbol $d$ in this model is a solute amplitude, not the dimensional layer depth. The terms $ab$ and $ad$ change the mean scalar profiles; $a(1-c)$ and $a(1-e)$ express advection of the remaining background gradients.

The positive parameters are the [Prandtl number](../../../thermodynamics.md#prandtl-number) $\sigma=\nu/\kappa$, the ratio $\tau=\kappa_s/\kappa$ of [solutal diffusivity](../../../brownian-motion.md#solutal-diffusivity) to [thermal diffusivity](../../../thermodynamics.md#thermal-diffusivity), and the geometric vertical-mode decay ratio $\varpi$. In the usual fundamental-roll truncation with time normalized to the thermal roll-mode decay rate, $\varpi=4\pi^2/(k^2+\pi^2)$; treating it as an independently specified positive truncation parameter leaves the arguments below unchanged.

The parameter $r$ is the destabilizing thermal [Rayleigh number](../../../geophysics.md#rayleigh-number) divided by the free-slip critical-mode value, and $r_s>0$ measures stabilizing solutal buoyancy in the same thermal-diffusive normalization. For example, using a positive bottom-to-top stabilizing solute difference $\Delta S$ and density coefficient $\beta_S$,

$$
r=\frac{g\alpha_T\Delta T d_{\rm layer}^3}{\nu\kappa R_0(k)},\qquad r_s=\frac{g\beta_S\Delta S d_{\rm layer}^3}{\nu\kappa R_0(k)},\qquad R_0(k)=\frac{(k^2+\pi^2)^3}{k^2}.
$$

If a solutal [Rayleigh number](../../../geophysics.md#rayleigh-number) is instead defined with $\kappa_s$ in its denominator, the coefficient $r_s$ here is $\tau$ times that normalized number. **Thermal buoyancy drives the roll; solutal buoyancy opposes it and diffuses at a different rate.** This is the essential mechanism of [thermosolutal convection](../../../fluid-mechanics.md#thermosolutal-convection).

<h4 id="2/ii">ii</h4>

↑ **Parent:** [2](#2)

<h5 id="2/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/ii)

Set the time derivatives to zero. The scalar equations give

$$
b=\frac{a}{1+a^2},\qquad c=\frac{a^2}{1+a^2},\qquad d=\frac{a\tau}{\tau^2+a^2},\qquad e=\frac{a^2}{\tau^2+a^2}.
$$

For the nonzero convection branch, division of the velocity equation by $a$ gives

$$
\boxed{r(x)=(1+x)+\frac{r_s\tau(1+x)}{\tau^2+x},\qquad x=a^2\ge0.}
$$

Its zero-amplitude limit is $r_e=1+r_s/\tau$. Differentiation yields

$$
r'(x)=1-\frac{r_s\tau(1-\tau^2)}{(\tau^2+x)^2}.
$$

For $0<\tau<1$, the sharp condition for a [subcritical bifurcation](../../../dynamical-systems.md#subcritical-bifurcation) at the steady onset is $r_s>\tau^3/(1-\tau^2)$. The stronger bound printed in the question is sufficient, since $(1-\tau)^2<1-\tau^2$. Under it the branch initially runs toward smaller $r$, and the unique [saddle-node bifurcation](../../../dynamical-systems.md#saddle-node-bifurcation) has

$$
\boxed{x_*=a_*^2=-\tau^2+\sqrt{r_s\tau(1-\tau^2)}.}
$$

It is a genuine positive-amplitude minimum: $r''(x)=2r_s\tau(1-\tau^2)/(\tau^2+x)^3>0$. Put $h=\sqrt{r_s\tau}$ and $j=\sqrt{1-\tau^2}$. At the minimum, $1+x_*=j(j+h)$ and $\tau^2+x_*=hj$, so

$$
\boxed{r_{\rm min}=(h+j)^2=\left(\sqrt{r_s\tau}+\sqrt{1-\tau^2}\right)^2.}
$$

These results describe the [steady fold of a thermosolutal Lorenz model](../../../fluid-mechanics.md#steady-fold-of-a-thermosolutal-lorenz-model). They do not by themselves assert stability against every oscillatory disturbance.

<h4 id="2/iii">iii</h4>

↑ **Parent:** [2](#2)

<h5 id="2/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/iii)

Take $\beta\ge0$ without loss of generality, since its definition fixes only $\beta^2$. With $r_s=\beta^2\tau$, the steady-branch minimum expands as $r_{\rm min}=1+2\beta\tau+O(\tau^2)$. For fixed positive $\sigma$, the source's supplied approximation therefore gives

$$
r^{(0)}_{\rm supplied}-r_{\rm min}=\tau\left(\delta+\frac{\beta^2}{\delta}-2\beta\right)+O(\tau^2)=\frac{\tau}{\delta}(\beta-\delta)^2+O(\tau^2)\ge0\quad\text{to the retained order}.
$$

Thus **the requested inequality follows from the supplied approximation**, with equality at first order when $\beta=\delta$. If negative $\beta$ is retained, replace it by $|\beta|$ throughout.

There is an independent source-consistency issue with calling that supplied expression the oscillatory threshold of the displayed model. Linearizing about conduction, the $c,e$ modes decay separately and the $a,b,d$ characteristic polynomial is

$$
(\lambda+\sigma)(\lambda+1)(\lambda+\tau)-\sigma r(\lambda+\tau)+\sigma r_s(\lambda+1)=0.
$$

Writing it as $\lambda^3+A\lambda^2+B\lambda+C$, a nonzero imaginary pair requires $C=AB$ and $B>0$, by the [Routh-Hurwitz stability criterion](../../../dynamical-systems.md#routh-hurwitz-stability-criterion). Direct algebra gives the [oscillatory threshold of a thermosolutal Lorenz model](../../../fluid-mechanics.md#oscillatory-threshold-of-a-thermosolutal-lorenz-model)

$$
r_H=1+\frac{\tau(\sigma+1+\tau)}{\sigma}+\frac{\sigma+\tau}{\sigma+1}r_s,\qquad \omega_H^2=\frac{\sigma}{\sigma+1}r_s(1-\tau)-\tau^2.
$$

Consequently, with $\delta=\sigma/(1+\sigma)$,

$$
\boxed{r_H=1+\frac{\tau}{\delta}+\beta^2\tau\delta+O(\tau^2).}
$$

The two factors of $\delta$ in the supplied threshold are interchanged. For example $\sigma=1$, $\beta=2$, $\tau=10^{-3}$ gives a genuine marginal imaginary pair at $r_H=1.004003$, whereas the supplied first-order expression gives $1.0085$. The intended comparison remains true after correction:

$$
\boxed{r_H-r_{\rm min}=\frac{\tau}{\delta}(\beta\delta-1)^2+O(\tau^2)\ge0\text{ to first order}.}
$$

This comparison applies to a physical [Hopf bifurcation](../../../dynamical-systems.md#hopf-bifurcation) when $\omega_H^2>0$ and to an interior steady fold when $a_*^2>0$. For fixed nonzero $\beta$ and fixed $\sigma>0$, both conditions hold for sufficiently small positive $\tau$. At a vanishing squared difference, neglected terms must be examined before drawing a higher-order conclusion.

## Section II

↑ **Parent:** [Paper 77](paper-77.md)

### 3

↑ **Parent:** [Section II](#section-ii)

<h4 id="3/a">a</h4>

↑ **Parent:** [3](#3)

<h5 id="3/a/solution">Solution</h5>

↑ **Parent:** [A](#3/a)

For the [real-coefficient cubic-quintic amplitude equation](../../../partial-differential-equation.md#real-coefficient-cubic-quintic-amplitude-equation), the trivial pattern $A=0$ exists for every $\mu$. A nonzero spatially uniform pattern has arbitrary constant phase and intensity $q=|A|^2>0$ satisfying $\mu+\alpha q-q^2=0$. Thus

$$
\boxed{q_\pm=\frac{\alpha\pm\sqrt{\alpha^2+4\mu}}2.}
$$

Nonzero patterns exist for $\mu\ge-\alpha^2/4$. The upper branch $q_+$ exists throughout that range; a distinct positive lower branch $q_-$ exists only for $-\alpha^2/4<\mu<0$ and reaches zero at $\mu=0$.

For a homogeneous perturbation, write $A=Re^{i\phi}$. Then $\dot R=R(\mu+\alpha R^2-R^4)$ and $\dot\phi=0$. The radial eigenvalue at a nonzero pattern is

$$
\lambda_R=\mu+3\alpha q-5q^2=2q(\alpha-2q),
$$

while the phase eigenvalue is zero. Therefore **the upper branch is stable modulo its arbitrary phase for $\mu>-\alpha^2/4$; the lower branch is unstable.** The phase-neutral direction prevents asymptotic attraction to one particular complex amplitude, but permits [orbital stability](../../../dynamical-systems.md#orbital-stability) of the circle of equivalent patterns.

Conduction is asymptotically stable for $\mu<0$ and unstable for $\mu>0$. At $\mu=0$, the positive cubic term destabilizes arbitrarily small nonzero amplitudes, even though its linear eigenvalue vanishes. At $\mu=-\alpha^2/4$, the merged nonzero branch is semistable from above only: $\dot R=-R(R^2-\alpha/2)^2$, so amplitudes just below it eventually decrease toward zero. Thus the bistable interval is **$-\alpha^2/4<\mu<0$**, with the endpoints treated separately rather than declared stable merely because an eigenvalue is zero.

<h4 id="3/b">b</h4>

↑ **Parent:** [3](#3)

<h5 id="3/b/solution">Solution</h5>

↑ **Parent:** [B](#3/b)

For the intended nontrivial interface, take the limiting amplitude at the patterned end to be $R_->0$; the identically zero solution is otherwise a trivial exception. Splitting the stationary [real-coefficient cubic-quintic amplitude equation](../../../partial-differential-equation.md#real-coefficient-cubic-quintic-amplitude-equation) into real and imaginary parts gives

$$
R''-R(\phi')^2+\mu R+\alpha R^3-R^5=0,\qquad 2R'\phi'+R\phi''=0.
$$

The imaginary equation implies $R^2\phi'=J$, a constant. The radial first integral is

$$
\frac12(R')^2+\frac{J^2}{2R^2}+V(R)=E,\qquad V(R)=\frac\mu2R^2+\frac\alpha4R^4-\frac16R^6.
$$

A regular solution has finite $E$. As $R\to0$, the nonnegative $J^2/(2R^2)$ term would diverge unless $J=0$. Hence **$\phi'=0$ wherever the nontrivial front has positive amplitude**. This conclusion does not assume in advance that the patterned end has no phase gradient.

For a [heteroclinic orbit](../../../dynamical-systems.md#heteroclinic-orbit) connecting two constant states, $R'$ tends to zero at both ends. Thus $E=V(0)=0$, while the nonzero end must obey both $\mu+\alpha q-q^2=0$ and $V(\sqrt q)=0$. Eliminating $\mu$ gives

$$
0=\frac{q^3}{3}-\frac{\alpha q^2}{4},\qquad \boxed{q=\frac{3\alpha}{4},\quad\mu_M=-\frac{3\alpha^2}{16}<0.}
$$

This is the [stationary front of a cubic-quintic amplitude equation](../../../partial-differential-equation.md#stationary-front-of-a-cubic-quintic-amplitude-equation): a unique equal-potential parameter in the bistable interval.

Existence, not just a necessary condition, follows from the first integral. At $\mu_M$, $V(R)=-R^2(R^2-q)^2/6$. The descending solution obeys $R'=-R(q-R^2)/\sqrt3$, which integrates to

$$
\boxed{A(x)=e^{i\phi_0}\sqrt{\frac{3\alpha/4}{1+\exp[\sqrt3\alpha(x-x_0)/2]}}.}
$$

It connects the stable upper pattern at $x\to-\infty$ to conduction at $x\to+\infty$, with arbitrary translation $x_0$ and constant phase $\phi_0$.

### 4

↑ **Parent:** [Section II](#section-ii)

<h4 id="4/solution">Solution</h4>

↑ **Parent:** [4](#4)

Assume $\alpha>0$, so a finite nonzero critical [wavenumber](../../../wave-equation.md#wavenumber) exists. The linear growth rate of a [Fourier mode](../../../fourier-analysis.md#fourier-mode) is $\lambda(k)=-\alpha+\mu k^2-k^4$. Maximizing over $k$ and setting that maximum to zero gives

$$
\boxed{\mu_c=2\sqrt\alpha,\qquad k_c=\alpha^{1/4}.}
$$

Set $K=k_c^2=\sqrt\alpha$. The [resonant three-wave triad](../../../differential-equation.md#resonant-three-wave-triad) has wavevectors satisfy $\mathbf k_1+\mathbf k_2+\mathbf k_3=0$ and $\mathbf k_i\cdot\mathbf k_j=-K/2$ for $i\ne j$. With the slow time and amplitude scaling, every growth, quadratic and cubic term first enters at order $\epsilon^3$. Projection onto each critical mode removes the nonresonant correction $\Theta_3$ by the [method of multiple scales](../../../differential-equation.md#method-of-multiple-scales) solvability condition.

The parameter displacement contributes $\mu_2K A$ to the first mode. For the quadratic term, use $\nabla\cdot(\Theta_1\nabla\Theta_1)=\tfrac12\nabla^2(\Theta_1^2)$. The resonant coefficient of $\Theta_1^2$ at $\mathbf k_1$ is $2\bar B\bar C$, so its contribution is $+\gamma K\bar B\bar C$.

For the cubic gradient term, an ordered triple of modes with wavevectors $\mathbf p,\mathbf q,\mathbf r$ summing to $\mathbf k_1$ contributes $(\mathbf p\cdot\mathbf q)(\mathbf k_1\cdot\mathbf r)$ times its amplitude product. The three self-interaction permutations yield $-3K^2|A|^2A$. The six permutations of $(\mathbf k_1,\mathbf k_2,-\mathbf k_2)$ yield $-2K^2-4(\mathbf k_1\cdot\mathbf k_2)^2=-3K^2$, and likewise for the third mode. Therefore the [hexagonal convection amplitude equations](../../../fluid-mechanics.md#hexagonal-convection-amplitude-equations) are

$$
\boxed{\begin{aligned}A_T&=\mu_2KA+\gamma K\bar B\bar C-3K^2A(|A|^2+|B|^2+|C|^2),\\B_T&=\mu_2KB+\gamma K\bar C\bar A-3K^2B(|A|^2+|B|^2+|C|^2),\\C_T&=\mu_2KC+\gamma K\bar A\bar B-3K^2C(|A|^2+|B|^2+|C|^2).\end{aligned}}
$$

For a nonzero [convection roll](../../../fluid-mechanics.md#convection-roll), $B=C=0$ and $|A|^2=\mu_2/(3K)$, requiring $\mu_2>0$. Choose its phase so $A=a>0$. The radial perturbation decays, but a perturbation in the two other orientations gives

$$
\partial_T\begin{pmatrix}B\\\bar C\end{pmatrix}=\begin{pmatrix}0&\gamma Ka\\\gamma Ka&0\end{pmatrix}\begin{pmatrix}B\\\bar C\end{pmatrix}.
$$

The eigenvalues are $\pm|\gamma|Ka$. Thus

$$
\boxed{\gamma\ne0\quad\Longrightarrow\quad\text{every nonzero roll is unstable}.}
$$

This is [roll instability from broken up-down symmetry](../../../fluid-mechanics.md#roll-instability-from-broken-up-down-symmetry). A growing homogeneous amplitude perturbation already proves instability, without a sideband calculation. The source's slightly asymmetric setting means nonzero quadratic coupling. If $\gamma=0$ is allowed literally, the displayed leading equations instead have a continuous sphere of constant-total-intensity states and neutral orientation perturbations. They then establish marginality, not strict growing-mode instability; higher-order effects would decide further selection. Likewise $\alpha=0$ would invalidate the assumed finite-$k_c$ triad scaling.

## Section III

↑ **Parent:** [Paper 77](paper-77.md)

### 5

↑ **Parent:** [Section III](#section-iii)

<h4 id="5/i">i</h4>

↑ **Parent:** [5](#5)

<h5 id="5/i/solution">Solution</h5>

↑ **Parent:** [I](#5/i)

Use the same length, thermal-time, velocity and temperature scales as in thermal convection. Write the imposed [magnetic field](../../../electromagnetism.md#magnetic-field) as $B_0\hat{\mathbf z}$ and measure its perturbation in units of $B_0$. The physical linear [magnetohydrodynamic momentum equation](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-momentum-equation) contains magnetic tension $(B_0^2/\mu_0)\partial_z\mathbf b$; the gradient part of the [Lorentz force density](../../../electromagnetism.md#lorentz-force-density) is absorbed into [magnetohydrodynamic total pressure](../../../astrophysical-fluid-dynamics.md#magnetohydrodynamic-total-pressure).

Divide the momentum equation by the viscous force scale $\rho_0\nu\kappa/d^3$. Its acceleration coefficient is $\kappa/\nu=1/\sigma$ and its magnetic coefficient is

$$
\frac{B_0^2d^2}{\mu_0\rho_0\nu\kappa}=Q\zeta,\qquad \zeta=\frac\eta\kappa,\qquad Q=\frac{B_0^2d^2}{\mu_0\rho_0\eta\nu}.
$$

Here $Q$ is the [Chandrasekhar number](../../../astrophysical-fluid-dynamics.md#chandrasekhar-number), comparing magnetic and viscous-diffusive effects, and $\zeta$ is the ratio of [magnetic diffusivity](../../../astrophysical-fluid-dynamics.md#magnetic-diffusivity) to [thermal diffusivity](../../../thermodynamics.md#thermal-diffusivity). The induction scale is $B_0\kappa/d^2$, so linearization gives

$$
\boxed{\frac1\sigma\dot{\mathbf u}=-\nabla P+Q\zeta\partial_z\mathbf b+R\theta\hat{\mathbf z}+\nabla^2\mathbf u,\qquad \dot{\mathbf b}=\partial_z\mathbf u+\zeta\nabla^2\mathbf b.}
$$

Complete the linear system with $\dot\theta=w+\nabla^2\theta$, $\nabla\cdot\mathbf u=0$ and the [solenoidal magnetic-field constraint](../../../electromagnetism.md#solenoidal-magnetic-field-constraint) $\nabla\cdot\mathbf b=0$. The omitted advective and perturbed-field tension terms are quadratic in the disturbances. Magnetic tension resists bending of the vertical field, while diffusion allows that bending to relax.

<h4 id="5/ii">ii</h4>

↑ **Parent:** [5](#5)

<h5 id="5/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/ii)

Interpret perfect conductivity here as the [perfectly conducting thermal boundary condition](../../../differential-equation.md#perfectly-conducting-thermal-boundary-condition) $\theta=0$; impose the stated magnetic verticality separately. Together with the [stress-free boundary condition](../../../viscous-fluid-flow.md#stress-free-boundary-condition), admissible vertical profiles are

$$
w=W\sin\pi z,\quad\theta=\vartheta\sin\pi z,\quad\mathbf u_h=\mathbf U_h\cos\pi z,\qquad b_z=Z\cos\pi z,\quad\mathbf b_h=\mathbf B_h\sin\pi z,
$$

each multiplied by $e^{i\mathbf k\cdot\mathbf x+\lambda t}$. Solenoidality requires $i\mathbf k\cdot\mathbf U_h=-\pi W$ and $i\mathbf k\cdot\mathbf B_h=\pi Z$. The [resistive induction equation](../../../astrophysical-fluid-dynamics.md#resistive-induction-equation) preserves both profile choices. In particular $\mathbf b_h=0$ at each boundary and $\partial_zb_z=0$ there.

Set $s=k^2+\pi^2$ and $p=\pi^2$. The pressure-projected vertical momentum, thermal and vertical induction equations reduce to

$$
(\lambda/\sigma+s)W=\frac{Rk^2}{s}\vartheta-Q\zeta\pi Z,\qquad (\lambda+s)\vartheta=W,\qquad (\lambda+\zeta s)Z=\pi W.
$$

Their determinant gives the [vertical-field magnetoconvection dispersion relation](../../../astrophysical-fluid-dynamics.md#vertical-field-magnetoconvection-dispersion-relation)

$$
\boxed{(\lambda+\sigma s)(\lambda+s)(\lambda+\zeta s)+\sigma Q\zeta p(\lambda+s)-\frac{\sigma Rk^2}{s}(\lambda+\zeta s)=0.}
$$

It is best kept as a polynomial rather than canceling a factor that might vanish at a special eigenvalue. For $\lambda=0$,

$$
\boxed{R^{(e)}(k)=\frac{s^3+Qps}{k^2}.}
$$

For an oscillatory marginal mode $\lambda=i\omega$ with $\omega\ne0$, write the polynomial as $\lambda^3+a_1\lambda^2+a_2\lambda+a_3$. Its coefficients are

$$
a_1=(\sigma+1+\zeta)s,\quad a_2=(\sigma+\sigma\zeta+\zeta)s^2+\sigma Q\zeta p-\sigma Rk^2/s,\quad a_3=\sigma\zeta s^3+\sigma Q\zeta ps-\sigma R\zeta k^2.
$$

Separating real and imaginary parts gives $a_3=a_1a_2$ and $\omega^2=a_2>0$. Solving yields

$$
\boxed{R^{(o)}(k)=\frac{(\sigma+\zeta)(1+\zeta)}{\sigma}\frac{s^3}{k^2}+\frac{\zeta(\sigma+\zeta)}{1+\sigma}\frac{Qps}{k^2},\qquad \omega^2=\frac{\sigma\zeta(1-\zeta)}{1+\sigma}Qp-\zeta^2s^2.}
$$

Therefore [oscillatory marginality in vertical-field magnetoconvection](../../../astrophysical-fluid-dynamics.md#oscillatory-marginality-in-vertical-field-magnetoconvection) requires

$$
\boxed{0<\zeta<1,\qquad Q>\frac{\zeta(1+\sigma)}{\sigma(1-\zeta)}\frac{(k^2+\pi^2)^2}{\pi^2}.}
$$

The equality has zero frequency and is not an oscillatory marginal mode. For some positive horizontal [wavenumber](../../../wave-equation.md#wavenumber) to satisfy this condition, it is necessary and sufficient that $Q>\zeta(1+\sigma)\pi^2/[\sigma(1-\zeta)]$, although the associated threshold must still be minimized over admissible modes. When $\omega^2>0$, $R^{(o)}<R^{(e)}$ at the same [wavenumber](../../../wave-equation.md#wavenumber); this also follows from $R^{(e)}-R^{(o)}=(\sigma+1+\zeta)s\omega^2/(\sigma\zeta k^2)$.

<h4 id="5/iii">iii</h4>

↑ **Parent:** [5](#5)

<h5 id="5/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#5/iii)

Both neutral curves can be written with $x=k^2$ and $p=\pi^2$ as

$$
R(x)=C\frac{(x+p)^3}{x}+DQp\frac{x+p}{x}.
$$

For steady convection, $(C,D)=(1,1)$; for oscillatory convection,

$$
C_o=\frac{(\sigma+\zeta)(1+\zeta)}\sigma,\qquad D_o=\frac{\zeta(\sigma+\zeta)}{1+\sigma},\qquad \frac{D_o}{C_o}=\frac{\sigma\zeta}{(1+\sigma)(1+\zeta)}.
$$

The oscillatory result is physically relevant only with positive frequency; for fixed $0<\zeta<1$ and fixed positive $\sigma$, that holds at the minimizing [wavenumber](../../../wave-equation.md#wavenumber) for sufficiently large $Q$.

Differentiation gives the exact minimization condition

$$
\boxed{x^2(2x+3p)=p^3+\frac DCQp^2.}
$$

Its left side is strictly increasing for $x>0$, so the minimum is unique. Define $h=[Dp^2Q/(2C)]^{1/3}$. An [asymptotic expansion](../../../analysis.md#asymptotic-expansion) gives

$$
\boxed{k_*^2=h-\frac p2+\frac{p^2}{4h}+O(h^{-2}),\qquad k_*\sim\left(\frac{Dp^2}{2C}\right)^{1/6}Q^{1/6}.}
$$

Substituting back, the leading magnetic term is order $Q$, while the two balanced terms $Cx^2$ and $DQp^2/x$ sum to $3Ch^2$. Hence, through order $Q^{2/3}$,

$$
\boxed{R_{\rm min}=DpQ+3C^{1/3}\left(\frac{Dp^2Q}{2}\right)^{2/3}+O(Q^{1/3}).}
$$

In particular,

$$
\boxed{R^{(e)}_c=\pi^2Q+3\left(\frac{\pi^4Q}{2}\right)^{2/3}+O(Q^{1/3}),\qquad (k_*^{(e)})^2=\left(\frac{\pi^4Q}{2}\right)^{1/3}-\frac{\pi^2}{2}+O(Q^{-1/3}),}
$$

while the same boxed general formulas with $(C_o,D_o)$ give the oscillatory minimum and critical [wavenumber](../../../wave-equation.md#wavenumber). Thus [strong-field wavenumber selection in magnetoconvection](../../../astrophysical-fluid-dynamics.md#strong-field-wavenumber-selection-in-magnetoconvection) has $k\propto Q^{1/6}$ for both types, with different parameter-dependent constants.

For the exact steady result at arbitrary $Q\ge0$, the stationarity equation with $C=D=1$ lets us eliminate $Q$ from $R^{(e)}$. It gives

$$
R_c=\frac{2(x+p)^3}{p},\qquad Qp=R_c-3(x+p)^2.
$$

At $Q=0$, $x=p/2$ and $R_0=27p^2/4$. Consequently

$$
\boxed{Q\pi^2=R_c-R_c^{2/3}R_0^{1/3},\qquad k_c^2=\pi^2\left[\frac32\left(\frac{R_c}{R_0}\right)^{1/3}-1\right].}
$$

This [exact critical Rayleigh relation for vertical-field magnetoconvection](../../../astrophysical-fluid-dynamics.md#exact-critical-rayleigh-relation-for-vertical-field-magnetoconvection) includes the nonmagnetic minimum, with $R_c\ge R_0$ and $k_c^2\ge\pi^2/2$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2012](../../2012.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
