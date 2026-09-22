# Nonlinear analysis

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Nonlinear_analysis)

Nonlinear analysis studies equations and variational problems in which superposition fails. Its tools include nonlinear functional inequalities, conserved energies, compactness, phase-plane methods, and concentration arguments.

**Table of contents**

- [Hardy–Littlewood–Sobolev inequality](#hardy-littlewood-sobolev-inequality)
- [Generalized Korteweg–De Vries equation](#generalized-korteweg-de-vries-equation)
  - [KdV mass and energy conservation](#kdv-mass-and-energy-conservation)
  - [Global existence for the energy-subcritical generalized KdV equation](#global-existence-for-the-energy-subcritical-generalized-kdv-equation)
  - [Generalized KdV solitary wave](#generalized-kdv-solitary-wave)
    - [Orbital stability of a generalized KdV solitary wave](#orbital-stability-of-a-generalized-kdv-solitary-wave)
- [Gravitational Hartree equation](#gravitational-hartree-equation)
  - [Hartree mass and energy conservation](#hartree-mass-and-energy-conservation)
  - [Global H1 solutions of the three-dimensional gravitational Hartree equation](#global-h1-solutions-of-the-three-dimensional-gravitational-hartree-equation)
  - [Virial identity for the four-dimensional gravitational Hartree equation](#virial-identity-for-the-four-dimensional-gravitational-hartree-equation)
- [Emden-Fowler transformation](#emden-fowler-transformation)
  - [Lane-Emden equation](#lane-emden-equation)
    - [Generalized Lane-Emden equation](#generalized-lane-emden-equation)
      - [Singular homogeneous solution of the Lane-Emden equation](#singular-homogeneous-solution-of-the-lane-emden-equation)
      - [Aubin-Talenti bubble](#aubin-talenti-bubble)
- [Pohozaev identity](#pohozaev-identity)
  - [Pohozaev identity for the mass-critical NLS ground state](#pohozaev-identity-for-the-mass-critical-nls-ground-state)
- [Symmetric decreasing rearrangement](#symmetric-decreasing-rearrangement)
  - [Pólya-Szegő inequality](#polya-szego-inequality)
- [Nonlinear Schrödinger blowup analysis](#nonlinear-schrodinger-blowup-analysis)
  - [Mass-critical focusing nonlinear Schrödinger equation](#mass-critical-focusing-nonlinear-schrodinger-equation)
  - [Mass conservation for the nonlinear Schrödinger equation](#mass-conservation-for-the-nonlinear-schrodinger-equation)
  - [Energy conservation for the nonlinear Schrödinger equation](#energy-conservation-for-the-nonlinear-schrodinger-equation)
  - [Blowup alternative for the nonlinear Schrödinger equation](#blowup-alternative-for-the-nonlinear-schrodinger-equation)
  - [Virial identity](#virial-identity)
    - [Localized virial identity](#localized-virial-identity)
      - [Negative-energy blowup for the mass-critical focusing nonlinear Schrödinger equation](#negative-energy-blowup-for-the-mass-critical-focusing-nonlinear-schrodinger-equation)
  - [Radial Sobolev inequality](#radial-sobolev-inequality)
  - [NLS ground state](#nls-ground-state)
    - [Weinstein functional](#weinstein-functional)
      - [Existence of a Weinstein-functional minimizer](#existence-of-a-weinstein-functional-minimizer)
      - [Classification of Weinstein-functional minimizers](#classification-of-weinstein-functional-minimizers)
    - [Sharp Gagliardo-Nirenberg inequality](#sharp-gagliardo-nirenberg-inequality)
      - [Coercivity below the NLS ground-state mass](#coercivity-below-the-nls-ground-state-mass)
      - [Compactness of a mass-critical minimizing sequence](#compactness-of-a-mass-critical-minimizing-sequence)
  - [Profile decomposition modulo translations](#profile-decomposition-modulo-translations)
  - [Gauge transform](#gauge-transform)
  - [Trapped focusing cubic ground-state equation](#trapped-focusing-cubic-ground-state-equation)
    - [Focusing Schrödinger lens ansatz](#focusing-schrodinger-lens-ansatz)
      - [Explicit expanding focusing Schrödinger lens](#explicit-expanding-focusing-schrodinger-lens)
- [Young's inequality for products](#young-s-inequality-for-products)
- [Confining-potential energy space](#confining-potential-energy-space)
  - [Compact embedding of a confining-potential energy space](#compact-embedding-of-a-confining-potential-energy-space)
  - [Fixed-L4 minimization in the harmonic-oscillator energy space](#fixed-l4-minimization-in-the-harmonic-oscillator-energy-space)
  - [Ground-state eigenfunction of a confining Schrödinger operator](#ground-state-eigenfunction-of-a-confining-schrodinger-operator)
- [Defocusing cubic nonlinear Schrödinger equation in two dimensions](#defocusing-cubic-nonlinear-schrodinger-equation-in-two-dimensions)
  - [Harmonic-oscillator energy space](#harmonic-oscillator-energy-space)
    - [Compact embedding of the harmonic-oscillator energy space](#compact-embedding-of-the-harmonic-oscillator-energy-space)
    - [Schrödinger trapped defocusing stationary equation](#schrodinger-trapped-defocusing-stationary-equation)
  - [Schrödinger expanding lens ansatz for the mass-critical equation](#schrodinger-expanding-lens-ansatz-for-the-mass-critical-equation)
  - [Strichartz estimate for the free Schrödinger equation](#strichartz-estimate-for-the-free-schrodinger-equation)
    - [Scattering from a finite Strichartz norm](#scattering-from-a-finite-strichartz-norm)

<h2 id="hardy-littlewood-sobolev-inequality">Hardy–Littlewood–Sobolev inequality</h2>

↑ **Parent:** [Nonlinear analysis](nonlinear-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hardy–Littlewood–Sobolev_inequality)

For $0<\lambda<d$ and suitable conjugate exponents, the Hardy–Littlewood–Sobolev inequality bounds convolution with the Riesz kernel $|x|^{-\lambda}$. One useful form is

$$
\iint_{\mathbb R^d\times\mathbb R^d}
\frac{f(x)g(y)}{|x-y|^\lambda}\,dx\,dy
\lesssim\|f\|_p\|g\|_q,
\qquad
\frac1p+\frac1q+\frac\lambda d=2.
$$

<h2 id="generalized-korteweg-de-vries-equation">Generalized Korteweg–De Vries equation</h2>

↑ **Parent:** [Nonlinear analysis](nonlinear-analysis.md)

The generalized Korteweg–De Vries equation is the [nonlinear partial differential equation](partial-differential-equation.md#nonlinear-partial-differential-equation)

$$
u_t+\partial_x(u_{xx}+u^p)=0.
$$

The cases below the exponent $p=5$ are energy-subcritical in $H^1(\mathbb R)$.

### KdV mass and energy conservation

↑ **Parent:** [Generalized Korteweg–De Vries equation](#generalized-korteweg-de-vries-equation)

Sufficiently regular decaying solutions conserve

$$
M(u)=\int_{\mathbb R}u^2,
\qquad
E(u)=\frac12\int_{\mathbb R}u_x^2-
\frac1{p+1}\int_{\mathbb R}u^{p+1}.
$$

Both identities follow by [integration by parts](calculus.md#integration-by-parts) from the divergence form of the equation.

### Global existence for the energy-subcritical generalized KdV equation

↑ **Parent:** [Generalized Korteweg–De Vries equation](#generalized-korteweg-de-vries-equation)

For $p<5$, the one-dimensional [Gagliardo-Nirenberg interpolation inequality](sobolev-space.md#gagliardo-nirenberg-interpolation-inequality) gives

$$
\|u\|_{p+1}^{p+1}
\lesssim\|u_x\|_2^{(p-1)/2}\|u\|_2^{(p+3)/2}.
$$

The exponent of $\|u_x\|_2$ is below two, so the conserved mass and energy control the $H^1$ norm. The blowup alternative then extends every local $H^1$ solution globally.

### Generalized KdV solitary wave

↑ **Parent:** [Generalized Korteweg–De Vries equation](#generalized-korteweg-de-vries-equation)

If $Q''-Q+Q^p=0$, then

$$
Q_c(x)=c^{1/(p-1)}Q(\sqrt c\,x)
$$

satisfies $Q_c''-cQ_c+Q_c^p=0$, and $u(t,x)=Q_c(x-ct)$ is a traveling-wave solution of the [Generalized Korteweg–De Vries equation](#generalized-korteweg-de-vries-equation).

#### Orbital stability of a generalized KdV solitary wave

↑ **Parent:** [Generalized KdV solitary wave](#generalized-kdv-solitary-wave)

For $p<5$, a generalized KdV solitary wave is orbitally stable in $H^1(\mathbb R)$ modulo spatial translations. The variational slope has the stable sign because

$$
\|Q_c\|_2^2
=c^{(5-p)/(2(p-1))}\|Q\|_2^2
$$

is strictly increasing in $c$. Conserved mass and energy then furnish a Lyapunov functional transverse to the translation orbit.

## Gravitational Hartree equation

↑ **Parent:** [Nonlinear analysis](nonlinear-analysis.md)

This attractive mean-field equation is a gravitational version of the [Hartree equations](quantum-mechanics.md#hartree-equations). The gravitational Hartree equation couples a wave function to its attractive Newtonian potential:

$$
iu_t+\Delta u-\phi u=0,
\qquad
\Delta\phi=|u|^2,
\qquad
\phi=-\frac1{C_N|x|^{N-2}}*|u|^2.
$$

### Hartree mass and energy conservation

↑ **Parent:** [Gravitational Hartree equation](#gravitational-hartree-equation)

The gravitational Hartree flow conserves

$$
M(u)=\int|u|^2,
\qquad
E(u)=\frac12\int|\nabla u|^2-\frac14\int|\nabla\phi|^2.
$$

The self-adjointness of the Newtonian convolution turns the time derivative of the potential energy into $\operatorname{Re}\int\phi u\overline{u_t}$, which cancels the derivative of the kinetic energy by the equation.

### Global H1 solutions of the three-dimensional gravitational Hartree equation

↑ **Parent:** [Gravitational Hartree equation](#gravitational-hartree-equation)

In three dimensions, the [Hardy–Littlewood–Sobolev inequality](#hardy-littlewood-sobolev-inequality) and [Gagliardo-Nirenberg interpolation inequality](sobolev-space.md#gagliardo-nirenberg-interpolation-inequality) give

$$
\int|\nabla\phi|^2
\lesssim\|u\|_{12/5}^4
\lesssim\|u\|_2^3\|\nabla u\|_2.
$$

Conserved mass and energy therefore bound the $H^1$ norm by [Young inequality](#young-s-inequality-for-products), and the blowup alternative gives global existence.

### Virial identity for the four-dimensional gravitational Hartree equation

↑ **Parent:** [Gravitational Hartree equation](#gravitational-hartree-equation)

For a finite-variance solution in four dimensions,

$$
I(t)=\int|x|^2|u(t,x)|^2\,dx
$$

satisfies $I''(t)=16E(u)$. The identity uses the degree $-2$ homogeneity of the Newtonian kernel. Negative-energy finite-variance data consequently blow up in finite time by the convexity argument.

## Emden-Fowler transformation

↑ **Parent:** [Nonlinear analysis](nonlinear-analysis.md)

The [Emden-Fowler transformation](#emden-fowler-transformation) is a change of variables for scaling-invariant radial equations, including the [Lane-Emden equation](#lane-emden-equation). The Emden-Fowler transformation replaces a radial variable $r$ by logarithmic time $s=\log r$ and rescales the dependent variable by a power of $r$. It converts many scale-invariant radial equations into autonomous ordinary differential equations.

### Lane-Emden equation

↑ **Parent:** [Emden-Fowler transformation](#emden-fowler-transformation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lane–Emden_equation)

The classical [Lane-Emden equation](#lane-emden-equation) is the dimensionless equation

$$
u''+\frac{2}{r}u'+u^p=0
$$

for a [spherically symmetric](geometry-and-topology.md#spherical-symmetry) [polytrope](astrophysical-fluid-dynamics.md#polytrope) in three dimensions. The [Generalized Lane-Emden equation](#generalized-lane-emden-equation) extends it to arbitrary dimensions and to functions without radial symmetry.

#### Generalized Lane-Emden equation

↑ **Parent:** [Lane-Emden equation](#lane-emden-equation)

A [Generalized Lane-Emden equation](#generalized-lane-emden-equation) is a [semilinear partial differential equation](partial-differential-equation.md#semilinear-partial-differential-equation) whose highest-order term is the [Laplacian](calculus.md#laplacian):

$$
\Delta u+u^p=0.
$$

For a [radial function](partial-differential-equation.md#radial-function) in $d$ dimensions it becomes $u''+(d-1)u'/r+u^p=0$. The case $d=3$ gives the classical [Lane-Emden equation](#lane-emden-equation).

##### Singular homogeneous solution of the Lane-Emden equation

↑ **Parent:** [Generalized Lane-Emden equation](#generalized-lane-emden-equation)

When $a=2/(p-1)$ and $a<d-2$, the Lane-Emden equation has the singular scale-invariant solution

$$
u_\infty(r)=\bigl(a(d-2-a)\bigr)^{1/(p-1)}r^{-a}.
$$

##### Aubin-Talenti bubble

↑ **Parent:** [Generalized Lane-Emden equation](#generalized-lane-emden-equation)

At the energy-critical exponent $p=(d+2)/(d-2)$, the normalized Aubin-Talenti bubble

$$
W(x)=\left(1+\frac{|x|^2}{d(d-2)}\right)^{-(d-2)/2}
$$

solves $\Delta W+W^p=0$ and optimizes the critical [Sobolev embedding theorem](sobolev-space.md#sobolev-embedding-theorem).

## Pohozaev identity

↑ **Parent:** [Nonlinear analysis](nonlinear-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pohozaev_identity)

A Pohozaev identity is an integral identity for a nonlinear partial differential equation, obtained by multiplying the equation by a scaling vector field such as $x\mathbin{\cdot}\nabla u$ and applying [integration by parts](calculus.md#integration-by-parts). It relates kinetic, potential, and nonlinear energies.

### Pohozaev identity for the mass-critical NLS ground state

↑ **Parent:** [Pohozaev identity](#pohozaev-identity)

Testing the ground-state equation against $Q$ and applying the [Pohozaev identity](#pohozaev-identity) gives

$$
\|\nabla Q\|_2^2=\frac d2\|Q\|_2^2,
\qquad
\|Q\|_{2+4/d}^{2+4/d}=\frac{d+2}{d}\|\nabla Q\|_2^2.
$$

Consequently $E(Q)=0$ and $\inf J=\frac{d}{d+2}\|Q\|_2^{4/d}$.

## Symmetric decreasing rearrangement

↑ **Parent:** [Nonlinear analysis](nonlinear-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_decreasing_rearrangement)

The symmetric decreasing rearrangement $u^*$ of a measurable function is the radial, radially nonincreasing function whose superlevel sets are centered balls with the same measures as those of $|u|$. It preserves $L^p$ norms, and the [Pólya-Szegő inequality](#polya-szego-inequality) gives $\|\nabla u^*\|_2\leq\|\nabla u\|_2$.

<h3 id="polya-szego-inequality">Pólya-Szegő inequality</h3>

↑ **Parent:** [Symmetric decreasing rearrangement](#symmetric-decreasing-rearrangement)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pólya-Szegő_inequality)

For $u\in W^{1,p}(\mathbb R^d)$, the [symmetric decreasing rearrangement](#symmetric-decreasing-rearrangement) satisfies

$$
\|\nabla u^*\|_{L^p}\leq\|\nabla u\|_{L^p}.
$$

<h2 id="nonlinear-schrodinger-blowup-analysis">Nonlinear Schrödinger blowup analysis</h2>

↑ **Parent:** [Nonlinear analysis](nonlinear-analysis.md)

Nonlinear Schrödinger blowup analysis studies whether a solution of the [Focusing nonlinear Schrodinger equation](integrable-systems.md#focusing-nonlinear-schrodinger-equation) remains bounded in its natural Sobolev space or develops an unbounded gradient norm in finite time.

<h3 id="mass-critical-focusing-nonlinear-schrodinger-equation">Mass-critical focusing nonlinear Schrödinger equation</h3>

↑ **Parent:** [Nonlinear Schrödinger blowup analysis](#nonlinear-schrodinger-blowup-analysis)

The mass-critical focusing nonlinear Schrödinger equation on $\mathbb R^d$ is

$$
i\partial_tu+\Delta u+|u|^{4/d}u=0.
$$

Its scaling $u(t,x)\mapsto\lambda^{d/2}u(\lambda^2t,\lambda x)$ preserves the [Lebesgue space](measure-theory.md#lp-space) norm $\|u\|_{L^2}$, which is the [conserved mass](#mass-conservation-for-the-nonlinear-schrodinger-equation).

<h3 id="mass-conservation-for-the-nonlinear-schrodinger-equation">Mass conservation for the nonlinear Schrödinger equation</h3>

↑ **Parent:** [Nonlinear Schrödinger blowup analysis](#nonlinear-schrodinger-blowup-analysis)

For sufficiently regular solutions of a gauge-invariant nonlinear Schrödinger equation,

$$
M(u(t))=\int_{\mathbb R^d}|u(t,x)|^2\,dx
$$

is independent of time.

<h3 id="energy-conservation-for-the-nonlinear-schrodinger-equation">Energy conservation for the nonlinear Schrödinger equation</h3>

↑ **Parent:** [Nonlinear Schrödinger blowup analysis](#nonlinear-schrodinger-blowup-analysis)

For the focusing power equation $iu_t+\Delta u+|u|^{p-1}u=0$, the conserved energy is

$$
E(u)=\frac12\int|\nabla u|^2-
\frac1{p+1}\int|u|^{p+1}.
$$

<h3 id="blowup-alternative-for-the-nonlinear-schrodinger-equation">Blowup alternative for the nonlinear Schrödinger equation</h3>

↑ **Parent:** [Nonlinear Schrödinger blowup analysis](#nonlinear-schrodinger-blowup-analysis)

An $H^1$ solution of the nonlinear Schrödinger equation either exists globally forward in time or its $H^1$ norm, equivalently its gradient norm when mass is conserved, becomes unbounded at the finite endpoint of its maximal lifespan.

### Virial identity

↑ **Parent:** [Nonlinear Schrödinger blowup analysis](#nonlinear-schrodinger-blowup-analysis)

A virial identity describes the time derivatives of a spatial moment of a solution to a dispersive equation. For the mass-critical nonlinear Schrödinger equation, the second derivative of the variance is a constant multiple of the conserved energy.

#### Localized virial identity

↑ **Parent:** [Virial identity](#virial-identity)

A localized virial identity differentiates a weighted mass $\int\chi|u|^2$ and its associated momentum. Compactly supported or flattened weights retain the coercive interior contribution while replacing an infinite-variance assumption by controllable tail errors.

<h5 id="negative-energy-blowup-for-the-mass-critical-focusing-nonlinear-schrodinger-equation">Negative-energy blowup for the mass-critical focusing nonlinear Schrödinger equation</h5>

↑ **Parent:** [Localized virial identity](#localized-virial-identity)

For a finite-variance solution of the [mass-critical focusing nonlinear Schrödinger equation](#mass-critical-focusing-nonlinear-schrodinger-equation), the [virial identity](#virial-identity) gives

$$
\frac{d^2}{dt^2}\int_{\mathbb R^d}|x|^2|u(t,x)|^2\,dx=16E(u_0).
$$

If $E(u_0)<0$, the right-hand side is a negative constant. The nonnegative variance would then become negative in finite time if the solution remained regular, so the solution blows up in finite time.

### Radial Sobolev inequality

↑ **Parent:** [Nonlinear Schrödinger blowup analysis](#nonlinear-schrodinger-blowup-analysis)

For a radial function $u\in H^1(\mathbb R^d)$,

$$
|u(r)|^2\lesssim_d r^{-(d-1)}\|u\|_2\|\nabla u\|_2.
$$

This supplies spatial decay without requiring a weighted moment.

### NLS ground state

↑ **Parent:** [Nonlinear Schrödinger blowup analysis](#nonlinear-schrodinger-blowup-analysis)

For the [mass-critical focusing nonlinear Schrödinger equation](#mass-critical-focusing-nonlinear-schrodinger-equation) in dimension $d$, the NLS ground state is the positive radial solution of

$$
-\Delta Q+Q-Q^{1+4/d}=0.
$$

Its symmetry orbit consists of the optimizers of the sharp Gagliardo-Nirenberg inequality.

#### Weinstein functional

↑ **Parent:** [NLS ground state](#nls-ground-state)

For $p=2+4/d$, the mass-critical Weinstein functional is

$$
J(u)=\frac{\|\nabla u\|_2^2\|u\|_2^{4/d}}{\|u\|_p^p}.
$$

It is invariant under multiplication by a nonzero scalar, spatial dilation, translation, and constant phase. Its positive minimizers are rescalings and translations of the [NLS ground state](#nls-ground-state).

##### Existence of a Weinstein-functional minimizer

↑ **Parent:** [Weinstein functional](#weinstein-functional)

Normalize a minimizing sequence so that its $L^2$ norm and gradient norm are fixed. [Symmetric decreasing rearrangement](#symmetric-decreasing-rearrangement) does not increase the gradient norm and preserves every $L^p$ norm, while radial compactness prevents translation loss. A weakly convergent subsequence therefore converges strongly in the nonlinear $L^{2+4/d}$ norm and yields a nonnegative minimizer.

##### Classification of Weinstein-functional minimizers

↑ **Parent:** [Weinstein functional](#weinstein-functional)

Every minimizer of the [Weinstein functional](#weinstein-functional) has the form

$$
u(x)=aQ(b(x-x_0)),
\qquad
a\in\mathbb C\setminus\{0\},\quad b>0,\quad x_0\in\mathbb R^d,
$$

where $Q$ is the positive radial [NLS ground state](#nls-ground-state). The [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) first reduces a minimizer to a rescaled ground-state equation; the equality cases in the diamagnetic and rearrangement inequalities give the constant phase, translation, and radial profile.

#### Sharp Gagliardo-Nirenberg inequality

↑ **Parent:** [NLS ground state](#nls-ground-state)

In dimension $d$, the mass-critical sharp inequality is

$$
\|u\|_{2+4/d}^{2+4/d}
\leq\frac{d+2}{d\|Q\|_2^{4/d}}
\|u\|_2^{4/d}\|\nabla u\|_2^2,
$$

and equality holds exactly on the phase, translation, and scaling orbit of the [NLS ground state](#nls-ground-state) $Q$. For $d=2$ this becomes $\|u\|_4^4\leq2\|Q\|_2^{-2}\|u\|_2^2\|\nabla u\|_2^2$.

##### Coercivity below the NLS ground-state mass

↑ **Parent:** [Sharp Gagliardo-Nirenberg inequality](#sharp-gagliardo-nirenberg-inequality)

The sharp inequality implies

$$
E(u)\geq\frac12\|\nabla u\|_2^2
\left[1-\left(\frac{\|u\|_2}{\|Q\|_2}\right)^{4/d}\right].
$$

Thus energy controls the gradient whenever the mass is strictly below the mass of the [NLS ground state](#nls-ground-state).

##### Compactness of a mass-critical minimizing sequence

↑ **Parent:** [Sharp Gagliardo-Nirenberg inequality](#sharp-gagliardo-nirenberg-inequality)

Suppose $\|u_n\|_2=\|Q\|_2$, $\|\nabla u_n\|_2=\|\nabla Q\|_2$, and $E(u_n)\to0$. The [profile decomposition modulo translations](#profile-decomposition-modulo-translations) and the sharp inequality force exactly one nonzero profile: splitting the mass would make the sharp inequality strict. Hence some translations $u_n(\cdot+x_n)$ converge strongly in $H^1$, and therefore in $L^{2+4/d}$, to an optimizer.

### Profile decomposition modulo translations

↑ **Parent:** [Nonlinear Schrödinger blowup analysis](#nonlinear-schrodinger-blowup-analysis)

Every bounded sequence $(u_n)$ in $H^1(\mathbb R^d)$ has, after passage to a subsequence, a decomposition

$$
u_n=\sum_{j=1}^J\phi^j(\,\cdot-x_n^j)+r_n^J,
$$

where $|x_n^j-x_n^k|\to\infty$ for $j\ne k$, the $L^2$ and gradient norms decouple asymptotically, and

$$
\lim_{J\to\infty}\limsup_{n\to\infty}
\|r_n^J\|_{L^p}=0
$$

for every $2<p<2^*$.

### Gauge transform

↑ **Parent:** [Nonlinear Schrödinger blowup analysis](#nonlinear-schrodinger-blowup-analysis)

This local phase change is a [gauge transformation](electromagnetism.md#gauge-transformation) of the wave function. Multiplication by $e^{ia\psi(x)}$ is a gauge transform that preserves pointwise modulus and mass while shifting the gradient by $ia(\nabla\psi)u$.

### Trapped focusing cubic ground-state equation

↑ **Parent:** [Nonlinear Schrödinger blowup analysis](#nonlinear-schrodinger-blowup-analysis)

The trapped focusing cubic ground-state equation in two dimensions is

$$
\Delta P_\eta-P_\eta-\frac\eta4|x|^2P_\eta+P_\eta^3=0.
$$

A nonzero positive solution follows from minimizing the harmonic-oscillator quadratic form subject to a fixed $L^4$ norm and then rescaling by the positive Lagrange multiplier.

<h4 id="focusing-schrodinger-lens-ansatz">Focusing Schrödinger lens ansatz</h4>

↑ **Parent:** [Trapped focusing cubic ground-state equation](#trapped-focusing-cubic-ground-state-equation)

If $P_\eta$ solves the [trapped focusing cubic ground-state equation](#trapped-focusing-cubic-ground-state-equation), the ansatz

$$
u(t,x)=\lambda(t)^{-1}P_\eta(x/\lambda(t))
\exp\left(-\frac{i}{4}b(t)|x/\lambda(t)|^2+i\gamma(t)\right)
$$

solves the two-dimensional [mass-critical focusing nonlinear Schrödinger equation](#mass-critical-focusing-nonlinear-schrodinger-equation) when

$$
b=-\lambda\lambda_t,
\qquad
\lambda^2b_t+b^2=-\eta,
\qquad
\gamma_t=\lambda^{-2}.
$$

<h5 id="explicit-expanding-focusing-schrodinger-lens">Explicit expanding focusing Schrödinger lens</h5>

↑ **Parent:** [Focusing Schrödinger lens ansatz](#focusing-schrodinger-lens-ansatz)

The initial conditions $\lambda(-1)=\sqrt{1+\eta}$ and $b(-1)=1$ select

$$
\lambda(t)=\sqrt{t^2+\eta},
\qquad b(t)=-t,
\qquad
\gamma(t)-\gamma(-1)=\int_{-1}^t\frac{d\tau}{\tau^2+\eta}.
$$

The scale grows linearly at infinity, yielding a finite critical spacetime norm for the corresponding lens solution.

<h2 id="young-s-inequality-for-products">Young's inequality for products</h2>

↑ **Parent:** [Nonlinear analysis](nonlinear-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Young's_inequality_for_products)

Young's inequality for products states that for conjugate exponents $q,q'>1$ and nonnegative $a,b$,

$$
ab\leq\frac{a^q}{q}+\frac{b^{q'}}{q'}.
$$

Its weighted form absorbs a lower power into a coercive higher power at the cost of a constant.

## Confining-potential energy space

↑ **Parent:** [Nonlinear analysis](nonlinear-analysis.md)

For a nonnegative potential $V(x)\to\infty$ as $|x|\to\infty$, the confining-potential energy space is

$$
\Sigma_V=\{u:\nabla u\in L^2,\ V^{1/2}u\in L^2\},
\qquad
\|u\|_{\Sigma_V}^2=\|\nabla u\|_2^2+\|V^{1/2}u\|_2^2.
$$

A local [Poincaré inequality](sobolev-space.md#poincare-inequality) controls the missing $L^2$ term, so this energy norm makes $\Sigma_V$ a [Hilbert space](hilbert-space.md).

### Compact embedding of a confining-potential energy space

↑ **Parent:** [Confining-potential energy space](#confining-potential-energy-space)

The embedding $\Sigma_V\hookrightarrow L^2(\mathbb R^d)$ is compact. The [Rellich-Kondrachov compactness theorem](sobolev-space.md#rellich-kondrachov-theorem) gives compactness on each fixed ball, while

$$
\int_{|x|>R}|u|^2
\leq\left(\inf_{|x|>R}V(x)\right)^{-1}
\int_{\mathbb R^d}V|u|^2
$$

makes the tails uniformly small.

### Fixed-L4 minimization in the harmonic-oscillator energy space

↑ **Parent:** [Confining-potential energy space](#confining-potential-energy-space)

In two dimensions, the quadratic functional

$$
\int|\nabla u|^2+\int|u|^2+\frac\eta4\int|x|^2|u|^2
$$

attains its minimum subject to $\|u\|_4^4=M>0$. A bounded minimizing sequence is weakly compact in the harmonic-oscillator energy space and strongly compact in $L^4$: local [Rellich-Kondrachov compactness theorem](sobolev-space.md#rellich-kondrachov-theorem) and the weighted tail bound prevent escape to infinity.

<h3 id="ground-state-eigenfunction-of-a-confining-schrodinger-operator">Ground-state eigenfunction of a confining Schrödinger operator</h3>

↑ **Parent:** [Confining-potential energy space](#confining-potential-energy-space)

The minimum of

$$
\|\nabla u\|_2^2+\|V^{1/2}u\|_2^2
$$

subject to $\|u\|_2=1$ is attained because $\Sigma_V$ embeds compactly into $L^2$. Replacing a minimizer by its [absolute value](real-analysis.md#absolute-value) does not increase its energy. The [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) therefore produces a nonnegative eigenfunction of $-\Delta+V$ for its lowest eigenvalue.

<h2 id="defocusing-cubic-nonlinear-schrodinger-equation-in-two-dimensions">Defocusing cubic nonlinear Schrödinger equation in two dimensions</h2>

↑ **Parent:** [Nonlinear analysis](nonlinear-analysis.md)

The two-dimensional defocusing cubic nonlinear Schrödinger equation is mass-critical: the scaling $u(t,x)\mapsto\lambda^{-1}u(t/\lambda^2,x/\lambda)$ preserves the $L^2$ norm. The defocusing sign makes its nonlinear energy positive.

### Harmonic-oscillator energy space

↑ **Parent:** [Defocusing cubic nonlinear Schrödinger equation in two dimensions](#defocusing-cubic-nonlinear-schrodinger-equation-in-two-dimensions)

The harmonic-oscillator energy space is

$$
\Sigma=\{v\in H^1(\mathbb R^d):|x|v\in L^2(\mathbb R^d)\},
\qquad
\|v\|_\Sigma^2=\|\nabla v\|_2^2+\||x|v\|_2^2.
$$

The spatial moment prevents mass from escaping to infinity.

#### Compact embedding of the harmonic-oscillator energy space

↑ **Parent:** [Harmonic-oscillator energy space](#harmonic-oscillator-energy-space)

The embedding $\Sigma\hookrightarrow L^2(\mathbb R^d)$ is compact. Rellich compactness controls a fixed ball, while

$$
\int_{|x|>R}|v|^2\leq R^{-2}\||x|v\|_2^2
$$

controls the tail uniformly.

<h4 id="schrodinger-trapped-defocusing-stationary-equation">Schrödinger trapped defocusing stationary equation</h4>

↑ **Parent:** [Harmonic-oscillator energy space](#harmonic-oscillator-energy-space)

Critical points of the trapped defocusing cubic energy

$$
J(v)=\frac12\|v\|_\Sigma^2-\frac\omega2\|v\|_2^2+\frac14\|v\|_4^4
$$

satisfy $-\Delta v+|x|^2v-\omega v+v^3=0$.

<h3 id="schrodinger-expanding-lens-ansatz-for-the-mass-critical-equation">Schrödinger expanding lens ansatz for the mass-critical equation</h3>

↑ **Parent:** [Defocusing cubic nonlinear Schrödinger equation in two dimensions](#defocusing-cubic-nonlinear-schrodinger-equation-in-two-dimensions)

If $v$ solves the trapped stationary equation, the rescaled quadratic-phase ansatz

$$
u(t,x)=\lambda(t)^{-1}v(x/\lambda(t))
\exp\!\left(-\frac{i}{4}b(t)|x/\lambda(t)|^2+i\gamma(t)\right)
$$

solves the free mass-critical equation when the scaling, chirp, and phase parameters satisfy the associated lens-transform system.

<h3 id="strichartz-estimate-for-the-free-schrodinger-equation">Strichartz estimate for the free Schrödinger equation</h3>

↑ **Parent:** [Defocusing cubic nonlinear Schrödinger equation in two dimensions](#defocusing-cubic-nonlinear-schrodinger-equation-in-two-dimensions)

In two dimensions, the endpoint spacetime estimate and its dual include

$$
\|e^{it\Delta}f\|_{L^4_{t,x}}\lesssim\|f\|_2,
\qquad
\left\|\int e^{-is\Delta}F(s)\,ds\right\|_2
\lesssim\|F\|_{L^{4/3}_{t,x}}.
$$

#### Scattering from a finite Strichartz norm

↑ **Parent:** [Strichartz estimate for the free Schrödinger equation](#strichartz-estimate-for-the-free-schrodinger-equation)

If a global cubic Schrödinger solution has finite $L^4_{t,x}$ norm on a time ray, the dual Strichartz estimate makes its interaction representation Cauchy in $L^2$. It therefore converges to scattering data $u_\infty$, and $u(t)-e^{it\Delta}u_\infty\to0$ in $L^2$.

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)
