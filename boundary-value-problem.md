# Boundary value problem

↑ **Parent:** [Ordinary differential equation](differential-equation.md#ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Boundary_value_problem)

A boundary value problem asks for a differential-equation solution satisfying conditions at more than one point or boundary component.

**Table of contents**

- [Neumann boundary-value problem](#neumann-boundary-value-problem)
  - [Uniqueness of the Neumann problem](#uniqueness-of-the-neumann-problem)
- [Boundary trace of a function](#boundary-trace-of-a-function)
- [Oblique derivative boundary condition](#oblique-derivative-boundary-condition)
  - [Corner compatibility for collinear oblique derivative data](#corner-compatibility-for-collinear-oblique-derivative-data)
  - [Rational-angle oblique derivative problem on a quadrant](#rational-angle-oblique-derivative-problem-on-a-quadrant)
    - [Quarter-plane oblique boundary spectral functions](#quarter-plane-oblique-boundary-spectral-functions)
      - [Single-function spectral elimination for a rational-angle quadrant](#single-function-spectral-elimination-for-a-rational-angle-quadrant)
    - [Homogeneous corner ambiguity in a quadrant Laplace problem](#homogeneous-corner-ambiguity-in-a-quadrant-laplace-problem)
- [Dirichlet-to-Neumann map](#dirichlet-to-neumann-map)
  - [Semistrip Dirichlet-to-Neumann sine transforms](#semistrip-dirichlet-to-neumann-sine-transforms)
- [Riemann-Hilbert problem](#riemann-hilbert-problem)
  - [Sectorial half-line mKdV Riemann-Hilbert reconstruction](#sectorial-half-line-mkdv-riemann-hilbert-reconstruction)
  - [Half-line NLS Riemann-Hilbert reconstruction](#half-line-nls-riemann-hilbert-reconstruction)
  - [Negative-index scalar Riemann-Hilbert moment conditions](#negative-index-scalar-riemann-hilbert-moment-conditions)
  - [Matrix NLS reconstruction from a normalized Riemann-Hilbert problem](#matrix-nls-reconstruction-from-a-normalized-riemann-hilbert-problem)
  - [Canonical factorization of a rational scalar Riemann-Hilbert jump](#canonical-factorization-of-a-rational-scalar-riemann-hilbert-jump)
- [Wiener-Hopf method](#wiener-hopf-method)
  - [Mixed Dirichlet-Neumann half-plane diffraction](#mixed-dirichlet-neumann-half-plane-diffraction)
  - [Wiener-Hopf factorization](#wiener-hopf-factorization)
  - [Wiener-Hopf equation](#wiener-hopf-equation)
    - [Wiener-Hopf kernel](#wiener-hopf-kernel)
    - [Pole subtraction in a Wiener-Hopf equation](#pole-subtraction-in-a-wiener-hopf-equation)
- [Fokas method](#fokas-method)
  - [Two-trace half-line cubic dispersion representation](#two-trace-half-line-cubic-dispersion-representation)
  - [Boundary spectral representation of a holomorphic function on a semistrip](#boundary-spectral-representation-of-a-holomorphic-function-on-a-semistrip)
  - [Quadrant modified Helmholtz spectral reconstruction](#quadrant-modified-helmholtz-spectral-reconstruction)
  - [Neumann spectral formula for half-line constant drift](#neumann-spectral-formula-for-half-line-constant-drift)
  - [Dirichlet spectral formula for half-line constant drift](#dirichlet-spectral-formula-for-half-line-constant-drift)
  - [Local relation](#local-relation)
  - [Dispersion symmetry elimination of a boundary trace](#dispersion-symmetry-elimination-of-a-boundary-trace)
    - [Cubic-dispersion elimination of one missing boundary trace](#cubic-dispersion-elimination-of-one-missing-boundary-trace)
    - [Cubic Stokes dispersion symmetry](#cubic-stokes-dispersion-symmetry)
  - [Upper-quadrant cancellation of reflected boundary transforms](#upper-quadrant-cancellation-of-reflected-boundary-transforms)
- [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)
  - [Dirichlet spectral formula for Airy flow with negative transport](#dirichlet-spectral-formula-for-airy-flow-with-negative-transport)
  - [Finite-interval Airy global relation](#finite-interval-airy-global-relation)
    - [Finite-interval Airy spectral determinant](#finite-interval-airy-spectral-determinant)
  - [Semistrip Laplace spectral global relation](#semistrip-laplace-spectral-global-relation)
  - [Drift-diffusion half-line global relation](#drift-diffusion-half-line-global-relation)
  - [Half-line linear dispersive Stokes global relation](#half-line-linear-dispersive-stokes-global-relation)
    - [Dirichlet spectral representation for the linear dispersive Stokes equation](#dirichlet-spectral-representation-for-the-linear-dispersive-stokes-equation)
  - [Half-line Schrodinger boundary-trace elimination](#half-line-schrodinger-boundary-trace-elimination)
  - [Finite-time spectral boundary transform](#finite-time-spectral-boundary-transform)
    - [Finite-horizon extension of a boundary transform](#finite-horizon-extension-of-a-boundary-transform)
  - [Polygonal modified Helmholtz global relation](#polygonal-modified-helmholtz-global-relation)
    - [Dirichlet reconstruction in an equilateral triangle](#dirichlet-reconstruction-in-an-equilateral-triangle)
  - [Half-line drift global relation](#half-line-drift-global-relation)
    - [Exponential-decay contour for half-line drift diffusion](#exponential-decay-contour-for-half-line-drift-diffusion)
  - [Collocation points for a global relation](#collocation-points-for-a-global-relation)
  - [Conjugate global relations for the modified Helmholtz equation](#conjugate-global-relations-for-the-modified-helmholtz-equation)
    - [Rotationally invariant Neumann reconstruction in an equilateral triangle](#rotationally-invariant-neumann-reconstruction-in-an-equilateral-triangle)
    - [Sine collocation of square modified Helmholtz global relations](#sine-collocation-of-square-modified-helmholtz-global-relations)
      - [Square modified Helmholtz Dirichlet-to-Neumann coefficients](#square-modified-helmholtz-dirichlet-to-neumann-coefficients)
      - [Diagonal dominance of paired square global-relation collocation](#diagonal-dominance-of-paired-square-global-relation-collocation)
- [Spectral parameter for a linear boundary value problem](#spectral-parameter-for-a-linear-boundary-value-problem)
- [Boundary lifting](#boundary-lifting)
  - [Uniform half-line Schrodinger representation by boundary lifting](#uniform-half-line-schrodinger-representation-by-boundary-lifting)

## Neumann boundary-value problem

↑ **Parent:** [Boundary value problem](boundary-value-problem.md)

A [boundary value problem](boundary-value-problem.md) with prescribed outward [normal derivative](differential-geometry.md#normal-derivative), or the associated weighted flux, on the boundary. Its boundary data are [Neumann boundary data](differential-equation.md#neumann-boundary-data). For an elliptic divergence-form operator without a zeroth-order term, integration over the domain imposes a compatibility condition between total source and boundary flux. A connected domain generally leaves a constant undetermined, fixed by a mean or reference value.

### Uniqueness of the Neumann problem

↑ **Parent:** [Neumann boundary-value problem](#neumann-boundary-value-problem)

On a connected bounded domain, two harmonic potentials with the same normal [derivative](calculus.md#derivative) differ by a constant. Their difference $u$ has $\nabla^2u=0$ and $\partial_nu=0$. [Green's first identity](partial-differential-equation.md#green-s-first-identity) gives $\int|\nabla u|^2dV=\int_{\partial\Omega}u\partial_nu\,dA=0$, so the [gradient](multivariable-calculus.md#gradient) vanishes. In a multiply connected magnetic core, also fix the [circulation](vorticity.md#circulation-physics) around each independent hole: a curl-free [magnetic field intensity](electromagnetism.md#magnetic-field-intensity) with nonzero [circulation](vorticity.md#circulation-physics) need not be the [gradient](multivariable-calculus.md#gradient) of a single-valued scalar potential. After those [circulations](vorticity.md#circulation-physics) have been matched, apply the scalar-potential uniqueness argument to the difference field.

## Boundary trace of a function

↑ **Parent:** [Boundary value problem](boundary-value-problem.md)

For a sufficiently regular [function](function.md) on a domain $\Omega$, its boundary trace is the restriction to $\partial\Omega$, using the limit from within the domain when necessary. In a half-line evolution problem, the traces $f_j(t)=\partial_x^ju(0,t)$ are boundary values of the spatial [derivatives](calculus.md#derivative). An initial value does not generally determine every such trace without the [partial differential equation](partial-differential-equation.md) and suitable [boundary conditions](differential-equation.md#boundary-condition). The [Sobolev trace operator](sobolev-space.md#trace-operator) extends classical restriction continuously to appropriate [Sobolev spaces](sobolev-space.md), where pointwise values need not be defined.

## Oblique derivative boundary condition

↑ **Parent:** [Boundary value problem](boundary-value-problem.md)

An oblique derivative boundary condition prescribes a linear combination of the outward [normal derivative](differential-geometry.md#normal-derivative) and the tangential [derivative](calculus.md#derivative) on a boundary. Its strictly oblique case has a nonzero normal coefficient; a zero normal coefficient is a limiting tangential condition. Both trace directions must be tracked when constructing a [global relation](#global-relation-for-a-linear-boundary-value-problem). On unbounded domains, regularity at corners and a growth condition at infinity are separate parts of an admissible [boundary value problem](boundary-value-problem.md).

### Corner compatibility for collinear oblique derivative data

↑ **Parent:** [Oblique derivative boundary condition](#oblique-derivative-boundary-condition)

For a solution with a continuous [gradient](multivariable-calculus.md#gradient) at a quadrant corner, the prescribed derivative directions are $( -\sin\beta_1,\cos\beta_1)$ and $(\cos\beta_2,-\sin\beta_2)$. When $\beta_1+\beta_2=\pi/2$, these vectors are negatives of one another. Their corner data must therefore be opposite. Imposing $h_1(0)=h_2(0)$ as well forces both to vanish. Smooth decay of separate boundary functions alone does not ensure this local [compatibility condition for an overdetermined linear system](integrable-systems.md#compatibility-condition-for-an-overdetermined-linear-system).

// Target: analysis.bigb

### Rational-angle oblique derivative problem on a quadrant

↑ **Parent:** [Oblique derivative boundary condition](#oblique-derivative-boundary-condition)

For a complex-valued [harmonic function](partial-differential-equation.md#harmonic-function) in the first quadrant, write $\Phi=q_z$ and $\Psi(\bar z)=q_{\bar z}$ as independent [holomorphic functions](holomorphic-function.md). Prescribe $i(e^{i\beta_1}\Phi-e^{-i\beta_1}\Psi)=g_1$ on the imaginary axis and $e^{-i\beta_2}\Phi+e^{i\beta_2}\Psi=g_2$ on the real axis. If $\beta_1+\beta_2=n\pi/2$, set $\epsilon=(-1)^n$. Reflection into four quadrants produces a scalar [Riemann-Hilbert problem](#riemann-hilbert-problem) with parity $H(-z)=-\epsilon H(z)$ and known jumps. Provided its corner and large-arc contributions vanish, the [Cauchy integral formula](analysis.md#cauchy-integral-formula) gives

$$
\Phi(z)=\frac1{2\pi i}\left[e^{i\beta_2}\int_0^\infty g_2(s)\left(\frac1{s-z}-\frac\epsilon{s+z}\right)ds-e^{-i\beta_1}\int_0^\infty g_1(s)\left(\frac1{is-z}-\frac\epsilon{is+z}\right)ds\right].
$$

Complex boundary data do not justify replacing $q_{\bar z}$ by the conjugate of $q_z$.

#### Quarter-plane oblique boundary spectral functions

↑ **Parent:** [Rational-angle oblique derivative problem on a quadrant](#rational-angle-oblique-derivative-problem-on-a-quadrant)

For real [harmonic](partial-differential-equation.md#harmonic-function) $q$, prescribe $-\sin\beta_1q_x+\cos\beta_1q_y=h_1$ on the vertical axis and $\cos\beta_2q_x-\sin\beta_2q_y=h_2$ on the horizontal axis. Their orthogonal derivatives $j_1,j_2$ determine the missing gradient components. If $H_1,J_1$ use the kernel $e^{ky}$ and $H_2,J_2$ use $e^{-ikx}$, the clockwise spectra $\widehat q_1=\int_0^{i\infty}e^{-ikz}q_z\,dz$, $\widehat q_2=-\int_0^\infty e^{-ikz}q_z\,dz$ have the displayed expressions. Their [global relation](#global-relation-for-a-linear-boundary-value-problem) is $\widehat q_1+\widehat q_2=0$ in the third spectral quadrant.

// Target: analysis.bigb

##### Single-function spectral elimination for a rational-angle quadrant

↑ **Parent:** [Quarter-plane oblique boundary spectral functions](#quarter-plane-oblique-boundary-spectral-functions)

Reality of the boundary derivatives gives $H_1(\bar k)=\overline{H_1(k)}$ and $H_2(-\bar k)=\overline{H_2(k)}$, and the same identities for $J_1,J_2$. The [global relation](#global-relation-for-a-linear-boundary-value-problem) and its conjugate express both [quarter-plane oblique boundary spectral functions](#quarter-plane-oblique-boundary-spectral-functions) in terms of the known $H_1,H_2$ and the single bounded [holomorphic function](holomorphic-function.md) $\Phi$ in the upper half-plane. For $\gamma=\beta_1+\beta_2\in\{0,\pi/2,\pi\}$, its coefficients on the positive real and positive imaginary reconstruction rays are opposite, because $e^{4i\gamma}=1$. Closing the first-quadrant contour removes $\Phi$ by the [Cauchy integral theorem](complex-analysis.md#cauchy-s-integral-theorem).

// Target: analysis.bigb

#### Homogeneous corner ambiguity in a quadrant Laplace problem

↑ **Parent:** [Rational-angle oblique derivative problem on a quadrant](#rational-angle-oblique-derivative-problem-on-a-quadrant)

For tangential data with $\beta_1=\beta_2=0$, the [harmonic function](partial-differential-equation.md#harmonic-function) $q=xy$ has zero prescribed data on both axes but a growing nonzero derivative. For normal data with $\beta_1=\beta_2=\pi/2$, $q=\log|z|$ also has zero prescribed data, and $q_z=1/(2z)$ decays at infinity but is singular at the corner. Thus decay of the data, and even decay of the solution gradient, does not alone determine the quadrant representation. Requiring the reflected gradient to decay at infinity and satisfy $|z|H(z)\to0$ at the corner removes both examples. Without such conditions, add homogeneous [holomorphic](holomorphic-function.md) terms obeying the reflection parity.

## Dirichlet-to-Neumann map

↑ **Parent:** [Boundary value problem](boundary-value-problem.md)

Given a uniquely solvable [Dirichlet problem](analysis.md#dirichlet-problem), this map sends prescribed [Dirichlet boundary data](differential-equation.md#dirichlet-boundary-data) to the solution's outward [normal derivative](differential-geometry.md#normal-derivative). It depends on the differential operator and domain. Spectral [global relations](#global-relation-for-a-linear-boundary-value-problem) offer one way to compute it numerically from boundary traces, while a finite collocation scheme still requires a rank and conditioning check.

### Semistrip Dirichlet-to-Neumann sine transforms

↑ **Parent:** [Dirichlet-to-Neumann map](#dirichlet-to-neumann-map)

In the [semistrip Laplace spectral global relation](#semistrip-laplace-spectral-global-relation), reality makes $W(\pm\kappa)$ real for $\kappa>0$. Its imaginary parts at those two arguments remove the unknown vertical-side [normal derivative](differential-geometry.md#normal-derivative). With $G_j^s(\kappa)=\int_0^\infty\sin(\kappa x)g_j(x)\,dx$ and $S_j(\kappa)=\int_0^\infty\sin(\kappa x)q_y(x,j)\,dx$, the result is

$$
S_0=\frac{\kappa[-\cosh(\kappa l)G_0^s+G_l^s+\int_0^l\sinh(\kappa(l-y))h(y)\,dy]}{\sinh(\kappa l)},\qquad
S_l=\frac{\kappa[-G_0^s+\cosh(\kappa l)G_l^s-\int_0^l\sinh(\kappa y)h(y)\,dy]}{\sinh(\kappa l)}.
$$

The lower outward [normal derivative](differential-geometry.md#normal-derivative) is $-q_y$, so its [Dirichlet-to-Neumann map](#dirichlet-to-neumann-map) coefficient is $-S_0$, whereas the upper coefficient is $S_l$.

// Target: analysis.bigb

## Riemann-Hilbert problem

↑ **Parent:** [Boundary value problem](boundary-value-problem.md)

Find functions analytic on the two sides of a contour whose boundary values obey a prescribed jump, with suitable normalization at infinity and other distinguished points. An additive jump $J$ on a counterclockwise closed contour is solved by the [Cauchy integral formula](analysis.md#cauchy-integral-formula) $F(k)=(2\pi i)^{-1}\int J(\zeta)/(\zeta-k)d\zeta$, subject to the normalization and compatibility conditions. The [Sokhotski–Plemelj theorem](holomorphic-function.md#sokhotski-plemelj-theorem) verifies the jump.

### Sectorial half-line mKdV Riemann-Hilbert reconstruction

↑ **Parent:** [Riemann-Hilbert problem](#riemann-hilbert-problem)

Use the bounded columns supplied by [Volterra analyticity sectors for reverse-dispersion mKdV](integrable-systems.md#volterra-analyticity-sectors-for-reverse-dispersion-mkdv) and divide the necessary columns by their determinants. This gives a normalized meromorphic matrix on the six-ray contour $\arg k=m\pi/3$. The constant [scattering data](integrable-systems.md#scattering-data) connection matrices generate its jumps by conjugation with $e^{i(kx-4k^3t)\sigma_3}$. Zeros of column determinants require residue conditions; in a sufficiently small-data, zero-free regime only jumps are needed. The off-diagonal expansion coefficient reconstructs $q=-2i\lim_{k\to\infty}kM_{12}$ for this sign convention.

### Half-line NLS Riemann-Hilbert reconstruction

↑ **Parent:** [Riemann-Hilbert problem](#riemann-hilbert-problem)

Combine columns of the three normalized [Lax pair](integrable-systems.md#lax-pair) eigenfunctions in their common [Volterra analyticity sectors for a half-line NLS Lax pair](integrable-systems.md#volterra-analyticity-sectors-for-a-half-line-nls-lax-pair), dividing by the relevant determinants $a,d,d^\sharp,a^\sharp$. The resulting matrix is normalized to the identity at infinity and has jumps on the real and imaginary axes. Connection matrices determine each jump explicitly. Zeros of those determinants require residue conditions or local contour deformations.

### Negative-index scalar Riemann-Hilbert moment conditions

↑ **Parent:** [Riemann-Hilbert problem](#riemann-hilbert-problem)

Suppose a scalar canonical factor has exterior growth $X_-(z)\sim z^q$ with index $-q<0$, and the original exterior unknown must decay as $O(z^{-1})$. Dividing by the canonical factor gives an additive jump $D_+-D_-=g$ with exterior decay $O(z^{-q-1})$. The exterior [Cauchy integral](complex-analysis.md#cauchy-transform) expands in moments $-\int_Lt^jg(t)dt/(2\pi iz^{j+1})$. Its first $q$ coefficients must therefore vanish, yielding the displayed solvability conditions. Under this decay there is no nonzero entire [polynomial](polynomial.md) addition. A nonlocal moment appearing in $g$ must additionally agree with the moment of the reconstructed original jump.

### Matrix NLS reconstruction from a normalized Riemann-Hilbert problem

↑ **Parent:** [Riemann-Hilbert problem](#riemann-hilbert-problem)

Assume a regular invertible normalized [Riemann-Hilbert problem](#riemann-hilbert-problem) solution $\mu=I+\mu_1/k+\mu_2/k^2+\cdots$ with jump tending to the identity and conjugated by $e^{-i(kx+2k^2t)\sigma_3}$. Residuals of its two differential equations have no jump and vanish at infinity, so [Liouville theorem](complex-analysis.md#liouville-theorem) gives a [Lax pair](integrable-systems.md#lax-pair). Coefficient comparison gives the displayed reconstruction and $A=2Q$; compatibility yields $iQ_t-Q_{xx}\sigma_3+2Q^3\sigma_3=0$. A jump matrix tending to zero instead is inconsistent with the normalization. Recovering the initial jump from a prescribed initial potential still requires direct scattering.

### Canonical factorization of a rational scalar Riemann-Hilbert jump

↑ **Parent:** [Riemann-Hilbert problem](#riemann-hilbert-problem)

A rational jump with no zeros or poles on the contour can be split into factors analytic and nonvanishing on the two sides. The exterior factor may carry a power of $z$ recording the winding number. For a circle enclosing $0,\pm1$, the jump $G=z/(z^2-1)$ has the canonical factors $X_+=1$, $X_-=z-z^{-1}$. The exterior growth of $X_-$ imposes compatibility conditions when a Cauchy transform is required to vanish at infinity.

## Wiener-Hopf method

↑ **Parent:** [Boundary value problem](boundary-value-problem.md)

The Wiener-Hopf method solves a [boundary value problem](boundary-value-problem.md) with complementary half-line traces by [Wiener-Hopf factorization](#wiener-hopf-factorization) and additive splitting into upper- and lower-half-plane analytic functions. Analytic continuation gives a common entire function, whose growth and edge conditions determine its admissible value.

### Mixed Dirichlet-Neumann half-plane diffraction

↑ **Parent:** [Wiener-Hopf method](#wiener-hopf-method)

For a scalar wave above a line with a Dirichlet half and a Neumann half, the boundary transform factors into $\beta_+(\alpha)=\sqrt{k+\alpha}$ and $\beta_-(\alpha)=\sqrt{k-\alpha}$. For $e^{-i\omega t}$, the [limiting absorption principle](gravity-wave.md#limiting-absorption-principle) puts $-k$ below and $k$ above the inversion contour. With Dirichlet conditions on the negative half-line and incident tangential wavenumber $a$, pole subtraction gives the diffracted trace $U_+=2i\sqrt{k-a}/[(\alpha+a)\sqrt{k+\alpha}]$. Its large-transform decay gives a bounded field with a square-root edge trace. The normal derivative has an inverse-square-root singularity on the Dirichlet half; it is identically zero on the Neumann half.

### Wiener-Hopf factorization

↑ **Parent:** [Wiener-Hopf method](#wiener-hopf-method)

The plus factor is analytic and nonzero above the transform contour, and the minus factor below it. Their continuations inherit singularities and zeros in the opposite half-planes. Allocation of branch cuts and modal poles must agree with the physical outgoing continuation; no factor may have a zero inside its designated analytic domain.

### Wiener-Hopf equation

↑ **Parent:** [Wiener-Hopf method](#wiener-hopf-method)

A scalar Wiener-Hopf equation couples two [Half-range Fourier transforms](fourier-transform.md#half-range-fourier-transform) analytic in complementary half-planes. After dividing by a kernel factor, additive splitting separates the known forcing. Source poles, boundary terms and contour prescriptions are part of the problem data.

#### Wiener-Hopf kernel

↑ **Parent:** [Wiener-Hopf equation](#wiener-hopf-equation)

The scalar coefficient multiplying an unknown half-line transform in a [Wiener-Hopf equation](#wiener-hopf-equation) is its kernel. This is a transform-domain [function](function.md), distinct from the [null space](kernel-of-a-linear-map.md) of a [linear map](vector-space.md#linear-map). Its analytic zeros, [poles](isolated-singularity.md#pole) and [winding number](complex-analysis.md#winding-number) govern [Wiener-Hopf factorization](#wiener-hopf-factorization). For mixed scalar Helmholtz half-plane diffraction a typical kernel is the outgoing vertical [wavenumber](wave-equation.md#wavenumber) $\sqrt{k^2-\alpha^2}$.

#### Pole subtraction in a Wiener-Hopf equation

↑ **Parent:** [Wiener-Hopf equation](#wiener-hopf-equation)

A forcing pole can be split between analytic half-planes by subtracting a factor's value at the pole. For instance,

$$
\frac{L^+(k)}{k+k_0}=\frac{L^+(-k_0)}{k+k_0}
+\frac{L^+(k)-L^+(-k_0)}{k+k_0}.
$$

The second quotient has a removable pole and belongs to the plus expression; the first keeps the prescribed minus-side forcing pole. After [Wiener-Hopf factorization](#wiener-hopf-factorization), analytic continuation identifies an entire remainder, whose value is fixed by growth and edge conditions. The pole prescription must be stated together with the [Fourier transform](fourier-transform.md) convention.

## Fokas method

↑ **Parent:** [Boundary value problem](boundary-value-problem.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fokas_method)

The Fokas method uses a [global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem) between transformed boundary traces, complex spectral symmetries, and [contour integration](complex-analysis.md#contour-integration) to eliminate unknown traces or construct a numerical boundary scheme. The distinction between the domains of analyticity of the transforms and the decay sectors of spectral exponentials controls valid contour deformations.

### Two-trace half-line cubic dispersion representation

↑ **Parent:** [Fokas method](#fokas-method)

For $q_t+q_x-q_{xxx}=0$ on $x>0$, its [local relation](#local-relation) has flux $(1+k^2)q-ikq_x-q_{xx}$. With $Q_0(k)=\int_0^\infty e^{-ikx}q(x,0)dx$ and $G_j(k,T)=\int_0^T e^{w(k)s}\partial_x^jq(0,s)ds$, its [global relation](#global-relation-for-a-linear-boundary-value-problem) is $e^{wT}\widehat q=Q_0+(1+k^2)G_0-ikG_1-G_2$. In $D_+=\{\operatorname{Im}k>0,\operatorname{Re}w(k)<0\}$, choose the other cubic root $\nu(k)$ in the lower half-plane. Then the known spectral density is $-Q_0(\nu)+(k^2-\nu^2)G_0-i(k-\nu)G_1$. The remaining final-state transform has zero integral around $\partial D_+$ by the [Cauchy integral theorem](complex-analysis.md#cauchy-s-integral-theorem) and exponential decay. The full boundary includes the real axis and the hyperbola $\operatorname{Im}k=\sqrt{1+3(\operatorname{Re}k)^2}$, oriented with the domain on the left.

### Boundary spectral representation of a holomorphic function on a semistrip

↑ **Parent:** [Fokas method](#fokas-method)

For a [holomorphic function](holomorphic-function.md) on $x>0$, $0<y<l$, define boundary spectra by counterclockwise traversal: $\rho_L=\int_{il}^0e^{-ikw}f(w)\,dw$, $\rho_B=\int_0^\infty e^{-ikx}f(x)\,dx$, and $\rho_T=-e^{kl}\int_0^\infty e^{-ikx}f(x+il)\,dx$. The displayed reconstruction follows from the [Cauchy integral formula](analysis.md#cauchy-integral-formula) and the ray identity $\int_0^{e^{i\theta}\infty}e^{ik(z-w)}\,dk=i/(z-w)$ whenever that exponential decays. The three rays are selected by the inward normals of the three sides.

// Target: analysis.bigb

### Quadrant modified Helmholtz spectral reconstruction

↑ **Parent:** [Fokas method](#fokas-method)

For $\lambda>0$, put $a=k-\lambda/k$, $b=k+\lambda/k$. The spectral integral uses the positive real and positive imaginary rays, both oriented outward. On the first ray its density is $\rho_x=i\int_0^\infty e^{-iax}[bq(x,0)-q_y(x,0)]dx$; on the second it is $\rho_y=\int_0^\infty e^{by}[a q(0,y)-i q_x(0,y)]dy$. The [global relation](#global-relation-for-a-linear-boundary-value-problem) $\rho_x+\rho_y=0$ holds in the third spectral quadrant. Primitives from the corner and from each infinite boundary end give an additive [Riemann-Hilbert problem](#riemann-hilbert-problem). Their limits are $-q$ at infinity and $q$ at zero, which explains the factor $1/(4\pi i)$.

### Neumann spectral formula for half-line constant drift

↑ **Parent:** [Fokas method](#fokas-method)

The reflected [global relation](#global-relation-for-a-linear-boundary-value-problem) expresses the unknown value trace in terms of the prescribed derivative trace. Multiplying the [half-line drift null contour identity](fourier-transform.md#half-line-drift-null-contour-identity) by $(ik+\alpha)/(ik)$ removes the reflected time-dependent transform. Its pole at $k=0$ lies below the contour and is not crossed. The formula concerns the derivative $q_x(0,t)$, rather than the outward derivative $-q_x(0,t)$.

### Dirichlet spectral formula for half-line constant drift

↑ **Parent:** [Fokas method](#fokas-method)

Let $I_C[F]=(2\pi)^{-1}\int_Ce^{ikx-(k^2-i\alpha k)t}F(k)dk$. The [drift-diffusion half-line global relation](#drift-diffusion-half-line-global-relation) and the [half-line drift null contour identity](fourier-transform.md#half-line-drift-null-contour-identity) give the formula in the secondary title. Its real-space kernel is the difference of two drifted [Gaussian heat kernels](diffusion-equation.md#gaussian-heat-kernel), and its boundary-forcing kernel is $x(2\sqrt\pi t^{3/2})^{-1}\exp[-(x+\alpha t)^2/(4t)]$. This kernel is an [approximate identity](fourier-analysis.md#approximate-identity) in time as $x\downarrow0$, which verifies the [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition).

### Local relation

↑ **Parent:** [Fokas method](#fokas-method)

A spectral-parameter-dependent divergence identity equivalent to a partial differential equation. Integrating it over a space-time region gives a [global relation](#global-relation-for-a-linear-boundary-value-problem) between transformed initial and boundary data. For the half-line free [Schrödinger equation](mathematical-physics.md#schrodinger-equation), take $P=e^{-ikx+ik^2t}q$ and $Q=e^{-ikx+ik^2t}(-kq+iq_x)$.

### Dispersion symmetry elimination of a boundary trace

↑ **Parent:** [Fokas method](#fokas-method)

To eliminate an unknown boundary transform by a [dispersion relation](dispersion-relation.md) symmetry, evaluate the [global relation](#global-relation-for-a-linear-boundary-value-problem) at $\nu(k)$ only where the spatial transform remains analytic. Substitute the resulting trace identity into the contour representation. An unwanted transform vanishes only if its transformed argument and exponential admit a valid [contour deformation](complex-analysis.md#contour-deformation) and decay estimate. For constant drift, $\nu(k)=i\alpha-k$ maps the upper domain $\operatorname{Re}(k^2-i\alpha k)<0$ into the lower transform half-plane.

#### Cubic-dispersion elimination of one missing boundary trace

↑ **Parent:** [Dispersion symmetry elimination of a boundary trace](#dispersion-symmetry-elimination-of-a-boundary-trace)

For the [backward-sign Airy half-line global relation](integrable-systems.md#backward-sign-airy-half-line-global-relation), suppose exactly one trace of derivative order $j\in\{0,1,2\}$ is unknown. Its spectral multiplier is a constant times $k^r$, $r=2-j$. Use the [rotated null contours for half-range Fourier inversion](fourier-transform.md#rotated-null-contours-for-half-range-fourier-inversion) with the displayed coefficients. The unknown contribution becomes an integral over the boundary of the middle upper sector $\pi/3<\arg k<2\pi/3$. There $\operatorname{Im}k^3<0$, so

$$
e^{-ik^3t}F_j(k,t)=\int_0^t e^{-ik^3(t-s)}f_j(s)\,ds
$$

is bounded, while $e^{ikx}$ decays exponentially. The [Cauchy integral theorem](complex-analysis.md#cauchy-s-integral-theorem) therefore removes that entire unknown contribution. The resulting solution depends on the initial transform and the two prescribed boundary transforms only.

// Target: analysis.bigb

#### Cubic Stokes dispersion symmetry

↑ **Parent:** [Dispersion symmetry elimination of a boundary trace](#dispersion-symmetry-elimination-of-a-boundary-trace)

For the [linear dispersive Stokes equation](integrable-systems.md#linear-dispersive-stokes-equation), $\omega(\nu)=\omega(k)$ factors as $(\nu-k)(\nu^2+k\nu+k^2-1)=0$. In $D_+=\{\operatorname{Im}k>0,\operatorname{Re}\omega(k)<0\}$ the two displayed other roots lie in the lower half-plane, so both can be used in the [global relation](#global-relation-for-a-linear-boundary-value-problem). To check the root locations, at $k=ib$ they have imaginary part $-b/2$. A root could reach the real axis only where $\operatorname{Re}\omega(k)=0$, so continuity preserves their signs throughout this connected domain. The branch points $\pm2/\sqrt3$ lie outside its closure. The weights $A_1=(k-\nu_2)/(\nu_1-\nu_2)$ and $A_2=(\nu_1-k)/(\nu_1-\nu_2)$ obey $A_1+A_2=1$ and $\nu_j'=-A_j$.

### Upper-quadrant cancellation of reflected boundary transforms

↑ **Parent:** [Fokas method](#fokas-method)

If $P(k)$ is analytic in the upper half-plane with suitable growth, paired integrals along the positive real and imaginary rays cancel when their exponential is $e^{ik(x+iy)}$ with $x,y>0$. For $0<y<\ell$, the analogous pair along the imaginary and negative real rays cancels with $e^{ik(x+i(y-\ell))}$. These two applications of the [Cauchy integral theorem](complex-analysis.md#cauchy-s-integral-theorem) eliminate reflected unknown transforms from a strip [global relation](#global-relation-for-a-linear-boundary-value-problem); an individual ray integral need not vanish.

## Global relation for a linear boundary value problem

↑ **Parent:** [Boundary value problem](boundary-value-problem.md)

A global relation is an identity connecting transforms or integrals of the boundary traces of a solution. For a formally self-adjoint operator $L=\Delta-k^2$, [Green second identity](partial-differential-equation.md#green-second-identity) gives

$$
\int_{\partial\Omega}(v\partial_nu-u\partial_nv)\,ds=0
$$

for every homogeneous adjoint solution $Lv=0$. Exponential adjoint families turn this into a spectral identity between the [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) and unknown [normal derivative](differential-geometry.md#normal-derivative).

### Dirichlet spectral formula for Airy flow with negative transport

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

Let $F(k)=\int_0^\infty e^{-ikx}q_0(x)dx$ and $G_0(k,t)=\int_0^t e^{w(k)s}g_0(s)ds$. Using the roots of [cubic dispersion symmetry with negative transport](integrable-systems.md#cubic-dispersion-symmetry-with-negative-transport), put $\mathcal T F=[(k-\nu_2)F(\nu_1)+(\nu_1-k)F(\nu_2)]/(\nu_1-\nu_2)$. The [Fokas method](#fokas-method) formula is an initial real-line integral minus an integral over $\partial D_+$ of $e^{ikx-wt}[\mathcal TF+(3k^2+1)G_0]$, both divided by $2\pi$. The boundary is oriented with $D_+$ on the left. Its unknown final-state transform has zero integral by analyticity and upper-half-plane decay.

### Finite-interval Airy global relation

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

For the [Airy equation](integrable-systems.md#airy-equation) $q_t+q_{xxx}=0$ on $0<x<L$, define $F_j=\int_0^t e^{-ik^3s}\partial_x^jq(0,s)ds$ and $G_j$ analogously at $L$. Set $\mathcal F=k^2F_0-ikF_1-F_2$ and $\mathcal G=k^2G_0-ikG_1-G_2$. Integrating the [local relation](#local-relation) with flux $-q_{xx}-ikq_x+k^2q$ proves the displayed [global relation](#global-relation-for-a-linear-boundary-value-problem). The [dispersion relation](dispersion-relation.md) is invariant under multiplication of $k$ by a cube root of unity; the resulting three equations determine the three missing boundary transforms for data $q(0,t),q(L,t),q_x(L,t)$.

#### Finite-interval Airy spectral determinant

↑ **Parent:** [Finite-interval Airy global relation](#finite-interval-airy-global-relation)

Here $\alpha=e^{2\pi i/3}$. The missing-trace matrix has determinant $-\sqrt3k\Delta(k)$. Its nonzero zeros are the [eigenvalues](linear-operator-theory.md#eigenvalue) in the parametrization $Av=ik^3v$ of $A=-d^3/dx^3$ with $v(0)=v(L)=v'(L)=0$. [Integration by parts](calculus.md#integration-by-parts) gives $\operatorname{Re}\langle v,Av\rangle=-|v'(0)|^2/2$. No nonzero zero lies in $\operatorname{Re}(-ik^3)\leq0$: on its boundary the determinant equation reduces, after rotation, to an equality between a unit-modulus exponential and $\cosh u-i\sqrt3\sinh u$, whose modulus exceeds one unless $u=0$. The zero at the origin is removable in the original boundary problem. There are nevertheless infinitely many genuine negative [eigenvalues](linear-operator-theory.md#eigenvalue) of $A$, obtained from $e^{-3s/2}=2\cos(\sqrt3s/2+\pi/3)$, $s>0$, with $k=-is/L$. Absence of contour poles in the [Fokas method](#fokas-method) does not imply absence of [discrete spectrum](functional-analysis.md#discrete-spectrum) of the operator.

### Semistrip Laplace spectral global relation

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

Let $q$ be a real [harmonic function](partial-differential-equation.md#harmonic-function) in a semistrip, $g_0(x)=q(x,0)$, $g_l(x)=q(x,l)$ and $h(y)=q(0,y)$. Let $G_j,N_j$ be the negative-exponential [Half-range Fourier transforms](fourier-transform.md#half-range-fourier-transform) of $g_j$ and $q_y(x,j)$, and put $H(k)=\int_0^l e^{ky}h(y)\,dy$, $W(k)=\int_0^l e^{ky}q_x(0,y)\,dy$. The [closed differential form](differential-form.md#closed-differential-form) $e^{-ikz}q_z\,dz$ has zero boundary integral. [Integration by parts](calculus.md#integration-by-parts) of tangential derivatives cancels all corner values and gives the displayed [global relation](#global-relation-for-a-linear-boundary-value-problem), for $\operatorname{Im}k\leq0$.

// Target: analysis.bigb

### Drift-diffusion half-line global relation

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

For $q_t=q_{xx}+\alpha q_x$ on $x>0$, write $Q(k)=\int_0^\infty e^{-ikx}q(x,0)dx$ and $G_j(k,t)=\int_0^t e^{\omega(k)s}\partial_x^jq(0,s)ds$. Twice integrating by parts gives $e^{\omega(k)t}\widehat q(k,t)=Q(k)-G_1(k,t)-(ik+\alpha)G_0(k,t)$ in the lower transform half-plane. The [dispersion relation](dispersion-relation.md) is invariant under $k\mapsto i\alpha-k$. This [global relation](#global-relation-for-a-linear-boundary-value-problem) eliminates one unknown boundary trace after the symmetry maps the inversion contour into the transform's analytic domain.

### Half-line linear dispersive Stokes global relation

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

For the [linear dispersive Stokes equation](integrable-systems.md#linear-dispersive-stokes-equation) $q_t+q_x+q_{xxx}=0$, let $\omega(k)=i(k-k^3)$. Its [local relation](#local-relation) is obtained with $X=q_{xx}+ikq_x+(1-k^2)q$. Integrating $\partial_t(e^{-ikx+\omega t}q)+\partial_x(e^{-ikx+\omega t}X)=0$ over the half-line gives the displayed [global relation](#global-relation-for-a-linear-boundary-value-problem), with negative-exponential [Half-range Fourier transforms](fourier-transform.md#half-range-fourier-transform) and $G_j(k,t)=\int_0^t e^{\omega(k)s}\partial_x^jq(0,s)\,ds$. The spatial transforms are [holomorphic](holomorphic-function.md) for $\operatorname{Im}k<0$, whereas the finite-time boundary transforms are [entire functions](holomorphic-function.md#entire-function).

#### Dirichlet spectral representation for the linear dispersive Stokes equation

↑ **Parent:** [Half-line linear dispersive Stokes global relation](#half-line-linear-dispersive-stokes-global-relation)

Let $A_j$ be the weights of the [cubic Stokes dispersion symmetry](#cubic-stokes-dispersion-symmetry) and set $F(k)=\sum_jA_j(k)\widehat q_0(\nu_j(k))$. Orient $\partial D_+$ with $D_+$ on its left. Evaluating the [global relation](#global-relation-for-a-linear-boundary-value-problem) at its two lower-half-plane roots and interpolating the linear expression $ikG_1+G_2$ removes both unknown boundary traces. The resulting [Fokas method](#fokas-method) formula is

$$
q(x,t)=\frac1{2\pi}\int_{\mathbb R}e^{ikx-\omega t}\widehat q_0(k)\,dk+\frac1{2\pi}\int_{\partial D_+}e^{ikx-\omega t}\bigl[(1-3k^2)G_0(k,t)-F(k)\bigr]dk.
$$

The discarded transform of the solution is [holomorphic](holomorphic-function.md) in $D_+$ and has zero [integral](integral.md) after closing its [contour](complex-analysis.md#complex-integration-contour) for $x>0$. Initial compatibility and sufficient smoothness and spatial decay are required. At the boundary, use a fixed time horizon later than $t$ before [Fourier inversion](fourier-analysis.md#fourier-inversion-theorem), to avoid an endpoint half-value.

### Half-line Schrodinger boundary-trace elimination

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

Orient the upper-quadrant contour from $i\infty$ down to zero and then to $+\infty$. The reflected half-line transform has zero inverse contribution for positive $x$. Adding $c$ times this contribution, and deforming boundary integrands through the second quadrant where $|e^{ikx-ik^2(t-\tau)}|\leq e^{-x\operatorname{Im}k}$, gives boundary coefficients $(1-c)k\widetilde g_0-i(1+c)\widetilde g_1$. Thus $c=-1$ removes the unknown Neumann trace for a prescribed Dirichlet value, while $c=1$ removes the unknown Dirichlet trace for a prescribed Neumann value. The initial reflected term has coefficient $c$ and cannot be discarded after the time-dependent spectral decomposition.

### Finite-time spectral boundary transform

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

A boundary trace transformed over a finite time interval using the [dispersion relation](dispersion-relation.md) of a linear [partial differential equation](partial-differential-equation.md). For integrable trace data and a polynomial dispersion function, it is an [entire function](holomorphic-function.md#entire-function) of the complex [spectral parameter](integrable-systems.md#spectral-parameter). Its growth depends on $\operatorname{Re}\omega(k)$; multiplying by $e^{-\omega(k)t}$ changes the integrand to the causal factor $e^{-\omega(k)(t-s)}$.

#### Finite-horizon extension of a boundary transform

↑ **Parent:** [Finite-time spectral boundary transform](#finite-time-spectral-boundary-transform)

In a [Fokas method](#fokas-method) boundary [integral](integral.md) over $\partial D_+$, where $\operatorname{Re}\omega<0$ inside, the contribution of replacing $G(k,t)$ by $G(k,T)$ is an [integral](integral.md) of $e^{ikx}\int_t^T e^{\omega(k)(s-t)}g(s)\,ds$ times an [holomorphic](holomorphic-function.md) coefficient. For $x>0$ it vanishes by the [Cauchy integral theorem](complex-analysis.md#cauchy-s-integral-theorem) and the exponential decay in the upper domain. The transformed amplitude is then independent of the observation time, which simplifies differentiation of the [partial differential equation](partial-differential-equation.md). Temporal inversion at $0<t<T$ recovers the full boundary value rather than the half-value of a truncated transform at its endpoint.

### Polygonal modified Helmholtz global relation

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

For $u_{z\bar z}=\beta^2u$, pull back its spectral [closed differential one-form](differential-form.md#closed-differential-one-form) along each straight side $z=m_j+sh_j$. Under counterclockwise traversal and outward [normal derivatives](differential-geometry.md#normal-derivative) $q_j$, the side density is $i e^{-i\beta(\lambda z-\bar z/\lambda)}[|h_j|q_j+\beta(\lambda h_j+\bar h_j/\lambda)g_j]$, where $g_j$ is the [Dirichlet boundary data](differential-equation.md#dirichlet-boundary-data). The [Generalized Stokes theorem](differential-form.md#generalized-stokes-theorem) gives the displayed [global relation](#global-relation-for-a-linear-boundary-value-problem). Clockwise traversal reverses the normal-derivative coefficient; all orientations must be changed consistently.

#### Dirichlet reconstruction in an equilateral triangle

↑ **Parent:** [Polygonal modified Helmholtz global relation](#polygonal-modified-helmholtz-global-relation)

For equal oriented [Dirichlet boundary data](differential-equation.md#dirichlet-boundary-data) on all three sides and a uniquely solvable elliptic problem, rotation invariance makes their outward [normal derivatives](differential-geometry.md#normal-derivative) equal. Pairing the global relation with its [Schwarz conjugation of a spectral function](complex-analysis.md#schwarz-conjugation-of-a-spectral-function) at $\ell(k+\lambda/k)=2\pi in$ determines every Fourier coefficient of the common normal trace. The zero mode at $\lambda=0$ follows from zero total flux. At negative parameters, uniqueness and possible removable spectral denominators must be checked rather than assumed.

### Half-line drift global relation

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

For the [advection-diffusion equation](diffusion-equation.md#advection-diffusion-equation) $u_t=u_{xx}+\alpha u_x$ on $x>0$, the spectral [divergence form](analysis.md#divergence-form) uses $\omega=k^2-i\alpha k$ and factor $e^{-ikx+\omega t}$. With negative-exponential [Half-range Fourier transforms](fourier-transform.md#half-range-fourier-transform), integration gives the displayed [global relation](#global-relation-for-a-linear-boundary-value-problem) for $\operatorname{Im}k\le0$. The boundary transform $G_1$ refers to $u_x(0,t)$, the negative of the outward [normal derivative](differential-geometry.md#normal-derivative).

#### Exponential-decay contour for half-line drift diffusion

↑ **Parent:** [Half-line drift global relation](#half-line-drift-global-relation)

For $q_t=q_{xx}+\alpha q_x$ with $\alpha>0$, the [dispersion relation](dispersion-relation.md) is $\omega=k^2-i\alpha k$ and its symmetry is $\nu=i\alpha-k$. On the upper domain $\operatorname{Re}\omega<0$, $\operatorname{Im}k>\alpha$ and therefore $\operatorname{Im}\nu<0$. After removing the unknown trace through the [global relation](#global-relation-for-a-linear-boundary-value-problem), deform the boundary [contour](complex-analysis.md#complex-integration-contour) to the displayed two rays, with $0<\theta<\pi/4$, oriented from left infinity to $i\alpha$ to right infinity. The factor $e^{ikx}$ decays like $e^{-r x\sin\theta}$, while $e^{-\omega t}$ has Gaussian decay for large $r$. Apparent poles introduced by splitting a finite-time forcing transform must be treated as removable singularities of the unsplit expression.

### Collocation points for a global relation

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

These are chosen complex values of a [spectral parameter for a linear boundary value problem](#spectral-parameter-for-a-linear-boundary-value-problem) at which a truncated [global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem) is enforced. Their directions and magnitudes determine which boundary side and which tangential mode are tested. Suitable row combinations can give much better conditioning than arbitrary raw samples.

### Conjugate global relations for the modified Helmholtz equation

↑ **Parent:** [Global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem)

The two [modified Helmholtz adjoint plane waves](partial-differential-equation.md#modified-helmholtz-adjoint-plane-wave) $v_\lambda$ and $\widetilde v_\lambda=\overline{v_{\overline\lambda}}$ give boundary identities $\mathcal G(\lambda)=0$ and $\widetilde{\mathcal G}(\lambda)=0$. For real solution traces, $\widetilde{\mathcal G}(\lambda)=\overline{\mathcal G(\overline\lambda)}$. Reality is needed for this conjugation argument; the parametrization separately yields the reciprocal identity $\widetilde{\mathcal G}(\lambda)=\mathcal G(1/\lambda)$.

#### Rotationally invariant Neumann reconstruction in an equilateral triangle

↑ **Parent:** [Conjugate global relations for the modified Helmholtz equation](#conjugate-global-relations-for-the-modified-helmholtz-equation)

For the [modified Helmholtz equation](partial-differential-equation.md#modified-helmholtz-equation) $\Delta q-4\lambda q=0$ with identical oriented outward [Neumann boundary data](differential-equation.md#neumann-boundary-data) on all sides of an [equilateral triangle](euclidean-geometry.md#equilateral-triangle), uniqueness forces rotation invariance. Put $\chi(k)=l(k+\lambda/k)/2$, $\Psi(k)=\int_{-l/2}^{l/2}e^{(k+\lambda/k)s}f(s)ds$, and $a=e^{2\pi i/3}$. At $\chi(k_n)=i\pi n$, paired [global relations](#global-relation-for-a-linear-boundary-value-problem) give

$$
Q_n=\frac{i[\cosh\chi(\bar a k_n)\Psi(k_n)+(-1)^n\Psi(\bar a k_n)+\Psi(a k_n)]}{(k_n-\lambda/k_n)\sinh\chi(\bar a k_n)}.
$$

For $\lambda>0$ one may choose $k_n=i[\pi n/l+\sqrt{(\pi n/l)^2+\lambda}]$; both denominator factors are nonzero. The derivation retains the tangential-derivative term in each side spectrum. Its endpoint contribution vanishes at these samples because rotation invariance makes all vertex values equal. For $\lambda=0$ the data must have zero total flux and an additive constant remains; negative parameters at [Neumann Laplacian](partial-differential-equation.md#neumann-laplacian) eigenvalues require the [Fredholm solvability condition](sturm-liouville-theory.md#fredholm-solvability-condition) and allow homogeneous additions.

#### Sine collocation of square modified Helmholtz global relations

↑ **Parent:** [Conjugate global relations for the modified Helmholtz equation](#conjugate-global-relations-for-the-modified-helmholtz-equation)

On the square $[-1,1]^2$, write normal traces in $\phi_n(s)=\sin[n\pi(s+1)/2]$. Set $p_n=n\pi/2$, $\omega_n=\sqrt{k^2+p_n^2}$, $r_n=(\omega_n+p_n)/k$. Paired spectral samples $\{r_n,r_n^{-1}\}$, $\{-r_n,-r_n^{-1}\}$, $\{ir_n,i/r_n\}$, $\{-ir_n,-i/r_n\}$ give adjoint tests $e^{\mp\omega_ny}\phi_n(x)$ and $e^{\mp\omega_nx}\phi_n(y)$. Each test vanishes on the adjacent sides, removing their unknown [normal derivatives](differential-geometry.md#normal-derivative).

##### Square modified Helmholtz Dirichlet-to-Neumann coefficients

↑ **Parent:** [Sine collocation of square modified Helmholtz global relations](#sine-collocation-of-square-modified-helmholtz-global-relations)

Let $R_{jn}=\int_{\partial\Omega}f\partial_nv_{jn}ds$ for a square sine adjoint test, and put $\rho_{jn}=e^{-\omega_n}R_{jn}$, $\delta_n=e^{-2\omega_n}$. The opposite-side normal-trace coefficients obey

$$
c_{Bn}=\frac{\rho_{Bn}-\delta_n\rho_{Tn}}{1-\delta_n^2},\qquad c_{Tn}=\frac{\rho_{Tn}-\delta_n\rho_{Bn}}{1-\delta_n^2},
$$

with the same formulas for $L,R$. When the known [Dirichlet boundary condition](differential-equation.md#dirichlet-boundary-condition) is integrated exactly, these are exact coefficients, since [orthogonality](inner-product.md#orthogonal-vectors) eliminates all other unknown modes.

##### Diagonal dominance of paired square global-relation collocation

↑ **Parent:** [Sine collocation of square modified Helmholtz global relations](#sine-collocation-of-square-modified-helmholtz-global-relations)

For [sine collocation of square modified Helmholtz global relations](#sine-collocation-of-square-modified-helmholtz-global-relations), each opposite-side mode has a scaled matrix

$$
\begin{pmatrix}1&\delta_n\\\delta_n&1\end{pmatrix},\qquad\delta_n=e^{-2\sqrt{k^2+(n\pi/2)^2}}<e^{-\pi}.
$$

The assembled system has [strict diagonal dominance](vector-space.md#strictly-diagonally-dominant-matrix), and its [spectral condition number of a positive-definite matrix](quadratic-form.md#spectral-condition-number-of-a-positive-definite-matrix) is below $(1+e^{-\pi})/(1-e^{-\pi})<1.091$. The conclusion concerns the explicit paired sine rows, not arbitrary uncombined complex rows.

## Spectral parameter for a linear boundary value problem

↑ **Parent:** [Boundary value problem](boundary-value-problem.md)

A complex parameter labels auxiliary solutions of a linear [differential equation](differential-equation.md), such as exponential adjoint solutions used in a [global relation for a linear boundary value problem](#global-relation-for-a-linear-boundary-value-problem). It need not be a discrete [eigenvalue](linear-operator-theory.md#eigenvalue) or a parameter of a nonlinear [Lax pair](integrable-systems.md#lax-pair). Analytic dependence on it allows transformed boundary identities to be sampled or inverted.

## Boundary lifting

↑ **Parent:** [Boundary value problem](boundary-value-problem.md)

Subtract a known function with the required boundary trace so that the remaining unknown has homogeneous [boundary conditions](differential-equation.md#boundary-condition). For an interval with [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) $g(t),h(t)$, $\ell=(1-x/L)g+(x/L)h$ is a simple lifting. In $w_t=w_{xx}-cw$, $z=w-\ell$ has forcing $-\ell_t-c\ell$ and zero endpoint values. This improves [Fourier sine series](fourier-series.md#fourier-sine-series) convergence.

### Uniform half-line Schrodinger representation by boundary lifting

↑ **Parent:** [Boundary lifting](#boundary-lifting)

For the [free Schrodinger equation](mathematical-physics.md#free-schrodinger-equation) with compatible smooth initial and boundary data, subtract $g(t)e^{-x}$ before taking a [Fourier sine transform](fourier-transform.md#fourier-sine-transform). The lifted initial datum vanishes at the endpoint, making its sine transform $O(k^{-2})$ if its second derivative is integrable. The transformed forcing is $k(ig-g')/(1+k^2)$; time integration followed by [integration by parts](calculus.md#integration-by-parts) makes its solution contribution uniformly $O(k^{-3})$. An integrable spectral majorant proves [uniform convergence](sequence-and-series.md#uniform-convergence) even at the compatible initial-boundary corner.

## ↑ Ancestors (6)

1. [Ordinary differential equation](differential-equation.md#ordinary-differential-equation)
2. [Differential equation](differential-equation.md)
3. [Analysis](analysis.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (37)

- [Blasius boundary layer](continuum-mechanics.md#blasius-boundary-layer)
- [Dead loading](elasticity-physics.md#dead-loading)
- [Degenerate ordinary differential equation](differential-equation.md#degenerate-ordinary-differential-equation)
- [Electrostatics](electrostatics.md)
- [Initial value problem](differential-equation.md#initial-value-problem)
- [Multigrid method](multigrid-method.md)
- [Neumann boundary data](differential-equation.md#neumann-boundary-data)
- [Neumann boundary-value problem](#neumann-boundary-value-problem)
- [Oblique derivative boundary condition](#oblique-derivative-boundary-condition)
- [One-third-power similarity of an indented channel boundary layer](viscous-fluid-flow.md#one-third-power-similarity-of-an-indented-channel-boundary-layer)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-72.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-72.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-73.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-81.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-2.md#16b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-70.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-70.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-3.md#7a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-337.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-337.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-337.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-2.md#5b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-2.md#14a/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2001/paper-2.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#10/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1.md#3/b/solution)
- [Solution](past-exam-of-the-mphil-in-nuclear-energy-course-of-the-university-of-cambridge/2019/paper-ne1.md#2/d/solution)
- [Solution](past-exam-of-the-mphil-in-nuclear-energy-course-of-the-university-of-cambridge/2021/paper-ne1.md#3/c/ii/solution)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2016/paper-2.md#section-b/b7/solution)
- [Solution](past-exam-of-the-soft-matter-and-biological-physics-course-of-the-university-of-cambridge/2012/paper-1.md#3/c/solution)
- [Singular perturbation](singular-perturbation.md)
- [Stationary solution](differential-equation.md#stationary-solution)
- [Wiener-Hopf method](#wiener-hopf-method)
