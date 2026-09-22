# Calculus of variations

↑ **Parent:** [Analysis](analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Calculus_of_variations)

Calculus of variations finds [stationary points](#stationary-point) of [functionals](#functional), often among [functions](function.md) or [regular curves](differential-geometry.md#regular-curve).

**Table of contents**

- [Log-cosh energy on a Sobolev space](#log-cosh-energy-on-a-sobolev-space)
- [Weierstrass excess function](#weierstrass-excess-function)
  - [Weierstrass necessary condition](#weierstrass-necessary-condition)
    - [Bounded slope integrands force strong minima to be global](#bounded-slope-integrands-force-strong-minima-to-be-global)
  - [Strengthened Weierstrass condition](#strengthened-weierstrass-condition)
    - [Weierstrass sufficient condition](#weierstrass-sufficient-condition)
- [Strong local minimizer of a variational integral](#strong-local-minimizer-of-a-variational-integral)
  - [Coercivity transfers strong minimality to L1 minimality](#coercivity-transfers-strong-minimality-to-l1-minimality)
- [Weak local minimizer of a variational integral](#weak-local-minimizer-of-a-variational-integral)
  - [Periodic slopes give weak minima without strong minima](#periodic-slopes-give-weak-minima-without-strong-minima)
- [Length extremals from a constant quadratic energy](#length-extremals-from-a-constant-quadratic-energy)
- [Euler-Lagrange equation for a second-derivative functional](#euler-lagrange-equation-for-a-second-derivative-functional)
  - [Clamped fourth-order variational extremal on a quarter period](#clamped-fourth-order-variational-extremal-on-a-quarter-period)
  - [Beltrami identity for a second-derivative functional](#beltrami-identity-for-a-second-derivative-functional)
  - [Natural boundary conditions for second-derivative functionals](#natural-boundary-conditions-for-second-derivative-functionals)
- [Extremal](#extremal)
- [Variational principle](#variational-principle)
  - [Variational projection onto an involutive symmetry](#variational-projection-onto-an-involutive-symmetry)
- [Quadratic minor null Lagrangian](#quadratic-minor-null-lagrangian)
- [Brachistochrone problem](#brachistochrone-problem)
  - [Fixed-length brachistochrone between equal-height endpoints](#fixed-length-brachistochrone-between-equal-height-endpoints)
  - [Brachistochrone on a hemispherical ramp](#brachistochrone-on-a-hemispherical-ramp)
  - [Maximum-depth bound for a brachistochrone](#maximum-depth-bound-for-a-brachistochrone)
  - [Brachistochrone on a horizontal half-cylinder](#brachistochrone-on-a-horizontal-half-cylinder)
- [Travel-time minimization with speed proportional to squared radius](#travel-time-minimization-with-speed-proportional-to-squared-radius)
- [Gamma-convergence](#gamma-convergence)
- [Variational problem](#variational-problem)
- [Direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations)
  - [Lavrentiev phenomenon](#lavrentiev-phenomenon)
  - [Power-law comparison for vanishing derivative regularization](#power-law-comparison-for-vanishing-derivative-regularization)
  - [Tonelli existence theorem](#tonelli-existence-theorem)
  - [Weak lower semicontinuity of convex gradient energies](#weak-lower-semicontinuity-of-convex-gradient-energies)
  - [Symmetric elliptic Dirichlet energy with a nonpositive potential](#symmetric-elliptic-dirichlet-energy-with-a-nonpositive-potential)
  - [Screened sine-Gordon energy](#screened-sine-gordon-energy)
    - [Failure of the source-size bound for the screened sine-Gordon equation](#failure-of-the-source-size-bound-for-the-screened-sine-gordon-equation)
  - [Minimizing sequence](#minimizing-sequence)
    - [Oscillating minimizing sequence with no minimizer](#oscillating-minimizing-sequence-with-no-minimizer)
  - [Bounded slope condition](#bounded-slope-condition)
  - [Comparison principle for convex variational integrals](#comparison-principle-for-convex-variational-integrals)
- [Functional](#functional)
  - [Quadratic functional](#quadratic-functional)
    - [Resonant sine modes of a quadratic variational integral](#resonant-sine-modes-of-a-quadratic-variational-integral)
    - [Stationary values of a quadratic functional with a quadratic constraint](#stationary-values-of-a-quadratic-functional-with-a-quadratic-constraint)
  - [Epigraph](#epigraph)
  - [Functional derivative](#functional-derivative)
    - [Functional Taylor expansion](#functional-taylor-expansion)
    - [Functional chain rule](#functional-chain-rule)
  - [Energy functional](#energy-functional)
    - [Critical point of an energy functional](#critical-point-of-an-energy-functional)
    - [p-energy](#p-energy)
  - [Lagrangian](#lagrangian)
  - [Variation](#variation)
    - [First variation](#first-variation)
      - [Fundamental lemma of the calculus of variations](#fundamental-lemma-of-the-calculus-of-variations)
- [Stationary point](#stationary-point)
  - [Stationary points of a cosine-modulated Gaussian](#stationary-points-of-a-cosine-modulated-gaussian)
  - [Stationary points with real cube-root factors](#stationary-points-with-real-cube-root-factors)
  - [Stationary points under an increasing outer function](#stationary-points-under-an-increasing-outer-function)
- [Dirichlet principle](#dirichlet-principle)
  - [Quadratic energy minimization by the parallelogram law](#quadratic-energy-minimization-by-the-parallelogram-law)
  - [Sharp radial Dirichlet energy inequality](#sharp-radial-dirichlet-energy-inequality)
- [Optical ray in cylindrical coordinates](#optical-ray-in-cylindrical-coordinates)
  - [Helical extremal](#helical-extremal)
- [Noether theorem](#noether-theorem)
  - [Mass-weighted oscillator symmetries](#mass-weighted-oscillator-symmetries)
  - [Time-translation symmetry](#time-translation-symmetry)
  - [Noether second theorem](#noether-second-theorem)
    - [Noether identity for abelian scalar gauge symmetry](#noether-identity-for-abelian-scalar-gauge-symmetry)
  - [Noether conserved quantity for a mechanical point symmetry](#noether-conserved-quantity-for-a-mechanical-point-symmetry)
    - [Action symmetry](#action-symmetry)
- [Second variation](#second-variation)
  - [Coercive positivity of a second variation](#coercive-positivity-of-a-second-variation)
  - [Legendre necessary condition](#legendre-necessary-condition)
    - [Strengthened Legendre condition](#strengthened-legendre-condition)
  - [Jacobi equation](#jacobi-equation)
    - [Jacobi identity for the second variation](#jacobi-identity-for-the-second-variation)
  - [Conjugate point](#conjugate-point)
    - [Jacobi positivity criterion](#jacobi-positivity-criterion)
      - [Regularized Jacobi criterion for a degenerate second variation](#regularized-jacobi-criterion-for-a-degenerate-second-variation)
    - [Multiplicity of a conjugate point](#multiplicity-of-a-conjugate-point)
    - [Nonpositive sectional curvature excludes conjugate points](#nonpositive-sectional-curvature-excludes-conjugate-points)
  - [Wirtinger inequality](#wirtinger-inequality)
    - [Minimum Dirichlet energy at fixed L2 norm on an interval](#minimum-dirichlet-energy-at-fixed-l2-norm-on-an-interval)
    - [Periodic Wirtinger inequality](#periodic-wirtinger-inequality)

## Log-cosh energy on a Sobolev space

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

The inequalities $0\le\log\cosh t\le t^2/2$ make this energy finite on $H^1$. Since the second [derivative](calculus.md#derivative) of its [scalar](vector-space.md#scalar) potential is $\operatorname{sech}^2t\in(0,1]$, its [Fréchet derivative](multivariable-calculus.md#frechet-derivative) is $DI(v)[h]=\int(\nabla v\cdot\nabla h+\tanh(v)h)$, with [Taylor remainder](calculus.md#taylor-remainder) between zero and half the squared $H^1$ [norm](normed-vector-space.md#norm) of $h$. The [derivative](calculus.md#derivative) operator is strictly monotone because the [hyperbolic tangent](calculus.md#hyperbolic-tangent) is strictly increasing.

## Weierstrass excess function

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

This excess measures the height of the slope-dependent integrand above its tangent line at the reference slope $p$, evaluated at a trial slope $q$. A [convex function](real-analysis.md#convex-function) of slope has nonnegative excess. At a smooth strong local minimizer, localized needle variations force nonnegative excess along the minimizing curve for every trial slope. It detects fast-gradient competitors that the [second variation](#second-variation) around a fixed derivative can miss.

### Weierstrass necessary condition

↑ **Parent:** [Weierstrass excess function](#weierstrass-excess-function)

At a [strong local minimizer of a variational integral](#strong-local-minimizer-of-a-variational-integral), almost every reference slope $u'(x)$ is a [point of convexity](real-analysis.md#point-of-convexity) of $v\mapsto f(x,u(x),v)$. Equivalently its [Weierstrass excess function](#weierstrass-excess-function) is nonnegative for every trial slope. Uniformly small variations can have large derivatives, which is why this condition tests all trial slopes rather than only nearby ones. It is a necessary condition along the minimizing curve; the [strengthened Weierstrass condition](#strengthened-weierstrass-condition) additionally controls a neighborhood of that curve and its slopes.

#### Bounded slope integrands force strong minima to be global

↑ **Parent:** [Weierstrass necessary condition](#weierstrass-necessary-condition)

Suppose the [Weierstrass necessary condition](#weierstrass-necessary-condition) applies to a strong local minimum of this fixed-endpoint integral. It requires the tangent to $g$ at $u'(x)$ to lie below the entire graph for almost every $x$. A line of nonzero slope is unbounded above in one direction, while $g$ is bounded; hence this supporting line has slope zero. Its contact value is then a [global minimum](analysis.md#global-minimum) of $g$. The resulting [function](function.md) minimizes the integral globally, since its integrand is almost everywhere equal to the global lower bound. Thus for a bounded differentiable slope-only integrand a strong local minimum can exist only at global energy level. Weak local minima can behave differently because their competitors have nearby derivatives.

### Strengthened Weierstrass condition

↑ **Parent:** [Weierstrass excess function](#weierstrass-excess-function)

For a $C^1$ curve $u$, some $\delta>0$ must make the [Weierstrass excess function](#weierstrass-excess-function) nonnegative for every $x\in[a,b]$, every trial slope $q\in\mathbb R$, and all $y,p$ satisfying $|y-u(x)|<\delta$, $|p-u'(x)|<\delta$. Thus the supporting-line property persists in a tube of nearby heights and reference slopes. The term “strengthened” here refers to this neighborhood requirement; strict excess for $q\ne p$ is a further condition.

#### Weierstrass sufficient condition

↑ **Parent:** [Strengthened Weierstrass condition](#strengthened-weierstrass-condition)

Under the usual $C^2$ integrand regularity, an admissible $C^1$ curve satisfying the weak [Euler-Lagrange equation](analysis.md#euler-lagrange-equation), a coercively positive [second variation](#second-variation), and the [strengthened Weierstrass condition](#strengthened-weierstrass-condition) is a [strong local minimizer of a variational integral](#strong-local-minimizer-of-a-variational-integral). Strict excess away from the reference slope gives strict minimality. Coercive positivity means $\delta^2I(u)[\eta,\eta]\geq c\|\eta\|_{W^{1,2}}^2$ for every zero-trace variation and some $c>0$.

The [second variation](#second-variation) provides a neighboring field of extremals with slope $p(x,y)$. The associated endpoint-invariant Hilbert integral yields $I(v)-I(u)=\int E(x,v,p(x,v),v')\,dx$ for uniformly close admissible $v$. The tube condition makes this integral nonnegative even when $v'$ is large, explaining the passage from weak to strong minimality.

## Strong local minimizer of a variational integral

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

For a fixed-endpoint variational integral, an admissible function $u$ is a strong local minimizer if $I(v)\geq I(u)$ for all admissible $v$ whose [uniform norm](normed-vector-space.md#supremum-norm) distance from $u$ is sufficiently small. Derivatives can be far apart. Hence strong local minimality implies [weak local minimality](#weak-local-minimizer-of-a-variational-integral), while a global minimizer implies both. Small narrow bumps and rapid low-amplitude oscillations explain why the reverse implication can fail.

### Coercivity transfers strong minimality to L1 minimality

↑ **Parent:** [Strong local minimizer of a variational integral](#strong-local-minimizer-of-a-variational-integral)

With fixed endpoint values on a finite interval, the displayed [derivative](calculus.md#derivative) [coercivity](real-analysis.md#coercive-function) makes a finite-energy [strong local minimizer of a variational integral](#strong-local-minimizer-of-a-variational-integral) also a local minimizer in $L^1$. Otherwise choose better competitors converging in $L^1$. The upper energy bound controls their derivatives in $L^p$, and a common endpoint controls their function norms. Compact [Sobolev embedding](sobolev-space.md#failure-of-first-order-sobolev-embedding-into-linfinity-in-two-dimensions) gives a uniformly convergent subsequence; its limit is the $L^1$ limit. This contradicts strong local minimality. [Convexity](real-analysis.md#convex-function) of the integrand is unnecessary for this neighborhood-transfer argument.

## Weak local minimizer of a variational integral

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

For a fixed-endpoint integral on $W^{1,\infty}(a,b)$, an admissible function $u$ is a weak local minimizer if $I(v)\geq I(u)$ whenever the [Sobolev norm](sobolev-space.md#sobolev-norm) $\|v-u\|_{W^{1,\infty}}$ is sufficiently small. Both function and derivative must be close. “Weak” here labels the variational neighborhood convention, not the [weak topology](weak-topology.md) of a [Banach space](banach-space.md).

### Periodic slopes give weak minima without strong minima

↑ **Parent:** [Weak local minimizer of a variational integral](#weak-local-minimizer-of-a-variational-integral)

For $0<\delta<1$, choose the zero-trace piecewise affine curve with slope $\delta$ up to $1-\delta/4$ and slope $\delta-4$ thereafter. Periodicity makes $g'$ equal to the same nonzero constant at both slopes, and $g''>0$ on small neighborhoods of both. For sufficiently small Lipschitz perturbations, local [strict convexity](real-analysis.md#strictly-convex-function) bounds the energy difference below by $c\int\phi'^2$, since the common first-variation coefficient multiplies $\int\phi'=0$. This proves a strict weak minimum. The global supporting-tangent condition fails because its nonzero slope cannot stay below bounded $g$, so it is not a strong minimum. By contrast, tents of slopes $4n,-4n$ attain $g=-1$ everywhere and provide infinitely many distinct global minimizers.

## Length extremals from a constant quadratic energy

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

For an autonomous smooth [Lagrangian](#lagrangian) homogeneous of degree two in velocities, the [Beltrami identity](analysis.md#beltrami-identity) gives $\dot q\cdot L_{\dot q}-L=L$ constant on its [Euler-Lagrange](analysis.md#euler-lagrange-equation) extremals. On a regular segment with this constant positive, the Euler-Lagrange expression for $\sqrt L$ equals that for $L$ divided by $2\sqrt L$, since the extra term is proportional to $\dot L$. Hence an energy extremal has the same path as a length extremal. Length is invariant under regular reparametrization: in two coordinates, on a graph $v=v(u)$, its density is $\sqrt{E+2Fv_u+Gv_u^2}\,|du|$. If a nonnegative semidefinite energy vanishes along a curve, the curve instead minimizes length at zero; division by $\sqrt L$ is not permitted there. For a positive definite metric, regular nonconstant curves have positive energy.

## Euler-Lagrange equation for a second-derivative functional

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

For a sufficiently smooth [functional](#functional) $I[y]=\int_a^b F(x,y,y',y'')\,dx$, the [first variation](#first-variation) in direction $\eta$ is $\int(F_y\eta+F_{y'}\eta'+F_{y''}\eta'')dx$. Twice applying [integration by parts](calculus.md#integration-by-parts) gives the interior coefficient $F_y-(F_{y'})'+(F_{y''})''$ and boundary expression $[(F_{y'}-(F_{y''})')\eta+F_{y''}\eta']_a^b$. Variations supported in the interior and the [fundamental lemma of the calculus of variations](#fundamental-lemma-of-the-calculus-of-variations) force the displayed equation. The remaining boundary terms give the [natural boundary conditions for second-derivative functionals](#natural-boundary-conditions-for-second-derivative-functionals).

### Clamped fourth-order variational extremal on a quarter period

↑ **Parent:** [Euler-Lagrange equation for a second-derivative functional](#euler-lagrange-equation-for-a-second-derivative-functional)

With values $y(0)=y(\pi/2)=y'(\pi/2)=0$ and $y'(0)=1$, the [higher-order Euler-Lagrange equation](analysis.md#higher-order-euler-lagrange-equation) is $y^{(4)}-y=0$. Write $c=\cosh(\pi/2)$ and $s=\sinh(\pi/2)$. Solving the four linear boundary equations gives $y=[c(\cos x-\cosh x)+(1-s)\sin x+(1+s)\sinh x]/2$. The added function $x^2$ does not affect the [first variation](#first-variation).

### Beltrami identity for a second-derivative functional

↑ **Parent:** [Euler-Lagrange equation for a second-derivative functional](#euler-lagrange-equation-for-a-second-derivative-functional)

For a smooth [functional](#functional) $\int F(x,y,y',y'')\,dx$, let $P=F_{y'}$ and $Q=F_{y''}$. Along an [extremal](#extremal), the [Euler-Lagrange equation for a second-derivative functional](#euler-lagrange-equation-for-a-second-derivative-functional) is $F_y-P'+Q''=0$. Differentiating $H=y''Q+y'(P-Q')-F$ by the [chain rule](calculus.md#chain-rule) gives

$$
H'=y'(P'-Q''-F_y)-F_x=-F_x.
$$

Consequently $H$ is constant whenever $F$ has no explicit dependence on $x$. This extends the [Beltrami identity](analysis.md#beltrami-identity) to a second-derivative variational problem. If $F$ is independent of $y''$, the expression reduces to $y'F_{y'}-F$.

### Natural boundary conditions for second-derivative functionals

↑ **Parent:** [Euler-Lagrange equation for a second-derivative functional](#euler-lagrange-equation-for-a-second-derivative-functional)

At an endpoint of a second-derivative variational problem, a free value $y$ gives the first displayed condition, while a free slope $y'$ gives the second. Each condition is required only when its corresponding endpoint variation is free; a prescribed value or slope instead forces that variation to vanish. For $F=K(y'')^2/2+qy$, the two conditions become $y'''=0$ and $y''=0$, respectively. A clamped beam has both value and slope fixed, a pinned beam fixes value but leaves slope free, and a free end leaves both free.

## Extremal

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

A sufficiently regular admissible [function](function.md) at which the [first variation](#first-variation) of a [functional](#functional) vanishes for every permitted [variation](#variation). An [extremal](#extremal) is a stationary candidate; it need not be a local maximum or minimum. For a first-order integral [functional](#functional) with fixed endpoint values, it satisfies the [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) under the usual regularity assumptions.

## Variational principle

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

A variational principle specifies a [function](function.md), path or field by requiring a [functional](#functional) to be stationary under an allowed class of [variations](#variation). The admissible class includes the prescribed [boundary conditions](differential-equation.md#boundary-condition) and [constraints](classical-mechanics.md#constraint-mechanics). A stationary value need not be a [minimum](set.md#minimum-of-a-subset-of-a-total-order): the [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) expresses the first-order stationarity condition, while a minimum requires additional analysis. [Fermat principle](mathematical-physics.md#fermat-principle) applies this idea to optical path length, and the [Rayleigh-Ritz method](finite-element-method.md#rayleigh-ritz-method) approximates a variational problem in a chosen family of [trial functions](finite-element-method.md#trial-function).

### Variational projection onto an involutive symmetry

↑ **Parent:** [Variational principle](#variational-principle)

Let $H$ be a lower-bounded self-adjoint [Hamiltonian operator](quantum-system.md#hamiltonian-quantum-mechanics) and $I$ a commuting self-adjoint operator with $I^2=1$. For a normalized trial vector $\phi$, define $a=\langle H\rangle_\phi$, $b=\langle I\rangle_\phi$, $c=\langle HI\rangle_\phi$. The [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient) on $\phi+tI\phi$ is $[(1+t^2)a+2tc]/[1+t^2+2tb]$, with derivative $2(c-ab)(1-t^2)/(1+t^2+2tb)^2$. Unless $c=ab$, its extrema are the normalized nonzero vectors $\phi\pm I\phi$, with energies $(a\pm c)/(1\pm b)$. Their difference is $2(c-ab)/(1-b^2)$, identifying the maximum and minimum.

The orthogonal projections $(1\pm I)/2$ split any trial energy into a weighted mean of the two sector energies, so one nonzero sector projection never raises the trial energy. If $|b|=1$, one projected vector is zero and its quotient is undefined; the remaining family has constant energy. Exchange symmetry makes these sectors bosonic and fermionic spatial wavefunctions. Stationarity within this two-dimensional trial space does not generally make a vector an exact eigenvector of $H$.

## Quadratic minor null Lagrangian

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

For constant $K$, this quadratic combination of two-by-two gradient minors is a [divergence](multivariable-calculus.md#divergence). Indeed,

$$
K_{k\gamma}\epsilon_{\alpha\beta\gamma}\epsilon_{ijk}\overline{u_{i,\alpha}}u_{j,\beta}=\partial_\alpha\left(K_{k\gamma}\epsilon_{\alpha\beta\gamma}\epsilon_{ijk}\overline{u_i}u_{j,\beta}\right),
$$

because the term containing $u_{j,\beta\alpha}$ vanishes by antisymmetry of the [Levi-Civita symbol](multivariable-calculus.md#levi-civita-symbol). Its volume integral vanishes for homogeneous displacement boundary data. It also vanishes pointwise on [rank-one matrices](vector-space.md#rank-one-matrix), since $\nu_\alpha\nu_\beta$ is symmetric. Consequently one can strengthen an elastic energy density by such a term without changing fixed-boundary incremental energies or [acoustic tensors](elasticity-physics.md#acoustic-tensor).

## Brachistochrone problem

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

The brachistochrone problem asks for the curve along which a particle released from rest reaches a specified target fastest under a uniform gravitational field, without friction. With downward depth $u$, conservation of energy gives speed $\sqrt{2gu}$ and travel time $\int\sqrt{(1+u'^2)/(2gu)}\,dx$. The [Beltrami identity](analysis.md#beltrami-identity) makes $u(1+u'^2)$ constant, leading to a [cycloid](topology.md#cycloid). If only the horizontal endpoint coordinate $x_0>0$ is fixed, the [natural boundary conditions for a free endpoint](analysis.md#natural-boundary-conditions-for-a-free-endpoint) select the half arch ending at its deepest point, with depth $2x_0/\pi$ and minimum time $\sqrt{\pi x_0/g}$.

### Fixed-length brachistochrone between equal-height endpoints

↑ **Parent:** [Brachistochrone problem](#brachistochrone-problem)

For horizontal separation one, let $y>0$ be downward depth and constrain the [arc length](riemannian-geometry.md#arc-length) to $L$. [Conservation of energy](mathematical-physics.md#conservation-of-energy) makes the [travel time](dispersion-relation.md#travel-time) proportional to $\int\sqrt{1+y'^2}/\sqrt y\,dx$. An [isoperimetric constraint](analysis.md#isoperimetric-constraint) adds a [Lagrange multiplier](mathematical-optimization.md#lagrange-multiplier) $\lambda$, and the [Beltrami identity](analysis.md#beltrami-identity) gives $(y^{-1/2}+\lambda)/\sqrt{1+y'^2}=H>0$. With $b=\lambda/H$, $c=H^2$ and $s=\sin(\phi/2)$, the stationary arch is $y=s^2/[c(1-bs)^2]$, $dx/d\phi=s^2/[c(1-bs)^3]$, for $0\le\phi\le2\pi$. The endpoint and length integrals fix $b,c$ uniquely for $L>1$; symmetry gives $x(2\pi-\phi)=1-x(\phi)$. At $L=1$ the only curve is horizontal and a particle released from rest never completes the journey. The finite-time stationary arches have vertical endpoint tangents, so the graph is smooth only on the open interval. These first-variation equations alone do not establish global minimality in a larger admissible class.

### Brachistochrone on a hemispherical ramp

↑ **Parent:** [Brachistochrone problem](#brachistochrone-problem)

Measure polar angle $\theta$ from the downward vertical on the lower hemisphere of radius $R$. A particle released from rest at the rim and sliding without energy loss has speed $\sqrt{2gR\cos\theta}$. The spherical [arc length](riemannian-geometry.md#arc-length) along $\phi=\phi(\theta)$ is $R\sqrt{1+\sin^2\theta\,\phi'^2}|d\theta|$. Thus its [travel time](dispersion-relation.md#travel-time) has integrand proportional to $\sqrt{(1+\sin^2\theta\,\phi'^2)/\cos\theta}$. Since the azimuth is a [cyclic coordinate](lagrangian-mechanics.md#cyclic-coordinate), the [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) gives

$$
\frac{\sin^2\theta\,\phi'}{\sqrt{\cos\theta}\sqrt{1+\sin^2\theta\,\phi'^2}}=C.
$$

Solving for $\phi'^2$ gives the displayed [first integral](differential-equation.md#first-integral) on a segment where $\theta$ is a valid path parameter. For finite $C$, approaching the rim $\theta\uparrow\pi/2$ gives $\phi'\to0$. Thus a regular stationary path begins along the meridian toward the bottom. This is an initial direction condition; a path joining other rim points can turn before reaching the bottom. Monotone segments use positive $|d\theta|$ in the time integral, and a turning point requires another path parameter or a split into segments.

### Maximum-depth bound for a brachistochrone

↑ **Parent:** [Brachistochrone problem](#brachistochrone-problem)

Consider a frictionless track from rest between equal-height endpoints separated horizontally by $l>0$. Let depth $y$ be positive downward and let the maximum depth be $h>0$. [Conservation of energy](mathematical-physics.md#conservation-of-energy) gives speed $\sqrt{2gy}$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality), applied to the tangent displacement, gives

$$
\frac{ds}{\sqrt y}\geq\frac{dx}{\sqrt h}+\sqrt{\frac{h-y}{hy}}\,|dy|.
$$

The squared norm of the coefficient vector is $1/h+(h-y)/(hy)=1/y$. The track goes from depth zero to $h$ and returns to zero, so the second term integrates to at least $2\int_0^h\sqrt{(h-y)/(hy)}dy=\pi\sqrt h$. Integrating the first term gives $l/\sqrt h$, even if the track backtracks horizontally. Division by $\sqrt{2g}$ proves the first bound. The [arithmetic-geometric mean inequality](mathematical-optimization.md#arithmetic-geometric-mean-inequality) proves the second.

Equality requires $h=l/\pi$ and tangent slope $|dy/dx|=\sqrt{(h-y)/y}$, on the descending and ascending halves respectively. Substitution $y=h\sin^2\theta$ integrates to the [cycloid](topology.md#cycloid) $x=h(\theta-\frac12\sin2\theta)$, $0\leq\theta\leq\pi$. It attains the bound, proving global minimality of the single-arch [brachistochrone problem](#brachistochrone-problem) between these endpoints. Endpoint singularities are handled as limits of the integrals; the cycloid has finite travel time.

### Brachistochrone on a horizontal half-cylinder

↑ **Parent:** [Brachistochrone problem](#brachistochrone-problem)

Measure $\theta\in[-\pi/2,\pi/2]$ from the vertically downward direction on the lower half of a cylinder of radius $R$, and let $z$ be axial distance. From rest at an edge, [conservation of energy](mathematical-physics.md#conservation-of-energy) gives speed $\sqrt{2gR\cos\theta}$. The [travel time](dispersion-relation.md#travel-time) is $T=(2gR)^{-1/2}\int\sqrt{R^2+z'^2}/\sqrt{\cos\theta}\,d\theta$. Since $z$ is a [cyclic coordinate](lagrangian-mechanics.md#cyclic-coordinate), its conjugate quantity $z'/[\sqrt{\cos\theta}\sqrt{R^2+z'^2}]=K$ is constant, giving the displayed formula. For finite positive axial separation, $0<K<1$ is fixed uniquely by integrating $z'$ between the edges: the separation grows strictly from zero to infinity as $K$ increases from zero to one. The time integrand is strictly convex in $z'$, so its supporting-line inequality proves global minimality for the fixed endpoints. As the starting edge is approached, $z'\to0$: the initial direction is directly down the curved surface, with no axial component. This differs from the constant-pitch shortest [geodesic](riemannian-geometry.md#geodesic) on the unrolled cylinder.

## Travel-time minimization with speed proportional to squared radius

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

For speed $v=kr^2$ in the punctured plane, the travel-time element is $ds/(kr^2)$. Under the [inversion in a circle](group-theory.md#inversion-in-a-circle) with radial coordinate $u=1/r$, this becomes $k^{-1}\sqrt{du^2+u^2d\theta^2}$, the [arc length](riemannian-geometry.md#arc-length) in [Euclidean space](normed-vector-space.md#euclidean-norm) divided by $k$. Thus a shortest travel-time route corresponds to a straight [line segment](convex-set.md#line-segment) in the inverted plane, whenever that segment avoids the origin and lies in the allowed region. Between $(a,0)$ and $(0,a)$ the inverted segment has equation $u(\cos\theta+\sin\theta)=1/a$. The route is $r=a(\cos\theta+\sin\theta)$, and its minimum travel time is $\sqrt2/(ka)$. The [triangle inequality](topological-analysis.md#triangle-inequality) for [arc length](riemannian-geometry.md#arc-length) proves global minimality.

## Gamma-convergence

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

A sequence of functionals Gamma-converges in a specified [topology](topology.md) when every convergent $u_n\to u$ satisfies $F(u)\le\liminf_nF_n(u_n)$, and each $u$ has a recovery sequence $u_n\to u$ with $F_n(u_n)\to F(u)$. With appropriate compactness of energy sublevels, limits of approximate global [minimizers](analysis.md#global-minimizer) minimize $F$, and the minimum values converge. This is suited to variational approximation such as the [Ambrosio–Tortorelli approximation](computer-science.md#ambrosio-tortorelli-approximation); it does not describe arbitrary local minima.

## Variational problem

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)

A variational problem seeks a stationary point or minimizer of a [functional](#functional) on a specified [function space](functional-analysis.md#function-space). For a symmetric [coercive bilinear form](bilinear-form.md#coercive-bilinear-form) $a$ and bounded [linear functional](dual-space.md#linear-functional) $\ell$ on a real [Hilbert space](hilbert-space.md), minimizing $J(v)=a(v,v)/2-\ell(v)$ is equivalent to the [weak formulation](partial-differential-equation.md#weak-formulation) $a(u,v)=\ell(v)$ for every test vector. The [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem) gives a unique solution, and $J(u+w)-J(u)=a(w,w)/2$ proves unique minimization. Specifying the admissible space and its boundary constraints is part of the problem.

## Direct method in the calculus of variations

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Direct_method_in_the_calculus_of_variations)

The direct method takes a minimizing sequence, extracts a subsequence using compactness, and uses lower semicontinuity to show that its limit attains the infimum.

### Lavrentiev phenomenon

↑ **Parent:** [Direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations)

A Lavrentiev gap is a strict change in an [infimum](real-analysis.md#infimum) when the admissible regularity class is restricted, despite retaining the same endpoint values. For example $I(u)=\int_0^1(u^3-x)^2u'^6dx$ with $u(0)=0,u(1)=1$ has value zero at the absolutely continuous function $u=x^{1/3}$. Every Lipschitz competitor has a uniform positive lower energy bound. Indeed its ratio to $x^{1/3}$ starts at zero, so let $x_0$ be its first crossing of $u(x)=x^{1/3}/2$. Before that point, $|u^3-x|\geq7x/8$. [Holder inequality](functional-analysis.md#holder-inequality) gives

$$
\left(\frac{x_0^{1/3}}2\right)^6\leq\left(\int_0^{x_0}x^2|u'|^6dx\right)\left(\frac53x_0^{3/5}\right)^5.
$$

Thus $I(u)\geq(49/4096)(3/5)^5/x_0\geq(49/4096)(3/5)^5>0$. This proves a gap directly. The example's integrand lacks a uniform superlinear lower bound along its zero set; it illustrates the admissible-class issue rather than by itself furnishing a counterexample under stronger coercivity assumptions.

### Power-law comparison for vanishing derivative regularization

↑ **Parent:** [Direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations)

For $I_\varepsilon(u)=\int_0^1[(u^4-x)^2+\varepsilon|u'|^{4/3}]dx$ with endpoint values zero and one, the zero-penalty minimizer $x^{1/4}$ has infinite [derivative](calculus.md#derivative) penalty. Use $u=x^{1/4+\delta}$ instead. The mismatch is at most $(32/27)\delta^2$, while the [derivative](calculus.md#derivative) penalty is $(3\varepsilon/(4\delta))(1/4+\delta)^{4/3}$. Balancing $\delta^2$ and $\varepsilon/\delta$ by $\delta=\varepsilon^{1/3}$ gives an upper energy bound of order $\varepsilon^{2/3}$. Nonnegativity then proves convergence of minimum energies to zero. This is a recovery construction; no claim of a matching lower asymptotic constant is needed.

### Tonelli existence theorem

↑ **Parent:** [Direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations)

For a scalar fixed-endpoint problem on a bounded interval, suppose the continuous integrand $f(x,y,p)$ is convex in $p$ and satisfies $f(x,y,p)\geq\Theta(|p|)-C$, where $\Theta$ is nonnegative convex and $\Theta(r)/r\to\infty$. If there is one admissible absolutely continuous function of finite energy, a global minimizer exists in $W^{1,1}$.

The lower bound gives uniform integrability of derivatives in a minimizing sequence. Fixed endpoint values then give boundedness and equicontinuity of the functions. Extract uniform convergence of the functions and weak $L^1$ convergence of their derivatives; the limit retains the endpoint values. Convexity in the derivative gives [weak lower semicontinuity of convex gradient energies](#weak-lower-semicontinuity-of-convex-gradient-energies), so the limit attains the infimum. Strict convexity of the full integrand on a convex admissible class additionally gives uniqueness.

### Weak lower semicontinuity of convex gradient energies

↑ **Parent:** [Direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations)

Suppose the domain has finite measure and $F\in C^1$ is convex, with $|F(p)|\leq C(1+|p|^2)$ and $|DF(p)|\leq C(1+|p|)$. The supporting inequality $F(p)\geq F(q)+DF(q)\cdot(p-q)$, integrated with $q=Du$, gives $\int F(Du_k)\geq\int F(Du)+\int DF(Du)\cdot(Du_k-Du)$. The last term tends to zero by weak convergence of the gradients and the fixed $L^2$ test field $DF(Du)$. This proves weak lower semicontinuity without requiring pointwise convergence of gradients.

### Symmetric elliptic Dirichlet energy with a nonpositive potential

↑ **Parent:** [Direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations)

For a bounded domain, bounded symmetric uniformly elliptic $A$, $q\leq0$, and $f\in L^2$, minimizing $J$ on $\psi+H_0^1$ solves $\operatorname{div}(A\nabla u)+qu=f$. The nonnegative quadratic terms are weakly lower semicontinuous, and [Poincaré inequality](sobolev-space.md#poincare-inequality) makes the gradient norm coercive on the zero-boundary part. The first variation gives the weak equation with the forcing sign displayed above. If $q$ is positive, coercivity may fail at a Dirichlet eigenvalue; orthogonality to the homogeneous kernel is then needed for solvability.

### Screened sine-Gordon energy

↑ **Parent:** [Direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations)

For real $f\in L^2(\mathbb R^3)$, this [energy functional](#energy-functional) on $H^1(\mathbb R^3)$ is coercive and attains its minimum by the [direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations). The nonnegative potential term is weakly lower semicontinuous by [local Sobolev compactness gives lower semicontinuity of a nonnegative integral](functional-analysis.md#local-sobolev-compactness-gives-lower-semicontinuity-of-a-nonnegative-integral). Its [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) is $-\Delta u+u+\sin u=f$ in the [weak solution](partial-differential-equation.md#weak-solution) sense. The extra linear restoring term screens the [Sine-Gordon equation](integrable-systems.md#sine-gordon-equation) nonlinearity. The scalar potential $V(s)=s^2/2+1-\cos s$ is convex because $V''(s)=1+\cos s\geq0$; hence any weak critical point is a minimizer. The [elliptic regularity](distribution-theory.md#elliptic-regularity) estimate for $-\Delta+1$, together with $|\sin u|\leq|u|$, gives $u\in H^2$. The [Sobolev inequality](sobolev-space.md#sobolev-inequality) then puts $u$ in $W^{1,6}$, so [Morrey's inequality](sobolev-space.md#morrey-s-inequality) and [uniformly continuous integrable functions vanish at infinity](topological-analysis.md#uniformly-continuous-integrable-functions-vanish-at-infinity) give a continuous representative tending to zero.

#### Failure of the source-size bound for the screened sine-Gordon equation

↑ **Parent:** [Screened sine-Gordon energy](#screened-sine-gordon-energy)

Take $a=3\pi/2$, $L=10$ and $u(x)=a\exp(-|x|^2/L^2)$ on $\mathbb R^3$. Set $f=-\Delta u+u+\sin u$. Both functions are smooth and belong to [L2 space](measure-theory.md#l2-space-is-a-hilbert-space), and $u\in H^1$. The strictly increasing reaction $h(s)=s+\sin s$ has $0\leq h(u)\leq h(a)=a-1$, while

$$
|\Delta u|=\frac{a}{L^2}|4q-6|e^{-q}\leq\frac{6a}{L^2},\qquad q=|x|^2/L^2.
$$

Consequently $\|f\|_\infty\leq a-1+6a/L^2<a=\|u\|_\infty$. This $u$ is a minimizer of the [screened sine-Gordon energy](#screened-sine-gordon-energy): it solves the [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) and that energy is convex. Thus even the minimizing and smooth hypotheses do not justify the stronger source-size bound. The appropriate general estimate is [maximum bound for a monotone reaction term](elliptic-boundary-value-problem.md#maximum-bound-for-a-monotone-reaction-term).

### Minimizing sequence

↑ **Parent:** [Direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations)

A [minimizing sequence](#minimizing-sequence) satisfies $E(u_n)\to\inf E$. [Coercivity](real-analysis.md#coercive-function) bounds an appropriate [sublevel set](calculus.md#sublevel-set), [Compactness](topology.md#compact-space) supplies a [convergent subsequence](real-analysis.md#convergent-subsequence), and [sequential lower semicontinuity](calculus.md#sequential-lower-semicontinuity) turns its limit into a [global minimizer](analysis.md#global-minimizer).

#### Oscillating minimizing sequence with no minimizer

↑ **Parent:** [Minimizing sequence](#minimizing-sequence)

A [minimizing sequence](#minimizing-sequence) can converge uniformly while its [derivatives](calculus.md#derivative) keep oscillating between distinct energy wells. For the [functional](#functional) $I(u)=\int_0^1[u^4+(u'^4-16)^4]$, with zero endpoint values and [Lipschitz](real-analysis.md#lipschitz-continuity) admissible functions, the triangular waves displayed above have slopes $\pm2$ [almost everywhere](measure-theory.md#almost-everywhere) and height $1/N$. Direct integration gives $I(u_N)=1/(5N^4)$. Nonnegativity therefore makes the [infimum](real-analysis.md#infimum) zero. Attainment would require both $u=0$ and $|u'|=2$ [almost everywhere](measure-theory.md#almost-everywhere), an impossibility. The uniform limit is zero but its energy is $16^4$; thus the energy fails to be [lower semicontinuous](calculus.md#lower-semicontinuity) for this convergence. The example explains why control of [function](function.md) values alone cannot replace suitable [convexity](real-analysis.md#convex-function) in the [derivative](calculus.md#derivative) variable in the [direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations).

### Bounded slope condition

↑ **Parent:** [Direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations)

Boundary data $g$ satisfy the bounded slope condition with constant $K$ when every boundary point admits affine lower and upper supporting functions of Lipschitz constant at most $K$. Comparison with these barriers gives a global Lipschitz bound for convex variational problems.

### Comparison principle for convex variational integrals

↑ **Parent:** [Direct method in the calculus of variations](#direct-method-in-the-calculus-of-variations)

For suitable convex integral functionals, ordered boundary values of two minimizers imply the same ordering in the domain. Affine minimizers can therefore serve as upper and lower barriers.

## Functional

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Functional_(mathematics))

A functional is a [function](function.md) whose inputs are themselves functions, curves, or other elements of a function space.

### Quadratic functional

↑ **Parent:** [Functional](#functional)

A quadratic functional on a real vector space combines a [quadratic form](quadratic-form.md) $B(v,v)$, a [linear functional](dual-space.md#linear-functional) $\ell(v)$ and a constant. If $B$ is a symmetric [bounded bilinear form](bilinear-form.md#bounded-bilinear-form), its [first variation](#first-variation) is $DI(v)[w]=2B(v,w)-2\ell(w)$. For a strictly positive $B$, an existing stationary point is the unique minimizer by the [quadratic variational principle for a symmetric positive operator](hilbert-space.md#quadratic-variational-principle-for-a-symmetric-positive-operator).

#### Resonant sine modes of a quadratic variational integral

↑ **Parent:** [Quadratic functional](#quadratic-functional)

The [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) is $y''+ky=0$. For positive $k$ a nonzero stationary [function](function.md) exists exactly when $\sqrt k$ is a positive integer $n$, and all such [functions](function.md) are $B\sin(nx)$. These values are the [Dirichlet eigenvalues](sturm-liouville-theory.md#dirichlet-eigenvalue) of $-d^2/dx^2$ on the interval. At $k=0$ the solutions are affine and the endpoint conditions leave only zero; negative $k$ likewise leaves only zero. Stationarity alone does not assert minimization of the [quadratic functional](#quadratic-functional).

#### Stationary values of a quadratic functional with a quadratic constraint

↑ **Parent:** [Quadratic functional](#quadratic-functional)

Impose zero [Dirichlet boundary conditions](differential-equation.md#dirichlet-boundary-condition) on an interval. The [isoperimetric constraint](analysis.md#isoperimetric-constraint) $I[y]=1$ is regular because $DI_y[y]=2I[y]=2\ne0$. The [Lagrange multiplier](mathematical-optimization.md#lagrange-multiplier) rule applied to $J-\lambda(I-1)$ gives the [Sturm-Liouville equation](sturm-liouville-theory.md#sturm-liouville-equation)

$$
(py')'+qy+\lambda wy=0.
$$

Multiplying by $y$ and using [integration by parts](calculus.md#integration-by-parts) gives $J[y]=\lambda I[y]=\lambda$. Thus the multiplier is the stationary value of the original functional, or its [Rayleigh quotient](linear-operator-theory.md#rayleigh-quotient). This calculation does not require $w$ to have one sign; positive-weight spectral conclusions require additional hypotheses.

If two stationary functions have different multipliers, multiplying their equations crosswise and subtracting gives $(\lambda_n-\lambda_m)\int wy_ny_m=0$. The endpoint terms vanish. This proves the weighted [orthogonality of Sturm-Liouville eigenfunctions](sturm-liouville-theory.md#orthogonality-of-sturm-liouville-eigenfunctions). Higher stationary values need not be local minima of the constrained functional.

### Epigraph

↑ **Parent:** [Functional](#functional)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Epigraph_(mathematics))

The [epigraph](#epigraph) is $\{(u,t):E(u)\leq t\}$. It is a [convex set](convex-set.md) exactly when $E$ is a [convex function](real-analysis.md#convex-function), and is a [sequentially closed set](topology.md#sequentially-closed-set) in the [product topology](geometry-and-topology.md#product-topology) exactly when $E$ is [sequentially lower semicontinuous](calculus.md#sequential-lower-semicontinuity).

### Functional derivative

↑ **Parent:** [Functional](#functional)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Functional_derivative)

The functional derivative is defined by the first variation

$$
F[\phi+\epsilon h]-F[\phi]
=\epsilon\int\frac{\delta F}{\delta\phi(x)}h(x),dx+o(\epsilon).
$$

#### Functional Taylor expansion

↑ **Parent:** [Functional derivative](#functional-derivative)

The first variation of a differentiable [action functional](lagrangian-mechanics.md#action) gives its change under a small field deformation. With $E=\delta S/\delta\phi$, the change $\phi\mapsto\phi-\eta f$ generates $-\eta\int fE$ to first order. This is the basic cancellation behind the [equivalence theorem for field redefinitions](perturbative-quantum-field-theory.md#equivalence-theorem-for-field-redefinitions); the [functional Jacobian](quantum-field-theory.md#functional-jacobian) and transformed operator insertions must also be treated consistently.

#### Functional chain rule

↑ **Parent:** [Functional derivative](#functional-derivative)

Along a differentiable path of fields $\phi(x,t)$, a differentiable functional obeys

$$
\frac{d}{dt}F[\phi(t)]
=\int dx\,
\frac{\delta F}{\delta\phi(x)}\,
\partial_t\phi(x,t).
$$

Integrating in time expresses the functional change as the line integral of its functional derivative along the path.

### Energy functional

↑ **Parent:** [Functional](#functional)

An energy functional assigns an integral energy to a function. Minimization of a suitable energy is the basis of the [Dirichlet principle](#dirichlet-principle). For the modified Helmholtz equation, a natural example is

$$
E[u]=\int_V\left(|\nabla u|^2+m^2u^2\right)dV.
$$

#### Critical point of an energy functional

↑ **Parent:** [Energy functional](#energy-functional)

A field configuration is critical for an [energy functional](#energy-functional) $E$ if its [first variation](#first-variation) vanishes for every admissible infinitesimal field variation. For $E[\phi]=\int(\tfrac12|\nabla\phi|^2+U(\phi))$, integration by parts against compactly supported variations gives $\delta E=\int(-\Delta\phi+U'(\phi))\delta\phi$, so [stationary field configurations](#critical-point-of-an-energy-functional) satisfy the [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) $\Delta\phi=U'(\phi)$. A constrained target instead allows only tangent variations, changing that field equation. Criticality is stationarity, not necessarily energetic stability or a local minimum.

#### p-energy

↑ **Parent:** [Energy functional](#energy-functional)

The p-energy of a Sobolev function is

$$
E_p[u]=\frac1p\int_\Omega|Du|^p\,dx.
$$

Its stationary points under fixed boundary data are weak solutions of the [p-Laplacian equation](partial-differential-equation.md#p-laplacian).

### Lagrangian

↑ **Parent:** [Functional](#functional)

A Lagrangian is a function or density whose stationary integral encodes an extremization problem. In [Lagrangian mechanics](lagrangian-mechanics.md) its action gives the equations of motion; in geometry it describes geodesics and minimal surfaces.

In [Lagrangian](classical-field-theory.md#lagrangian-field-theory), the action integrates such a density over spacetime.

A finite-dimensional [optimization Lagrangian](mathematical-optimization.md#optimization-lagrangian) combines an [objective function](mathematical-optimization.md#objective-function) with [Lagrange multiplier](mathematical-optimization.md#lagrange-multiplier) terms for its constraints.

### Variation

↑ **Parent:** [Functional](#functional)

A variation of a function $y$ is a one-parameter family $y+\varepsilon\eta$, where $\eta$ satisfies the required [boundary conditions](differential-equation.md#boundary-condition).

#### First variation

↑ **Parent:** [Variation](#variation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/First_variation)

The first variation of a [functional](#functional) $L$ at $y$ in the direction $\eta$ is

$$
\delta L[y;\eta]
=\left.\frac d{d\varepsilon}L[y+\varepsilon\eta]\right|_{\varepsilon=0}.
$$

##### Fundamental lemma of the calculus of variations

↑ **Parent:** [First variation](#first-variation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fundamental_lemma_of_the_calculus_of_variations)

If a continuous function $f$ satisfies

$$
\int_a^b f(x)\eta(x)\,dx=0
$$

for every smooth compactly supported test function $\eta$, then $f=0$ on $(a,b)$.

## Stationary point

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stationary_point)

A point is stationary for a [differentiable function](analysis.md#differentiable-function) or [functional](#functional) when its first [derivative](calculus.md#derivative) or [first variation](#first-variation) vanishes in every admissible direction.

### Stationary points of a cosine-modulated Gaussian

↑ **Parent:** [Stationary point](#stationary-point)

The [gradient](multivariable-calculus.md#gradient) vanishes only when $y=0$ and $\tan x=-2x$. On each tangent branch, $\tan x+2x$ increases strictly from negative to positive infinity, so it has exactly one root $x_s$. With $z_s=e^{-x_s^2}\cos x_s$, the [Hessian matrix](multivariable-calculus.md#hessian-matrix) is diagonal with entries $-(4x_s^2+3)z_s$ and $-2z_s$. Its determinant is positive, so every stationary point is a strict maximum when $z_s>0$ or a strict minimum when $z_s<0$. Signs alternate between successive tangent branches. This gives infinitely many nondegenerate extrema under a decaying [Gaussian function](calculus.md#gaussian-function) envelope.

### Stationary points with real cube-root factors

↑ **Parent:** [Stationary point](#stationary-point)

Where $q(x)\ne0$, the [product rule](calculus.md#product-rule) and [chain rule](calculus.md#chain-rule) give the displayed real derivative. Its stationary points therefore satisfy $3q+(x-a)q'=0$. The denominator uses the square of the real [cube root](arithmetic.md#cube-root), which stays positive for negative $q$. Points with $q=0$ must be checked in the original function: a simple zero of $q$ with $x\ne a$ creates a vertical tangent, not a stationary point. If the prefactor also vanishes, a cancellation can change differentiability and must be analyzed separately.

### Stationary points under an increasing outer function

↑ **Parent:** [Stationary point](#stationary-point)

Suppose $h$ is differentiable and $F'>0$ on its range. The [multivariable chain rule](calculus.md#multivariable-chain-rule) shows that $F\circ h$ has exactly the same [stationary points](#stationary-point) as $h$. Since $F$ is strictly increasing, the type of every [local maximum](analysis.md#local-maximum), [local minimum](analysis.md#local-minimum), and [saddle point](analysis.md#saddle-point) is preserved. If both functions are twice differentiable, then at a stationary point

$$
\operatorname{Hess}(F\circ h)=F'(h)\operatorname{Hess}h,
$$

so the [Hessian matrix](multivariable-calculus.md#hessian-matrix) signature is unchanged. The hypothesis $F'>0$ matters for the converse about stationary points: a strictly increasing function such as $F(s)=s^3$ can have a zero [derivative](calculus.md#derivative) and create new stationary points in a composition.

## Dirichlet principle

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirichlet_principle)

Among functions with fixed boundary values, the solution of $\nabla\cdot(\kappa\nabla\phi)=0$ with $\kappa>0$ uniquely minimizes the weighted energy

$$
\int\kappa|\nabla\phi|^2.
$$

### Quadratic energy minimization by the parallelogram law

↑ **Parent:** [Dirichlet principle](#dirichlet-principle)

Let $V$ be a closed [linear subspace](vector-space.md#vector-subspace) of a real [Hilbert space](hilbert-space.md), and let $Q(v)=a(v,v)$ for a symmetric [bounded bilinear form](bilinear-form.md#bounded-bilinear-form) that is nonnegative on the ambient space and coercive on $V$. Then $Q$ has a unique minimizer on every closed [affine subspace](vector-space.md#affine-subspace) $g+V$. If $Q(v_j)\to m=\inf_{g+V}Q$, the midpoint belongs to $g+V$ and the [parallelogram law](quadratic-form.md#parallelogram-law) gives $Q(v_j-v_k)\leq2Q(v_j)+2Q(v_k)-4m\to0$. Coercivity on $V$ makes the [minimizing sequence](#minimizing-sequence) Cauchy; completeness and continuity give a minimizer. The vanishing [first variation](#first-variation) is $a(u,v)=0$ for all $v\in V$. Two minimizers differ by $w\in V$ with $Q(w)=0$, so coercivity gives uniqueness. This proves the symmetric existence theorem directly, without invoking the [Lax-Milgram theorem](functional-analysis.md#lax-milgram-theorem).

### Sharp radial Dirichlet energy inequality

↑ **Parent:** [Dirichlet principle](#dirichlet-principle)

For $g(1)=1$ and finite displayed energy, the angular mode $g(r)\cos\theta$ has [Dirichlet energy](differential-geometry.md#dirichlet-energy) equal to $\pi$ times that integral. The [harmonic function](partial-differential-equation.md#harmonic-function) $r\cos\theta$ minimizes the energy with the same boundary data by the [Dirichlet principle](#dirichlet-principle), giving the bound. Finite energy forces $g(r)\to0$ as $r\to0$: Cauchy–Schwarz bounds changes of $g^2$ by twice the product of the two energy tails, so $g^2$ has a limit, and a nonzero limit would make $\int g^2/r$ divergent. Consequently completing the square gives the exact identity $\int_0^1[rg'^2+g^2/r]=1+\int_0^1r(g'-g/r)^2$. Equality occurs exactly for $g(r)=r$. This identity also covers finite-energy functions whose polar expression is not classically smooth at the centre.

## Optical ray in cylindrical coordinates

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Optical_ray_in_cylindrical_coordinates)

Fermat-type optical paths in cylindrical coordinates extremize refractive index times Euclidean arclength.

### Helical extremal

↑ **Parent:** [Optical ray in cylindrical coordinates](#optical-ray-in-cylindrical-coordinates)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Helical_extremal)

A helical extremal has constant radius and a polar angle linear in axial position.

## Noether theorem

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Noether_theorem)

Noether’s theorem associates a conserved quantity to each continuous variational symmetry.

### Mass-weighted oscillator symmetries

↑ **Parent:** [Noether theorem](#noether-theorem)

For independent coordinates with $L=\sum_i m_i(\dot x_i^2-\omega^2x_i^2)/2$, the variables $X_i=\sqrt{m_i}x_i$ give an isotropic oscillator even at unequal masses. Rotations of the $X_i$ are continuous symmetries. Their conserved [Noether charges](#noether-theorem) $X_iP_j-X_jP_i$ therefore predate any equality of physical masses. Equal masses alone cannot create new invariances of arbitrary additional interactions.

### Time-translation symmetry

↑ **Parent:** [Noether theorem](#noether-theorem)

Invariance under a shift of the time coordinate, with other required background structures held fixed. A continuous [time-translation symmetry](#time-translation-symmetry) gives an [energy](energy.md) [conservation law](mathematical-physics.md#conservation-law) through [Noether theorem](#noether-theorem). A generic expanding cosmological background is not stationary and need not supply a corresponding globally conserved total [energy](energy.md).

### Noether second theorem

↑ **Parent:** [Noether theorem](#noether-theorem)

Suppose an action is invariant under a local transformation $\delta\Phi_a=R_a\alpha+R_a^\mu\partial_\mu\alpha$ for every compactly supported function $\alpha$. Variation and integration by parts give the off-shell identity

$$
\sum_a\left(\mathcal E_aR_a-\partial_\mu(\mathcal E_aR_a^\mu)\right)\equiv0.
$$

Thus arbitrary local symmetry parameters imply dependencies among the field equations. In [gauge theory](classical-field-theory.md#gauge-theory), these identities accompany constraints rather than independent physical charges for each function. This complements the conserved-current statement of [Noether theorem](#noether-theorem).

#### Noether identity for abelian scalar gauge symmetry

↑ **Parent:** [Noether second theorem](#noether-second-theorem)

For $\delta A_\mu=\partial_\mu\alpha$, $\delta\phi=-ie\alpha\phi$ and $\delta\phi^*=ie\alpha\phi^*$, [Noether second theorem](#noether-second-theorem) gives

$$
-\partial_\mu\mathcal E_A^\mu-ie\phi\mathcal E_\phi+ie\phi^*\mathcal E_{\phi^*}\equiv0.
$$

This holds without imposing the field equations. On the matter equations it becomes a divergence identity for the electromagnetic equation, expressing compatibility with charge conservation. The Hamiltonian description carries the corresponding [Gauss law constraint in gauge theory](relativistic-quantum-field.md#gauss-law-constraint-in-gauge-theory).

### Noether conserved quantity for a mechanical point symmetry

↑ **Parent:** [Noether theorem](#noether-theorem)

If a time-independent [Lagrangian](#lagrangian) $L(q,\dot q)$ is invariant under a one-parameter point transformation with infinitesimal generator $\xi_i=\partial_sQ_i|_{s=0}$, then every Euler-Lagrange trajectory conserves

$$
J=\sum_i\frac{\partial L}{\partial\dot q_i}\xi_i.
$$

#### Action symmetry

↑ **Parent:** [Noether conserved quantity for a mechanical point symmetry](#noether-conserved-quantity-for-a-mechanical-point-symmetry)

An infinitesimal transformation that preserves the [action](lagrangian-mechanics.md#action) up to endpoint terms. For $\delta t=\varepsilon\phi$ and $\delta q_i=\varepsilon\psi_i$, invariance of $L\,dt$ yields the [Noether charge](classical-field-theory.md#noether-charge) $\sum_ip_i\psi_i-H\phi$, less any boundary-term generator.

## Second variation

↑ **Parent:** [Calculus of variations](calculus-of-variations.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Second_variation)

The second variation is the quadratic term in a functional's expansion along $u+\varepsilon\eta$; positivity on admissible variations is a local-minimum test.

### Coercive positivity of a second variation

↑ **Parent:** [Second variation](#second-variation)

For fixed-endpoint variations, a [second variation](#second-variation) is coercively positive if the displayed estimate holds for one constant $c>0$ and every admissible variation. The endpoint [Poincaré inequality](sobolev-space.md#poincare-inequality) makes this equivalent to a positive lower bound in the $W^{1,2}$ norm. It is stronger than strict positivity on each nonzero variation: $q(\varphi)=\int\varphi^2$ is strictly positive, but high-frequency variations make its ratio to $\int\varphi'^2$ tend to zero.

For $q=\int(p\varphi'^2+2r\varphi\varphi'+s\varphi^2)$ with [continuous](calculus.md#continuous-function) coefficients, coercive positivity implies $p\geq c$. Indeed, if $p-c<0$ on an interval, multiply a smooth [function](function.md) supported there by $\sin(nx)$. Its negative highest-[derivative](calculus.md#derivative) contribution has order $n^2$, while the mixed term has order at most $n$ and the remaining term is bounded. This contradicts the displayed inequality for large $n$. In particular coercive positivity implies the [Strengthened Legendre condition](#strengthened-legendre-condition), whereas mere strict positivity does not.

### Legendre necessary condition

↑ **Parent:** [Second variation](#second-variation)

A nonnegative [second variation](#second-variation) requires its highest-[derivative](calculus.md#derivative) coefficient $P=f_{vv}$ to be nonnegative. If it were negative on an interval, a smooth compactly supported factor times $\sin(nx)$ would have negative [derivative](calculus.md#derivative) energy of order $n^2$, while its zero-order energy stays bounded. Large $n$ would contradict nonnegativity. This is a local necessary condition; it does not rule out negative directions caused by the lower-order terms.

#### Strengthened Legendre condition

↑ **Parent:** [Legendre necessary condition](#legendre-necessary-condition)

Strict positivity of the highest-[derivative](calculus.md#derivative) coefficient on the closed parameter interval is the strengthened Legendre condition. Continuity then gives a uniform positive lower bound and makes the [Jacobi equation](#jacobi-equation) a regular second-order equation. It permits the [Jacobi positivity criterion](#jacobi-positivity-criterion). It is not necessary for mere strict positivity of a [second variation](#second-variation): $\int\varphi^2$ is strictly positive on nonzero variations even though its [derivative](calculus.md#derivative) coefficient vanishes.

### Jacobi equation

↑ **Parent:** [Second variation](#second-variation)

The Jacobi equation is the linearization of an [Euler-Lagrange equation](analysis.md#euler-lagrange-equation) about a stationary path. Its solutions describe infinitesimal one-parameter families of stationary paths.

#### Jacobi identity for the second variation

↑ **Parent:** [Jacobi equation](#jacobi-equation)

If $w$ is a nonvanishing solution of $-(Pw')'+Qw=0$, expanding the right-hand side gives the displayed identity. Integrating expresses a scalar [second variation](#second-variation) as a square plus a boundary term. A simple zero of $w$ at a fixed endpoint causes no difficulty for [Lipschitz](real-analysis.md#lipschitz-continuity) endpoint-vanishing variations, since $\varphi=O(x-a)$ makes the boundary term tend to zero. This identity is the scalar form of a [ground-state transform for a weighted Dirichlet energy](sobolev-space.md#ground-state-transform-for-a-weighted-dirichlet-energy).

### Conjugate point

↑ **Parent:** [Second variation](#second-variation)

A conjugate point marks a nonzero endpoint-vanishing Jacobi variation and the loss of positive definiteness of the second variation.

For the energy functional of a [Riemannian manifold](riemannian-geometry.md#riemannian-manifold), this variational condition yields [conjugate points along a geodesic](riemannian-geometry.md#conjugate-points).

#### Jacobi positivity criterion

↑ **Parent:** [Conjugate point](#conjugate-point)

Assume the [Strengthened Legendre condition](#strengthened-legendre-condition) $P>0$ and let $q(\varphi)=\int_a^b(P\varphi'^2+Q\varphi^2)$. Then $q$ is strictly positive on all nonzero fixed-endpoint [Lipschitz](real-analysis.md#lipschitz-continuity) variations exactly when the normalized [Jacobi equation](#jacobi-equation) solution with $w(a)=0$, $P(a)w'(a)=1$ has no zero in $(a,b]$. A zero at $c$ gives a nonzero variation equal to $w$ up to $c$ and zero thereafter, with $q=0$. Conversely, if no zero occurs, the [Jacobi identity for the second variation](#jacobi-identity-for-the-second-variation) writes $q$ as a nonnegative square. Equality forces $\varphi=Cw$, and the endpoint at $b$ forces $C=0$.

##### Regularized Jacobi criterion for a degenerate second variation

↑ **Parent:** [Jacobi positivity criterion](#jacobi-positivity-criterion)

For continuous $P\geq0,Q$, a scalar [second variation](#second-variation) $q=\int(P\varphi'^2+Q\varphi^2)$ is strictly positive on nonzero fixed-endpoint [Lipschitz](real-analysis.md#lipschitz-continuity) variations if and only if every regularized form $q_\eta$ for $\eta>0$ has no [conjugate point](#conjugate-point) in $(a,b]$, and the original weak Jacobi boundary problem has no nonzero [Lipschitz](real-analysis.md#lipschitz-continuity) solution. The [Jacobi positivity criterion](#jacobi-positivity-criterion) applies to each regularized coefficient $P+\eta>0$. Letting $\eta$ decrease to zero gives $q\geq0$. For a nonnegative [quadratic form](quadratic-form.md), $q(\varphi)=0$ forces its mixed [bilinear form](bilinear-form.md) with every [test function](distribution-theory.md#test-function) to vanish, by considering $q(\varphi+t\psi)$ for both signs of $t$. This is the weak [Jacobi equation](#jacobi-equation), so the kernel condition gives strict positivity. Necessity follows by the same argument in reverse. It distinguishes strict positivity from a uniform coercive estimate when the [derivative](calculus.md#derivative) coefficient degenerates.

#### Multiplicity of a conjugate point

↑ **Parent:** [Conjugate point](#conjugate-point)

Along a nonconstant affinely parametrized [geodesic](riemannian-geometry.md#geodesic), the multiplicity of a [conjugate point](#conjugate-point) at positive time $t_0$ is the dimension of the space of [Jacobi fields](riemann-curvature-tensor.md#jacobi-field) vanishing at both endpoints. The tangential component of such a [Jacobi field](riemann-curvature-tensor.md#jacobi-field) is affine and vanishes at both endpoints, hence is zero. Uniqueness for the [Jacobi field](riemann-curvature-tensor.md#jacobi-field) equation embeds this space into the $(n-1)$-dimensional normal space by $J\mapsto D_tJ(0)$. Thus its dimension is at most $n-1$.

#### Nonpositive sectional curvature excludes conjugate points

↑ **Parent:** [Conjugate point](#conjugate-point)

For a [Jacobi field](riemann-curvature-tensor.md#jacobi-field) along a [geodesic](riemannian-geometry.md#geodesic) with nonpositive [sectional curvature](second-fundamental-form.md#sectional-curvature), the curvature convention with positive round-sphere curvature gives

$$
(|J|^2)''=2|D_tJ|^2-2\langle R(J,\dot\gamma)\dot\gamma,J\rangle\ge0.
$$

Thus $|J|^2$ is nonnegative and convex. If it vanishes at both ends of a segment, convexity forces it to vanish everywhere. No nonzero [Jacobi field](riemann-curvature-tensor.md#jacobi-field) can vanish at both ends, so the segment has no [conjugate points](riemannian-geometry.md#conjugate-points). Only curvature of planes containing the [geodesic](riemannian-geometry.md#geodesic) tangent is needed, and completeness is unnecessary.

### Wirtinger inequality

↑ **Parent:** [Second variation](#second-variation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wirtinger_inequality)

For $f(0)=f(T)=0$,

$$
\int_0^T|f'|^2dt\geq\frac{\pi^2}{T^2}\int_0^T|f|^2dt,
$$

with equality for a multiple of $\sin(\pi t/T)$.

#### Minimum Dirichlet energy at fixed L2 norm on an interval

↑ **Parent:** [Wirtinger inequality](#wirtinger-inequality)

Expand a real function with zero endpoint values in its [Fourier sine series](fourier-series.md#fourier-sine-series), $y=\sum_{n\geq1}a_n\sin(n\pi x/L)$. The [Parseval identity](fourier-analysis.md#parseval-identity) gives $\int y^2=(L/2)\sum a_n^2$. For its [weak derivative](distribution-theory.md#weak-derivative), the [Fourier cosine series](fourier-series.md#fourier-cosine-series) has coefficients $(n\pi/L)a_n$ and zero constant term, so

$$
\int_0^L|y'|^2\,dx=\frac L2\sum_{n\geq1}\left(\frac{n\pi}L\right)^2a_n^2
\geq\frac{\pi^2}{L^2}\int_0^Ly^2\,dx.
$$

The derivative coefficient identity follows by [integration by parts](calculus.md#integration-by-parts), rather than by assuming pointwise differentiation of an arbitrary series. This proves the [Wirtinger inequality](#wirtinger-inequality) and its equality case. Under unit [L2 norm](real-analysis.md#l2-norm), the only real minimizers are $y=\pm\sqrt{2/L}\sin(\pi x/L)$.

#### Periodic Wirtinger inequality

↑ **Parent:** [Wirtinger inequality](#wirtinger-inequality)

If a continuously differentiable $L$-periodic function $f$ has mean zero, then

$$
\int_0^L f(s)^2\,ds
\leq\frac{L^2}{4\pi^2}\int_0^L f'(s)^2\,ds.
$$

Equality holds exactly for $f(s)=A\cos(2\pi s/L)+B\sin(2\pi s/L)$.

## ↑ Ancestors (4)

1. [Analysis](analysis.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-advanced-fluid-dynamics-course-of-the-university-of-oxford/2017.md#1/b/solution)
- [Solution](past-exam-of-the-advanced-fluid-dynamics-course-of-the-university-of-oxford/2017.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-4.md#16b/solution)
- [Solution](past-exam-of-the-solid-mechanics-course-of-the-university-of-oxford/2011.md#3/b/solution)
