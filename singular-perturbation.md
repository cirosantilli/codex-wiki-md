# Singular perturbation

↑ **Parent:** [Ordinary differential equation](differential-equation.md#ordinary-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Singular_perturbation)

A [singular perturbation](singular-perturbation.md) is a parameter-dependent problem whose limiting problem changes qualitatively as the parameter tends to zero. In an [ordinary differential equation](differential-equation.md#ordinary-differential-equation), a small coefficient of the highest [derivative](calculus.md#derivative) can reduce the order of the limiting [differential equation](differential-equation.md), preventing it from satisfying all the original [boundary conditions](differential-equation.md#boundary-condition). Different length or time scales often require different [asymptotic expansions](asymptotic-expansion.md).[§1.1.2, p. 2: regular and singular perturbations](mathematics-bibliography.md#asymptotic-analysis-and-singular-perturbation-theory-by-john-k-hunter)

Consider the [boundary value problem](boundary-value-problem.md)

$$
\epsilon y_\epsilon''+y_\epsilon'=0,\qquad 0<x<1,\qquad y_\epsilon(0)=0,\quad y_\epsilon(1)=1,\qquad \epsilon>0.
$$

This [second-order differential equation](differential-equation.md#second-order-differential-equation) is exactly solvable. Setting $v=y_\epsilon'$ gives the [first-order linear differential equation](linear-ordinary-differential-equation.md#first-order-linear-differential-equation) $\epsilon v'+v=0$, so $v=C e^{-x/\epsilon}$. One [integration](integral.md) and the two [boundary conditions](differential-equation.md#boundary-condition) give

$$
y_\epsilon(x)=\frac{1-e^{-x/\epsilon}}{1-e^{-1/\epsilon}}.
$$

Both [boundary conditions](differential-equation.md#boundary-condition) hold for every positive $\epsilon$. For numerical evaluation, write the same ratio as $\operatorname{expm1}(-x/\epsilon)/\operatorname{expm1}(-1/\epsilon)$, where $\operatorname{expm1}(t)$ evaluates the [exponential function](calculus.md#exponential-function) minus one without [catastrophic cancellation](floating-point-arithmetic.md#catastrophic-cancellation) near $t=0$. Keep the denominator for finite $\epsilon$: at $\epsilon=0.2$ it is approximately $0.993262$, rather than exactly one.

Setting $\epsilon=0$ gives $y_0'=0$. The [outer solution](#outer-expansion) selected by the right [boundary condition](differential-equation.md#boundary-condition) is therefore $y_0=1$, which fails the left [boundary condition](differential-equation.md#boundary-condition). The exact [exponential function](calculus.md#exponential-function) $e^{-x/\epsilon}$ shows how that mismatch is repaired: the solution rises from zero to almost one within a [boundary layer](continuum-mechanics.md#boundary-layer) of width $x=O(\epsilon)$, using [Big O notation](real-analysis.md#big-o-notation). For each fixed $x>0$, $y_\epsilon(x)\to1$, while $y_\epsilon(0)=0$ always. This [pointwise convergence](sequence-and-series.md#pointwise-convergence) fails to be [uniform convergence](sequence-and-series.md#uniform-convergence) to the [outer solution](#outer-expansion) on $[0,1]$, since $\sup_{0\leq x\leq1}|y_\epsilon(x)-1|=1$ for every $\epsilon>0$.

<a id="image-exact-solutions-with-a-shrinking-left-boundary-layer"></a>
![](singular-perturbation-boundary-layer-profiles.png)

**[Figure 1](#image-exact-solutions-with-a-shrinking-left-boundary-layer). Exact solutions with a shrinking left boundary layer**. The exact normalized profiles at $\epsilon=0.2$, $0.05$, and $0.01$ satisfy both [boundary conditions](differential-equation.md#boundary-condition). The dashed [outer solution](#outer-expansion) misses the left [boundary condition](differential-equation.md#boundary-condition). Colored dots mark $x=\epsilon$, where most of the initial rise has already occurred.

The coefficient $\epsilon$ is small, but its product with the [second derivative](calculus.md#second-derivative) need not be small. Direct [differentiation](calculus.md#differentiation) gives

$$
y_\epsilon'(x)=\frac{e^{-x/\epsilon}}{\epsilon(1-e^{-1/\epsilon})},\qquad
y_\epsilon''(x)=-\frac{e^{-x/\epsilon}}{\epsilon^2(1-e^{-1/\epsilon})}.
$$

At $x=\epsilon X$ with fixed $X\geq0$, these [derivatives](calculus.md#derivative) grow as $\epsilon^{-1}$ and $\epsilon^{-2}$ respectively as $\epsilon\to0^+$. Consequently $\epsilon y_\epsilon''$ and $y_\epsilon'$ have exactly equal magnitudes and opposite signs. Even away from the [boundary layer](continuum-mechanics.md#boundary-layer), their magnitudes remain equal in this example; both become exponentially small at each fixed positive $x$. The [outer expansion](#outer-expansion) neglects an exponentially small transient there, rather than establishing that one [derivative](calculus.md#derivative) term is smaller than the other everywhere.

To predict the width without knowing the exact solution, suppose an order-one change occurs over distance $\delta$. The [derivative](calculus.md#derivative) scales are $y'=O(\delta^{-1})$ and $y''=O(\delta^{-2})$. The [dominant balance](asymptotic-expansion.md#dominant-balance) $\epsilon/\delta^2\sim1/\delta$ gives $\delta\sim\epsilon$. The resulting [inner variable](#inner-variable) $X=x/\epsilon$ makes the [boundary layer](continuum-mechanics.md#boundary-layer) visible at a fixed scale. This is the useful feature of [singular perturbation](singular-perturbation.md): an apparently disappearing term identifies the missing structure when one measures its [derivatives](calculus.md#derivative) on the appropriate scale.

**Table of contents**

- [Beyond-all-orders boundary-value sensitivity](#beyond-all-orders-boundary-value-sensitivity)
- [Adiabatic elimination](#adiabatic-elimination)
- [Matched asymptotic expansion](#matched-asymptotic-expansion)
  - [Endpoint derivative in a negative-drift boundary layer](#endpoint-derivative-in-a-negative-drift-boundary-layer)
  - [Logistic crossover in a weakly nonlinear Euler equation](#logistic-crossover-in-a-weakly-nonlinear-euler-equation)
    - [Nonlinear crossover delayed by a small unstable-mode coefficient](#nonlinear-crossover-delayed-by-a-small-unstable-mode-coefficient)
  - [Nonlinear endpoint layer with a quadratic reaction](#nonlinear-endpoint-layer-with-a-quadratic-reaction)
    - [One-third-power scaling at a nonlinear turning endpoint](#one-third-power-scaling-at-a-nonlinear-turning-endpoint)
  - [Asymptotic matching condition](#asymptotic-matching-condition)
  - [Square-root reaction problem with nested boundary layers](#square-root-reaction-problem-with-nested-boundary-layers)
    - [First integral of a square-root reaction layer](#first-integral-of-a-square-root-reaction-layer)
  - [Nested layers at an essential singular endpoint](#nested-layers-at-an-essential-singular-endpoint)
  - [Matched expansion with square-root and logarithmic corrections](#matched-expansion-with-square-root-and-logarithmic-corrections)
  - [Logarithmic matching in a small-exponent boundary layer](#logarithmic-matching-in-a-small-exponent-boundary-layer)
  - [Gaussian interior layer of a conservative drift equation](#gaussian-interior-layer-of-a-conservative-drift-equation)
  - [Oscillatory endpoint with a quadratically vanishing drift](#oscillatory-endpoint-with-a-quadratically-vanishing-drift)
  - [First-order composite expansion for a positive drift](#first-order-composite-expansion-for-a-positive-drift)
  - [Logarithmically enhanced nonlinear boundary layer](#logarithmically-enhanced-nonlinear-boundary-layer)
  - [Boundary layer around a moving endpoint](#boundary-layer-around-a-moving-endpoint)
  - [Square-root boundary layer at a vanishing drift](#square-root-boundary-layer-at-a-vanishing-drift)
    - [Error-function logarithmic switchback](#error-function-logarithmic-switchback)
  - [Overlap region](#overlap-region)
  - [Intermediate asymptotic region](#intermediate-asymptotic-region)
  - [Interior layer at a simple zero of advection](#interior-layer-at-a-simple-zero-of-advection)
    - [Endpoint layers for reversed diffusion](#endpoint-layers-for-reversed-diffusion)
  - [Distinguished limit](#distinguished-limit)
  - [Inner expansion](#inner-expansion)
    - [Square-root-degenerate endpoint layer](#square-root-degenerate-endpoint-layer)
    - [Inner variable](#inner-variable)
  - [Outer expansion](#outer-expansion)
  - [Additive composite expansion](#additive-composite-expansion)
  - [Multiplicative composite expansion](#multiplicative-composite-expansion)
  - [Outflow boundary layer](#outflow-boundary-layer)
  - [Switchback term](#switchback-term)
    - [Logarithmic overlap creates a switchback term](#logarithmic-overlap-creates-a-switchback-term)
- [Method of multiple scales](#method-of-multiple-scales)
  - [Slow oscillator damping by a relaxing auxiliary variable](#slow-oscillator-damping-by-a-relaxing-auxiliary-variable)
  - [Averaged oscillator damping by a power of velocity](#averaged-oscillator-damping-by-a-power-of-velocity)
  - [Second-order resonance from quadratic oscillator coupling](#second-order-resonance-from-quadratic-oscillator-coupling)
  - [Averaged amplitude for position-dependent damping](#averaged-amplitude-for-position-dependent-damping)
    - [Absolute-value damping amplitude law](#absolute-value-damping-amplitude-law)
    - [Van der Pol amplitude evolution](#van-der-pol-amplitude-evolution)
      - [Shifted Van der Pol amplitude evolution](#shifted-van-der-pol-amplitude-evolution)
    - [Odd position-dependent damping has zero first-order amplitude drift](#odd-position-dependent-damping-has-zero-first-order-amplitude-drift)
  - [Secular term](#secular-term)
  - [Whitham modulation theory](#whitham-modulation-theory)
    - [Averaged Lagrangian](#averaged-lagrangian)
      - [Modulated-wave first integral](#modulated-wave-first-integral)
      - [Whitham modulation equation](#whitham-modulation-equation)
        - [Wave-action density](#wave-action-density)
          - [Wave-action conservation law](#wave-action-conservation-law)
  - [Amplitude-phase equations for a weakly perturbed oscillator](#amplitude-phase-equations-for-a-weakly-perturbed-oscillator)
    - [Oscillator coupled to slow damping feedback](#oscillator-coupled-to-slow-damping-feedback)
    - [Velocity-only forcing in averaged oscillator equations](#velocity-only-forcing-in-averaged-oscillator-equations)
      - [Quadratically damped oscillator](#quadratically-damped-oscillator)
      - [Cubic velocity anti-damping](#cubic-velocity-anti-damping)
    - [Conservative forcing in averaged oscillator equations](#conservative-forcing-in-averaged-oscillator-equations)
  - [Slow time](#slow-time)
  - [Weakly nonlinear expansion](#weakly-nonlinear-expansion)
    - [Quadratic wave interaction](#quadratic-wave-interaction)
      - [Resonant three-wave triad](#resonant-three-wave-triad)
      - [Detuning of a wave resonance](#detuning-of-a-wave-resonance)
      - [Phase matching for a quadratic wave interaction](#phase-matching-for-a-quadratic-wave-interaction)
        - [Two-to-one resonance of dispersive waves](#two-to-one-resonance-of-dispersive-waves)
          - [Explosive two-to-one amplitude system](#explosive-two-to-one-amplitude-system)
  - [Harmonic balance](#harmonic-balance)
  - [Solvability condition in the method of multiple scales](#solvability-condition-in-the-method-of-multiple-scales)
  - [Parametric resonance](#parametric-resonance)
    - [Primary instability tongue of a weak Mathieu oscillator](#primary-instability-tongue-of-a-weak-mathieu-oscillator)
    - [Primary parametric resonance of a two-to-one oscillator pair](#primary-parametric-resonance-of-a-two-to-one-oscillator-pair)
    - [Second instability tongue of a weak Mathieu oscillator](#second-instability-tongue-of-a-weak-mathieu-oscillator)
      - [Slow amplitudes for the second Mathieu instability tongue](#slow-amplitudes-for-the-second-mathieu-instability-tongue)
      - [Fourth-order edges of the second Mathieu instability tongue](#fourth-order-edges-of-the-second-mathieu-instability-tongue)

## Beyond-all-orders boundary-value sensitivity

↑ **Parent:** [Singular perturbation](singular-perturbation.md)

A homogeneous mode can be order one inside an interval and exponentially small at an endpoint. Adjusting an endpoint value beyond all algebraic orders can then change the interior solution by order one. In the [nested layers at an essential singular endpoint](#nested-layers-at-an-essential-singular-endpoint) example, the mode $\exp(-x/\epsilon-2\epsilon^2/x)$ has this behavior: prescribed exact endpoint values give a unique solution for each fixed positive $\epsilon$, but leading asymptotic endpoint data do not select a unique bounded family.

## Adiabatic elimination

↑ **Parent:** [Singular perturbation](singular-perturbation.md)

[Adiabatic elimination](#adiabatic-elimination) replaces a rapidly relaxing variable by its instantaneous stable quasistatic value. If $\dot R=-\Gamma(t)R+P(t)$ with $\Gamma>0$, write $R=R_0+\delta R$, $R_0=P/\Gamma$. Then $\dot{\delta R}+\Gamma\delta R=-\dot R_0$. After the transient, $\delta R\simeq-\dot R_0/\Gamma$ when coefficients vary slowly compared with $\Gamma^{-1}$. This gives both the leading reduction and its time-scale error; rapid relaxation alone does not justify an additional Taylor expansion in another parameter.

## Matched asymptotic expansion

↑ **Parent:** [Singular perturbation](singular-perturbation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Matched_asymptotic_expansion)

A [matched asymptotic expansion](#matched-asymptotic-expansion) constructs approximations in regions with different [distinguished limits](#distinguished-limit) and fixes their free constants by requiring agreement in an [overlap region](#overlap-region). The [inner expansion](#inner-expansion) resolves rapid variation; the [outer expansion](#outer-expansion) describes the surrounding region. Matching compares their common limiting behavior, rather than imposing distant [boundary conditions](differential-equation.md#boundary-condition) directly on a local approximation.[§§4.3.3–4.3.4, pp. 57–58: inner expansion and matching](mathematics-bibliography.md#asymptotic-analysis-and-singular-perturbation-theory-by-john-k-hunter)

For the [singular perturbation](singular-perturbation.md) problem $\epsilon y''+y'=0$, $y(0)=0$, $y(1)=1$, the leading [outer solution](#outer-expansion) is $y_0=1$. The [inner variable](#inner-variable) $X=x/\epsilon$ gives $Y_0''+Y_0'=0$ and $Y_0(0)=0$, hence $Y_0=A(1-e^{-X})$. In the [overlap region](#overlap-region) $\epsilon\ll x\ll1$, the [inner variable](#inner-variable) tends to infinity while the outer coordinate tends to zero. The [asymptotic matching condition](#asymptotic-matching-condition) is

$$
\lim_{X\to\infty}Y_0(X)=\lim_{x\to0^+}y_0(x)=1,
$$

so $A=1$. One concrete path through the [overlap region](#overlap-region) is $x=\sqrt\epsilon$: then $x\to0$ and $X=\epsilon^{-1/2}\to\infty$. Matching selects the free constant that the left [boundary condition](differential-equation.md#boundary-condition) alone could not determine.

Why choose the right [boundary condition](differential-equation.md#boundary-condition) for the [outer solution](#outer-expansion)? If instead one selects $y_0=0$ from the left, a proposed right [boundary layer](continuum-mechanics.md#boundary-layer) with $Z=(1-x)/\epsilon$ satisfies $U_0''-U_0'=0$. Its [general solution](linear-ordinary-differential-equation.md#general-solution) is $A+B e^Z$. Matching to zero as $Z\to\infty$ forces $A=B=0$, contradicting $U_0(0)=1$. The direction in which the [exponential function](calculus.md#exponential-function) decays determines which endpoint can carry the [boundary layer](continuum-mechanics.md#boundary-layer); endpoint selection is part of the calculation.

### Endpoint derivative in a negative-drift boundary layer

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

For $\epsilon y''-(1+x)y'+y=0$, $y(0)=1$, $y(1)=1+\epsilon$, the exact outer solution is $1+x$ and the mismatch is at the right endpoint. In $X=(1-x)/\epsilon$, matching gives $Y_0=2-e^{-2X}$ and $Y_1=-X+(1-X-X^2/2)e^{-2X}$. Differentiation at $X=0$ gives the displayed endpoint slope. The order-one term requires the first inner correction; differentiating only the leading boundary layer loses it.

### Logistic crossover in a weakly nonlinear Euler equation

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

A growing linear mode can make a formally small [derivative](calculus.md#derivative) nonlinearity order one at large distance. After the crossover scaling, the equation $XH''-H'+(H')^2=0$ reduces to a [logistic differential equation](differential-equation.md#logistic-differential-equation) in $\log X$ for $H'$. Matching $H\sim X^2/2$ at small $X$ gives $H'=X/(1+X)$ and the displayed primitive with $H(0)=0$. It changes from quadratic growth to linear growth without a finite turning singularity.

#### Nonlinear crossover delayed by a small unstable-mode coefficient

↑ **Parent:** [Logistic crossover in a weakly nonlinear Euler equation](#logistic-crossover-in-a-weakly-nonlinear-euler-equation)

When the early growing solution is $Ax^2$ and the nonlinear coefficient depends on $\varepsilon y'$, its crossover occurs at the displayed scale. If $A$ is order one this is $x=O(\varepsilon^{-1})$; if the initial slope suppresses the leading mode and $A=O(\varepsilon)$, it is delayed to $x=O(\varepsilon^{-2})$. The first nonzero perturbative seed must therefore be computed before constructing the global leading approximation; setting the small parameter to zero can erase the mode that ultimately dominates.

### Nonlinear endpoint layer with a quadratic reaction

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

For $q>0$, matching $Y\to-q$, $Y'\to0$ fixes the [first integral](differential-equation.md#first-integral) to $(Y')^2=(q-2Y)(Y+q)^2/3$. Hence endpoint values above $q/2$ cannot match this outer branch. The upper family is $Y=-q+(3q/2)\operatorname{sech}^2[\sqrt q(\xi-\xi_0)/2]$. An endpoint value strictly between $-q$ and $q/2$ admits two translations, one initially approaching $-q$ and one initially moving towards the turning value $q/2$. Values below $-q$ give the unique lower family $Y=-q-(3q/2)\operatorname{csch}^2[\sqrt q(\xi+\xi_0)/2]$ with $\xi_0>0$. Matching to zero instead gives $(Y')^2=-qY^2-2Y^3/3$, which forbids a nonconstant real approach to zero. These are leading [boundary layer](continuum-mechanics.md#boundary-layer) classifications, not exact multiplicity theorems at degenerate endpoint data.

#### One-third-power scaling at a nonlinear turning endpoint

↑ **Parent:** [Nonlinear endpoint layer with a quadratic reaction](#nonlinear-endpoint-layer-with-a-quadratic-reaction)

In $\epsilon y''+xy+y^2=0$, balancing all three terms where the outer branches $0$ and $-x$ meet gives the displayed [dominant balance](asymptotic-expansion.md#dominant-balance) and the inner equation $Y''+XY+Y^2=0$. Matching to $-X$ and writing $Y=-X+u$ gives $u''-Xu+u^2=0$. Its linearized decaying correction is an [Airy function](linear-ordinary-differential-equation.md#airy-function); the growing correction is excluded. Matching to zero instead gives $Y''+XY=0$, whose nonzero [Airy function](linear-ordinary-differential-equation.md#airy-function) combinations oscillate. Thus the acceptable matching branches differ qualitatively at the turning endpoint.

### Asymptotic matching condition

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

An asymptotic matching condition requires the [inner expansion](#inner-expansion) and [outer expansion](#outer-expansion), re-expressed in a common overlap region, to agree to the retained order. Both function values and slopes may constrain the free constants. In the [square-root reaction problem with nested boundary layers](#square-root-reaction-problem-with-nested-boundary-layers), the shared small plateau sets the [first integral of a square-root reaction layer](#first-integral-of-a-square-root-reaction-layer), while its large-field fourth-power tail fixes the neighboring broad layer.

### Square-root reaction problem with nested boundary layers

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

For fixed $k>0$ and endpoint values $y(0)=0$, $y(1)=1$, the [outer solution](#outer-expansion) is $y\sim\varepsilon^2k^2$. The left [boundary layer](continuum-mechanics.md#boundary-layer) has width $\varepsilon$. At the right, a layer of width $\sqrt\varepsilon$ carries the order-one rise, and a translated layer of width $\varepsilon$ connects its inner edge to the small plateau. The [dominant balance](asymptotic-expansion.md#dominant-balance) depends on both amplitude and derivative scale; using the same scale at both ends loses a necessary match.

#### First integral of a square-root reaction layer

↑ **Parent:** [Square-root reaction problem with nested boundary layers](#square-root-reaction-problem-with-nested-boundary-layers)

After $y=\varepsilon^2Y$ and $x=\varepsilon\xi$ or a translated version, the layer equation is $Y''-\sqrt Y+k=0$. Multiplying by $Y'$ and matching $Y=k^2$, $Y'=0$ fixes the energy constant to $k^3/3$ and gives the displayed factorization. The increasing branch below $k^2$ approaches it at positive infinity; the increasing branch above it leaves it at negative infinity and grows like $\xi^4/144$. This supplies both interfaces of the [square-root reaction problem with nested boundary layers](#square-root-reaction-problem-with-nested-boundary-layers).

### Nested layers at an essential singular endpoint

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

Multiplication by $x^2$ makes this example exactly integrable once: $\epsilon x^2y\prime+(x^2-2\epsilon^3)y=C$. Its homogeneous solution is $\exp(-x/\epsilon-2\epsilon^2/x)$. A solution with $y(1)=\epsilon^3$ that remains uniformly bounded needs $C\sim\epsilon^3$, hence $y(0)\sim-1/2$. The scales $x=O(\epsilon)$ and $x=O(\epsilon^2)$ connect the small outer solution to the order-one endpoint value. Bounded homogeneous contributions remain invisible to algebraic matching at the right boundary.

### Matched expansion with square-root and logarithmic corrections

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

A decaying algebraic tail in an inner [asymptotic expansion](asymptotic-expansion.md) can become a fractional-order outer correction after rescaling. For an inner tail proportional to $r^{-1/2}$ and outer variable $x=\epsilon r$, the outer correction is proportional to $\epsilon^{1/2}x^{-1/2}$. If the next outer correction contains $\epsilon\log x$, expressing it in the inner variable produces both $\epsilon\log r$ and $\epsilon\log\epsilon$. Omitting the latter loses a term larger than a plain $O(\epsilon)$ correction. Matching must include all these scales and constants, rather than only the leading algebraic powers.

### Logarithmic matching in a small-exponent boundary layer

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

In a singular first-order equation with coefficient $x+\epsilon$, an outer correction proportional to $\epsilon\log x$ cannot be evaluated at the endpoint. The inner scale $x=\epsilon X$ changes it to $\epsilon\log\epsilon+\epsilon\log(1+X)$. Matching retains the logarithmic constant, which is larger than a plain order-epsilon correction. For $(x+\epsilon)y'=\epsilon y$, $y(1)=1$, the exact solution $[(x+\epsilon)/(1+\epsilon)]^\epsilon$ verifies the displayed endpoint asymptotic and its remainder.

### Gaussian interior layer of a conservative drift equation

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

The equation $\epsilon y''+xy'+y=0$ integrates to $\epsilon y'+xy=C$. Equal endpoint data $y(-1)=y(1)=A$ force $C=0$ and give the unique Gaussian solution above. Its central width is $\sqrt\epsilon$, with amplitude $A e^{1/(2\epsilon)}$. The exponentially large central mode is missed by an assumed bounded algebraic [outer expansion](#outer-expansion) $C/x$. Changes of order one relative to either endpoint value occur over distance $O(\epsilon)$ from that endpoint.

### Oscillatory endpoint with a quadratically vanishing drift

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

For $\epsilon y''+s^2y'+y=0$ on $s\geq0$, removing the drift by $y=e^{-s^3/(6\epsilon)}v$ gives

$$
\epsilon^2v''=(s^4/4+\epsilon s-\epsilon)v.
$$

The transformed potential changes sign at $s_t\sim\sqrt2\epsilon^{1/4}$. [WKB approximation](analysis.md#wkb-approximation) is oscillatory inside and exponential outside this turning region; an [Airy turning-point connection formula](analysis.md#airy-turning-point-connection-formula) applies over width $\epsilon^{5/12}$. At the endpoint the wavelength is $\sqrt\epsilon$, while the physical exponential prefactor changes on the envelope scale $\epsilon^{1/3}$. Balancing only diffusion and drift and declaring a single $\epsilon^{1/3}$ layer misses the zeroth-order term and the turning region. Matching constants may be singular at homogeneous boundary-value resonances.

### First-order composite expansion for a positive drift

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

For $\epsilon y''+a(x)y'+b(x)y=0$ with smooth $a$ bounded positively away from zero, the first-order equation for the [outer expansion](#outer-expansion) is selected by the right [boundary condition](differential-equation.md#boundary-condition). The left mismatch is repaired on the scale $\xi=x/\epsilon$. If $a(0)=a_0>0$, the leading inner transient is $B e^{-a_0\xi}$. Its next equation is $Y_1''+a_0Y_1'=-a'(0)\xi Y_0'-b(0)Y_0$. Matching its constant and linear large-$\xi$ terms to the [outer expansion](#outer-expansion) permits an order-$\epsilon$ composite approximation. A sign reversal of the drift places the transient at the opposite endpoint.

### Logarithmically enhanced nonlinear boundary layer

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

If a leading [outer expansion](#outer-expansion) diverges as $\log x$ and a [derivative](calculus.md#derivative) coefficient contains $x-\varepsilon z$, balancing that nonlinear correction gives a layer larger than $O(\varepsilon)$. Write $x=\varepsilon L X$ with $L=\log(1/\varepsilon)$ and subtract the large negative constant from $z$. Matching often introduces a $\log L$ correction and yields an endpoint slope of order $1/(\varepsilon L)$. The balance must be derived from the actual equation; logarithmic divergence alone does not fix a universal layer width.

### Boundary layer around a moving endpoint

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

For $\varepsilon xw''+w'+2xw=0$ with left endpoint $x=\varepsilon$, diffusion there is of size $\varepsilon^2$. The distinguished coordinate is $z=(x-\varepsilon)/\varepsilon^2$, giving $(1+\varepsilon z)W''+W'+2\varepsilon^3(1+\varepsilon z)W=0$. Matching to one with zero left value gives $W=1-e^{-z}-\varepsilon z(z+2)e^{-z}/2+O(\varepsilon^2)$. The layer width is different from the endpoint's distance from zero.

### Square-root boundary layer at a vanishing drift

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

In $\varepsilon y''+2xy'-2xy=0$, the drift vanishes at the endpoint $x=0$. Balancing diffusion against drift gives the [inner expansion](#inner-expansion) coordinate $z=x/\sqrt\varepsilon$. The leading layer equation is $Y''+2zY'=0$, with a bounded [error function](integral.md#error-function) profile. A regular outer first-order calculation alone cannot impose both endpoint values.

#### Error-function logarithmic switchback

↑ **Parent:** [Square-root boundary layer at a vanishing drift](#square-root-boundary-layer-at-a-vanishing-drift)

If an [outer expansion](#outer-expansion) contains $-(\varepsilon/2)\log x$ and the layer coordinate is $x=\sqrt\varepsilon z$, its overlap contains $-(\varepsilon/2)\log z-(\varepsilon/4)\log\varepsilon$. Matching forces an [inner expansion](#inner-expansion) term $-(\varepsilon/4)\log\varepsilon\operatorname{erf}z$ when that homogeneous profile tends to one in the overlap and vanishes at the boundary. The logarithm multiplies the matching profile, rather than an arbitrary constant.

### Overlap region

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

An overlap region is a parameter-dependent range in which two neighboring [asymptotic expansions](asymptotic-expansion.md) have simultaneously ordered common limits. Between scales $\epsilon^2$ and $\epsilon$, it is $\epsilon^2\ll x\ll\epsilon$: the narrow coordinate tends to infinity while the wider coordinate tends to zero. Matching uses these limiting descriptions, not an assertion that either expansion is uniform at all values of the other's scaled variable.

### Intermediate asymptotic region

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

An intermediate asymptotic region has a scale between two other scales and provides their connecting [matched asymptotic expansion](#matched-asymptotic-expansion). It can be needed because a coefficient changes its dominant form before the narrowest region's highest-derivative balance is reached. For example, a coefficient $x+\epsilon$ changes near $x=O(\epsilon)$ even when the fast [inner expansion](#inner-expansion) has width $O(\epsilon^2)$. The intermediate solution must be matched at both ends rather than assigned an independent boundary value.

### Interior layer at a simple zero of advection

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

In $\varepsilon^2y''+a(x)y'+\cdots=f$, a simple zero $a(x_*)=0$, $a'(x_*)\ne0$, balances diffusion and advection on width $\varepsilon$. With $a(x)\simeq2(x-x_*)$, the leading homogeneous inner equation is $Y''+2zY'=0$, whose bounded solutions are constants and the [error function](integral.md#error-function). Thus distinct order-one [outer solutions](#outer-expansion) can match across an interior transition. Reversing the diffusion sign makes the nonconstant homogeneous solution grow at both ends, changing the matching structure.

#### Endpoint layers for reversed diffusion

↑ **Parent:** [Interior layer at a simple zero of advection](#interior-layer-at-a-simple-zero-of-advection)

For $-\varepsilon^2y''+2(x-x_*)y'+\cdots=f$ on an interval straddling $x_*$, the bounded leading interior solution cannot connect unequal constants. A common bulk value is instead selected by an inner [solvability condition](linear-operator-theory.md#solvability-condition), and width-$\varepsilon^2$ endpoint layers enforce the two boundary values. At endpoints $x=0,2$ with $x_*=1$, their leading decaying factors are $e^{-2x/\varepsilon^2}$ and $e^{-2(2-x)/\varepsilon^2}$. The interior layer still corrects derivative mismatches at smaller amplitude.

### Distinguished limit

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

A distinguished limit rescales variables so that two or more effects enter the leading asymptotic balance together. It identifies a region whose governing equation differs from the equations in adjacent scales.

### Inner expansion

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inner_expansion)

An inner expansion resolves a region in which a stretched independent variable makes otherwise small effects enter the leading balance.

#### Square-root-degenerate endpoint layer

↑ **Parent:** [Inner expansion](#inner-expansion)

The [singular perturbation](singular-perturbation.md) equation $\epsilon\sqrt x\,u''+u'=0$ balances its derivatives on the width $x=\epsilon^2X$. The inner equation is $\sqrt X\,U''+U'=0$, so $U'=Ce^{-2\sqrt X}$. Its solution with $U(0)=0$ and $U(\infty)=1$ is the displayed $H$, since $\int_0^\infty e^{-2\sqrt q}dq=1/2$. Near zero $H=2X-8X^{3/2}/3+O(X^2)$, so the first derivative is finite while the second is singular. Treat the differential equation on the open interval and impose the endpoint value by continuous extension.

#### Inner variable

↑ **Parent:** [Inner expansion](#inner-expansion)

An [inner variable](#inner-variable) is a stretched coordinate such as $\xi=(x-x_0)/\delta(\epsilon)$ that remains order one inside a thin region of width $\delta(\epsilon)$. Its scale is chosen by a [dominant balance](asymptotic-expansion.md#dominant-balance), rather than by the size of a coefficient alone.

For the [singular perturbation](singular-perturbation.md) problem $\epsilon y''+y'=0$ with $y(0)=0$, $y(1)=1$, set $X=x/\epsilon$ and $Y_\epsilon(X)=y_\epsilon(\epsilon X)$. The [chain rule](calculus.md#chain-rule) gives

$$
\frac{d}{dx}=\epsilon^{-1}\frac{d}{dX},\qquad
\epsilon y_\epsilon''+y_\epsilon'=\epsilon^{-1}(Y_\epsilon''+Y_\epsilon').
$$

Thus both [derivative](calculus.md#derivative) terms survive in the inner [differential equation](differential-equation.md) $Y_\epsilon''+Y_\epsilon'=0$. The exact domain is $0\leq X\leq1/\epsilon$, with

$$
Y_\epsilon(X)=\frac{1-e^{-X}}{1-e^{-1/\epsilon}},\qquad
Y_0(X)=1-e^{-X}.
$$

For bounded $X$, $Y_\epsilon\to Y_0$ as $\epsilon\to0^+$: the [inner expansion](#inner-expansion) has a nonconstant limiting profile even though the [outer solution](#outer-expansion) is constant. The finite-$\epsilon$ profiles nearly collapse onto $Y_0$ after rescaling, with their remaining difference coming from the normalization at the distant right endpoint.

<a id="image-inner-rescaling-reveals-the-common-profile-and-derivative-balance"></a>
![](singular-perturbation-inner-rescaling-balance.png)

**[Figure 2](#image-inner-rescaling-reveals-the-common-profile-and-derivative-balance). Inner rescaling reveals the common profile and derivative balance**. Left: the exact normalized profiles nearly coincide as functions of the [inner variable](#inner-variable) $X=x/\epsilon$; the $\epsilon=0.2$ curve ends at $X=5$, its actual right boundary. Right: multiplication of the original [differential equation](differential-equation.md) by $\epsilon$ gives the signed terms $\epsilon y'=Y'$ and $\epsilon^2y''=Y''$, which cancel exactly.

### Outer expansion

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Outer_expansion)

An [outer expansion](#outer-expansion) describes the solution away from a thin or distant region resolved by an [inner expansion](#inner-expansion). It is matched to that [inner expansion](#inner-expansion) in their common [overlap region](#overlap-region). Its range of validity must be specified: an approximation at each fixed positive $x$ need not have [uniform convergence](sequence-and-series.md#uniform-convergence) down to an endpoint.

For the [singular perturbation](singular-perturbation.md) problem $\epsilon y''+y'=0$, $y(0)=0$, $y(1)=1$, try the [asymptotic expansion](asymptotic-expansion.md) $y\sim y_0+\epsilon y_1+\epsilon^2y_2+\cdots$ at fixed $x>0$. Substitution gives $y_0'=0$ and $y_n'=-y_{n-1}''$ for $n\geq1$. Expanding the right [boundary condition](differential-equation.md#boundary-condition) gives $y_0(1)=1$ and $y_n(1)=0$ for $n\geq1$. Therefore $y_0=1$ and every higher coefficient vanishes. The missing [boundary layer](continuum-mechanics.md#boundary-layer) is exponentially small at each fixed positive $x$, invisible to all these powers of $\epsilon$.

The exact solution supplies a quantitative limit. For every fixed $a\in(0,1)$,

$$
\sup_{a\leq x\leq1}|y_\epsilon(x)-1|
=\frac{e^{-a/\epsilon}-e^{-1/\epsilon}}{1-e^{-1/\epsilon}}
\leq\frac{e^{-a/\epsilon}}{1-e^{-1/\epsilon}}\longrightarrow0.
$$

This is [uniform convergence](sequence-and-series.md#uniform-convergence) on $[a,1]$. On $[0,1]$ the same [supremum norm](normed-vector-space.md#supremum-norm) of the error is exactly one. The [inner expansion](#inner-expansion) supplies the endpoint information that this [outer expansion](#outer-expansion) cannot encode.

### Additive composite expansion

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

An [additive composite expansion](#additive-composite-expansion) combines an [inner expansion](#inner-expansion) and an [outer expansion](#outer-expansion) by subtracting their common behavior in the [overlap region](#overlap-region):

$$
y_{\mathrm{comp}}=y_{\mathrm{out}}+y_{\mathrm{in}}-y_{\mathrm{overlap}}.
$$

The subtraction removes the part counted twice. Near the [boundary layer](continuum-mechanics.md#boundary-layer), the [outer expansion](#outer-expansion) cancels the overlap contribution; away from the [boundary layer](continuum-mechanics.md#boundary-layer), the [inner expansion](#inner-expansion) cancels it. An error estimate is needed to establish accuracy across the whole domain.[§4.3.5, p. 58: uniform solution and overlap subtraction](mathematics-bibliography.md#asymptotic-analysis-and-singular-perturbation-theory-by-john-k-hunter)

For the [singular perturbation](singular-perturbation.md) problem $\epsilon y''+y'=0$, $y(0)=0$, $y(1)=1$, the [outer solution](#outer-expansion) is one, the leading [inner expansion](#inner-expansion) is $1-e^{-x/\epsilon}$, and their overlap is one. Thus $y_{\mathrm{comp}}=1-e^{-x/\epsilon}$. With $q=e^{-1/\epsilon}$, comparison with the exact normalized solution gives

$$
y_\epsilon(x)-y_{\mathrm{comp}}(x)
=\frac{q(1-e^{-x/\epsilon})}{1-q},\qquad
\sup_{0\leq x\leq1}|y_\epsilon-y_{\mathrm{comp}}|=q.
$$

The [supremum norm](normed-vector-space.md#supremum-norm) error is therefore exponentially small on the entire interval, even though the [outer solution](#outer-expansion) alone has error one. This is an error bound for function values; errors in [derivatives](calculus.md#derivative) have additional powers of $\epsilon^{-1}$.

The composite satisfies the [differential equation](differential-equation.md) exactly but has right [boundary condition](differential-equation.md#boundary-condition) $y_{\mathrm{comp}}(1)=1-q$. Dividing it by $1-q$ restores that [boundary condition](differential-equation.md#boundary-condition) and recovers the exact solution. This example makes both the strength and the limit of matching explicit: it gives a global approximation, while finite-$\epsilon$ normalization can still carry information beyond every algebraic order.

### Multiplicative composite expansion

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

When inner and outer approximations share a nonzero multiplicative overlap, a multiplicative composite divides their product by that common part. It is especially convenient when different regions contribute separate exponential or boundary-layer factors.

### Outflow boundary layer

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

For $\epsilon y''+a(x)y'+b(x)y=0$ with $a>0$, the reduced first-order outer problem takes its boundary condition at the right endpoint. A rapidly decaying exponential in $x/\epsilon$ supplies the otherwise unsatisfied left-end condition, so the layer lies at the outflow end for the fast mode associated with this sign convention.

### Switchback term

↑ **Parent:** [Matched asymptotic expansion](#matched-asymptotic-expansion)

A switchback term such as $\epsilon\log\epsilon$ is forced into a matched expansion when logarithms of a stretched coordinate split into parameter-dependent and local pieces in the overlap region.

#### Logarithmic overlap creates a switchback term

↑ **Parent:** [Switchback term](#switchback-term)

If a stretched variable is $x=\epsilon r$ and an [outer expansion](#outer-expansion) contains $\epsilon^2\log x$, its expression in the fixed-$r$ region is $\epsilon^2\log r+\epsilon^2\log\epsilon$. The parameter logarithm must therefore be present in the [inner expansion](#inner-expansion), often multiplying a homogeneous solution selected by a boundary condition. An ansatz containing only integer powers with parameter-independent coefficients misses this [switchback term](#switchback-term). The same reasoning applies to other powers of $\epsilon$ and other stretched-coordinate scalings.

## Method of multiple scales

↑ **Parent:** [Singular perturbation](singular-perturbation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Method_of_multiple_scales)

The method of multiple scales treats fast and slow variables such as $t$ and $T=\epsilon t$ as independent, then removes resonant forcing to obtain slow amplitude and phase equations.

### Slow oscillator damping by a relaxing auxiliary variable

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

For $x''+3\epsilon yx'+x=2(y')^2$ and $y'=\epsilon(1+x-y)$ with leading oscillation $x=A(\tau)\sin t$, $\tau=\epsilon t$, averaging the auxiliary equation gives $Y'=1-Y$. Cancellation of resonant forcing in the oscillator gives $2A'+3YA=0$. With $Y(0)=3$ and $A(0)=1$, $Y=1+2e^{-\tau}$ and the displayed amplitude follows. Bounded oscillatory corrections repair the instantaneous auxiliary equation; secular terms in a fixed-time expansion show why the slow scale is needed.

### Averaged oscillator damping by a power of velocity

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

For $y''+\epsilon(y')^n+y=0$, the [method of multiple scales](#method-of-multiple-scales) gives no first-order phase drift. If $n$ is odd, the [amplitude](wave.md#wave-amplitude) obeys the displayed damping law with $C_n=2^{-(n+1)}\binom{n+1}{(n+1)/2}$. If $n$ is even, the average is zero and the amplitude is unchanged on the first slow time $T=\epsilon t$. The odd case dissipates [mechanical energy](energy.md#mechanical-energy), whereas the even case is reversible and its force is not damping of both velocity signs.

### Second-order resonance from quadratic oscillator coupling

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

Two fundamental harmonics of [frequency](wave.md#frequency) one multiply into only a constant and second harmonics. The first-order [solvability condition in the method of multiple scales](#solvability-condition-in-the-method-of-multiple-scales) therefore has no amplitude-changing resonant coupling. Their first-order particular corrections can mix back into the fundamental at second order, selecting the possible scale $t=O(\epsilon^{-2})$. Detuning may suppress the resulting [resonance](dynamical-systems.md#resonance), so identifying this scale alone does not prove instability for every initial state.

### Averaged amplitude for position-dependent damping

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

For $x\prime\prime+\epsilon f(x)x\prime+x=0$, write $x_0=A(T)\cos(t+\theta)$ and $T=\epsilon t$. Removing [secular terms](#secular-term) gives $A_T=-A\langle f(A\cos\psi)\sin^2\psi\rangle$ and $\theta_T=0$, where the brackets mean a period average. This is the first-order [solvability condition in the method of multiple scales](#solvability-condition-in-the-method-of-multiple-scales), with a slowly evolving amplitude and no first-order frequency correction.

#### Absolute-value damping amplitude law

↑ **Parent:** [Averaged amplitude for position-dependent damping](#averaged-amplitude-for-position-dependent-damping)

For $x''+\varepsilon|x|x'+x=0$ and unit initial amplitude, averaging uses $\langle|\cos\psi|\sin^2\psi\rangle=2/(3\pi)$. Thus $A_T=-2A^2/(3\pi)$ and the displayed algebraic envelope follows. The leading phase has no first-order drift. The dissipation is amplitude dependent, so an exponential envelope with a constant decay rate would give the wrong long-time scale.

#### Van der Pol amplitude evolution

↑ **Parent:** [Averaged amplitude for position-dependent damping](#averaged-amplitude-for-position-dependent-damping)

For $x''+\varepsilon(x^2-1)x'+x=0$, the [averaged amplitude for position-dependent damping](#averaged-amplitude-for-position-dependent-damping) has the displayed logistic-type equation. With $A(0)=1$, its positive solution is $A(T)=2/\sqrt{1+3e^{-T}}$. Small amplitudes grow and large ones decay toward the stable value two; the leading oscillation is $A(\varepsilon t)\cos t$.

##### Shifted Van der Pol amplitude evolution

↑ **Parent:** [Van der Pol amplitude evolution](#van-der-pol-amplitude-evolution)

For $x''+\epsilon c(1-x^2)x'+x=k$, use $T=\epsilon t$ and $x=k-r(T)\cos(t+\phi(T))$. Removal of [secular terms](#secular-term) gives $\phi_T=0$ and the displayed [amplitude equation](bifurcation-theory.md#amplitude-equation). With $R=r^2$, $R_T=c(k^2-1)R+(c/4)R^2$, which is explicitly integrable. If $c$ is replaced by a slowly varying coefficient $C(T)$, the same solution uses the accumulated time $\int_0^T C(s)\,ds$. The [method of multiple scales](#method-of-multiple-scales) is uniform on bounded slow-time intervals only while its [amplitude](wave.md#wave-amplitude) and correction estimates remain bounded.

#### Odd position-dependent damping has zero first-order amplitude drift

↑ **Parent:** [Averaged amplitude for position-dependent damping](#averaged-amplitude-for-position-dependent-damping)

If $f$ is odd, its average $\langle f(A\cos\psi)\sin^2\psi\rangle$ vanishes under a half-period shift. Hence the [averaged amplitude for position-dependent damping](#averaged-amplitude-for-position-dependent-damping) is constant at first order. Odd-power damping creates only even harmonics when multiplied by the leading oscillator velocity; these do not resonate with the fundamental harmonic. Higher-order drift is still possible.

### Secular term

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

A secular term grows in a nominal perturbation correction and eventually invalidates an otherwise ordered expansion. In the [method of multiple scales](#method-of-multiple-scales), a solvability condition removes resonant forcing that would generate such growth.

### Whitham modulation theory

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

Whitham modulation theory averages a variational wave equation over a fast periodic phase and derives slow equations for its local wavenumber, frequency, and amplitude.

#### Averaged Lagrangian

↑ **Parent:** [Whitham modulation theory](#whitham-modulation-theory)

The averaged Lagrangian is the phase average of a Lagrangian evaluated on a periodic wave profile. Variation with respect to profile parameters gives the local dispersion relation, while variation of the slow phase gives a modulation conservation law.

##### Modulated-wave first integral

↑ **Parent:** [Averaged Lagrangian](#averaged-lagrangian)

Multiplying a one-dimensional Euler--Lagrange wave equation by the derivative of its periodic profile with respect to fast phase produces a phase first integral plus slow divergence terms. Phase averaging removes the periodic derivative and yields the slow phase equation.

##### Whitham modulation equation

↑ **Parent:** [Averaged Lagrangian](#averaged-lagrangian)

For local wavenumber $k=\Theta_X$, frequency $\omega=-\Theta_T$, and averaged Lagrangian $\overline L(k,\omega,\ldots)$, slow-phase variation gives

$$
\partial_X\overline L_k-\partial_T\overline L_\omega=0.
$$

###### Wave-action density

↑ **Parent:** [Whitham modulation equation](#whitham-modulation-equation)

For an averaged Lagrangian, the wave-action density is $W=\partial\overline L/\partial\omega$, up to the sign convention used for the fast phase.

###### Wave-action conservation law

↑ **Parent:** [Wave-action density](#wave-action-density)

In a slowly varying conservative medium, wave action obeys a continuity equation with flux equal to wave-action density times group velocity.

### Amplitude-phase equations for a weakly perturbed oscillator

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

For $u''+u=\epsilon f(u,u',\epsilon t)$, write $u_0=R(T)\cos(t+\phi(T))$ with $T=\epsilon t$. Removing resonant sine and cosine forcing gives

$$
R'=-\langle f\sin(t+\phi)\rangle,
\qquad
R\phi'=-\langle f\cos(t+\phi)\rangle.
$$

#### Oscillator coupled to slow damping feedback

↑ **Parent:** [Amplitude-phase equations for a weakly perturbed oscillator](#amplitude-phase-equations-for-a-weakly-perturbed-oscillator)

For $x''+x=-2\varepsilon yx'$ and $y'=\varepsilon g(x)$, the [method of multiple scales](#method-of-multiple-scales) gives the displayed [amplitude-phase equations](#amplitude-phase-equations-for-a-weakly-perturbed-oscillator), together with constant leading phase. For $g(x)=x$, $Y$ is constant and $R$ changes exponentially. For $g(x)=\log|x|$ and positive amplitude, the integrable phase average is $\log(R/2)$. Thus $L=\log(R/2)$ obeys $L_{TT}+L=0$ with $L_T=-Y$. The identically zero oscillator is inadmissible for logarithmic feedback, whose force is undefined there.

#### Velocity-only forcing in averaged oscillator equations

↑ **Parent:** [Amplitude-phase equations for a weakly perturbed oscillator](#amplitude-phase-equations-for-a-weakly-perturbed-oscillator)

When the weak force depends only on [velocity](classical-mechanics.md#velocity), the phase average is a periodic total [derivative](calculus.md#derivative) and vanishes. The leading phase is constant, while the amplitude evolves according to the remaining average. The sign of that drift determines damping or growth and must be checked from the force, rather than inferred from its [velocity](classical-mechanics.md#velocity) dependence alone.

##### Quadratically damped oscillator

↑ **Parent:** [Velocity-only forcing in averaged oscillator equations](#velocity-only-forcing-in-averaged-oscillator-equations)

For initial amplitude one, the [method of multiple scales](#method-of-multiple-scales) gives $x\simeq A(\epsilon t)\sin t$ with $A_T=-4A^2/(3\pi)$, hence $A=1/(1+4\epsilon t/(3\pi))$. Positive damping causes algebraic decay. Negative damping yields a formal finite-time amplitude pole, but the weak-damping assumption fails before it because $|\epsilon|A$ becomes order one. A leading approximation has order-$|\epsilon|$ displacement error on fixed slow-time intervals away from that pole.

##### Cubic velocity anti-damping

↑ **Parent:** [Velocity-only forcing in averaged oscillator equations](#velocity-only-forcing-in-averaged-oscillator-equations)

For $y''+y=\varepsilon(y')^3$ with positive $\varepsilon$, the oscillator [energy](energy.md) increases at rate $\varepsilon(y')^4$. The [amplitude-phase equations](#amplitude-phase-equations-for-a-weakly-perturbed-oscillator) give $R(T)=R_0(1-3R_0^2T/4)^{-1/2}$. The [weakly nonlinear expansion](#weakly-nonlinear-expansion) fails when the growing amplitude makes $\varepsilon R^2$ large, so its formal finite-time divergence does not itself control the exact late-time trajectory.

#### Conservative forcing in averaged oscillator equations

↑ **Parent:** [Amplitude-phase equations for a weakly perturbed oscillator](#amplitude-phase-equations-for-a-weakly-perturbed-oscillator)

For a weak force depending only on [position](classical-mechanics.md#position), the amplitude average is a periodic total [derivative](calculus.md#derivative) and vanishes. The leading harmonic amplitude is constant, while the phase may drift. The [method of multiple scales](#method-of-multiple-scales) agrees with the exact [conservation of energy](mathematical-physics.md#conservation-of-energy) for bounded orbits in the effective potential. A cubic [position](classical-mechanics.md#position) force on the right side of the oscillator equation lowers the [frequency](wave.md#frequency) at first order when its coefficient is positive.

### Slow time

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

A slow time resolves evolution occurring over many periods of a faster process. It is treated as an independent variable in the [method of multiple scales](#method-of-multiple-scales).

### Weakly nonlinear expansion

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

A weakly nonlinear expansion writes a small disturbance as powers of an amplitude parameter while resolving its evolution on a [slow time](#slow-time). Near a critical [eigenvalue](linear-operator-theory.md#eigenvalue), linear detuning and nonlinear interactions enter the same perturbation order. The [Fredholm solvability condition for a self-adjoint operator](linear-operator-theory.md#fredholm-solvability-condition-for-a-self-adjoint-operator), or its adjoint form for a general operator, yields an [amplitude equation](bifurcation-theory.md#amplitude-equation) without requiring the full higher-order correction.

#### Quadratic wave interaction

↑ **Parent:** [Weakly nonlinear expansion](#weakly-nonlinear-expansion)

A quadratic product of [plane waves](wave-function.md#plane-wave) generates sums and differences of their [wavenumbers](wave-equation.md#wavenumber) and [angular frequencies](lagrangian-mechanics.md#angular-frequency). A component drives a [secular term](#secular-term) when its generated pair also satisfies the linear [dispersion relation](dispersion-relation.md). A [solvability condition in the method of multiple scales](#solvability-condition-in-the-method-of-multiple-scales) then determines the coupled [amplitude equations](bifurcation-theory.md#amplitude-equation) on a [slow time](#slow-time).

##### Resonant three-wave triad

↑ **Parent:** [Quadratic wave interaction](#quadratic-wave-interaction)

Three [Fourier modes](fourier-analysis.md#fourier-mode) form a spatial resonance when their wavevectors sum to zero. Products of the conjugate second and third modes then force the first mode, with cyclic counterparts. Such terms couple both amplitudes and phases, unlike self-saturation terms proportional only to squared magnitudes. For three equal [wavenumbers](wave-equation.md#wavenumber), the vectors are separated by $120$ degrees and support hexagonal pattern interactions.

##### Detuning of a wave resonance

↑ **Parent:** [Quadratic wave interaction](#quadratic-wave-interaction)

Detuning measures the small mismatch from a [resonance condition](linear-ordinary-differential-equation.md#resonance-condition). When the mismatch and nonlinear forcing are both $O(\epsilon)$, they enter the same [slow time](#slow-time) equation. A small shift of the [wavenumber](wave-equation.md#wavenumber) can therefore balance a quadratic interaction and permit a locked periodic [travelling wave](analysis.md#travelling-wave).

##### Phase matching for a quadratic wave interaction

↑ **Parent:** [Quadratic wave interaction](#quadratic-wave-interaction)

A resonant interaction requires matching both [wavenumber](wave-equation.md#wavenumber) and [angular frequency](lagrangian-mechanics.md#angular-frequency): $k_3=k_1+k_2$ and $\omega_3=\omega_1+\omega_2$ for a sum interaction, with corresponding sign changes for differences. A common [phase velocity](dispersion-relation.md#phase-velocity) alone does not guarantee that a generated harmonic lies on the [dispersion relation](dispersion-relation.md).

###### Two-to-one resonance of dispersive waves

↑ **Parent:** [Phase matching for a quadratic wave interaction](#phase-matching-for-a-quadratic-wave-interaction)

A fundamental wave and its second harmonic satisfy [phase matching for a quadratic wave interaction](#phase-matching-for-a-quadratic-wave-interaction) when $\omega(2k)=2\omega(k)$. The square of the fundamental drives the second harmonic, while its product with the conjugate second harmonic drives the fundamental. Projecting these terms onto the resonant modes gives coupled [amplitude equations](bifurcation-theory.md#amplitude-equation) rather than a uniformly valid correction at fixed amplitude.

###### Explosive two-to-one amplitude system

↑ **Parent:** [Two-to-one resonance of dispersive waves](#two-to-one-resonance-of-dispersive-waves)

For $A_T=-\overline AB/2$ and $B_T=-A^2/4$, write $A=Re^{i\theta}$, $B=Pe^{i\phi}$ and $\delta=\phi-2\theta$. The polar equations are

$$
R_T=-\frac{RP}2\cos\delta,\qquad \theta_T=-\frac P2\sin\delta,\qquad P_T=-\frac{R^2}4\cos\delta,\qquad \phi_T=\frac{R^2}{4P}\sin\delta.
$$

Where the polar phases are defined, direct [differentiation](calculus.md#differentiation) gives the [first integrals](differential-equation.md#first-integral) $R^2-2P^2$ and $R^2P\sin\delta$. In particular $R^2\theta_T$ and $P^2\phi_T$ are constant. If $\delta=\pi$ and $R^2-2P^2=C>0$, then $P_T=P^2/2+C/4$, a [Riccati equation](analysis.md#riccati-equation) whose positive solution develops a finite-time pole. This is [finite-time blowup](differential-equation.md#finite-time-blowup) of the reduced amplitude system; it does not establish blowup of the full wave equation beyond the domain of the [weakly nonlinear expansion](#weakly-nonlinear-expansion).

### Harmonic balance

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Harmonic_balance)

Harmonic balance substitutes a finite [Fourier series](fourier-series.md) into a differential equation and projects the residual onto the retained harmonics. It determines their amplitudes and phases. A nonlinear equation generally generates additional harmonics, so vanishing of the projected residual alone does not make the finite series an exact solution. In a [weakly nonlinear expansion](#weakly-nonlinear-expansion), nonresonant generated harmonics can be found at the next order by solving their linear equations.

### Solvability condition in the method of multiple scales

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)

At each perturbation order, the coefficient of a homogeneous oscillatory mode must vanish from the forcing to prevent secular growth. This solvability condition determines the slow evolution of lower-order amplitudes.

### Parametric resonance

↑ **Parent:** [Method of multiple scales](#method-of-multiple-scales)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parametric_resonance)

Parametric resonance occurs when periodic variation of a system parameter couples oscillatory modes and produces exponential amplitude growth. Multiple-scale solvability identifies the instability tongues and their detuning widths.

#### Primary instability tongue of a weak Mathieu oscillator

↑ **Parent:** [Parametric resonance](#parametric-resonance)

For $y''+(\omega^2+\epsilon\cos t)y=0$, use the [method of multiple scales](#method-of-multiple-scales) with $T=\epsilon t$ and $y_0=a(T)\cos(t/2)+b(T)\sin(t/2)$. Removing [secular terms](#secular-term) gives $a_T=(k-1/2)b$ and $b_T=-(k+1/2)a$. The slow [eigenvalues](linear-operator-theory.md#eigenvalue) satisfy $\lambda^2=1/4-k^2$, so an exponentially growing mode exists inside the displayed leading instability interval. At its leading endpoints the slow matrix is nilpotent; higher-order corrections are needed to determine the exact edges. [Floquet theory](differential-equation.md#floquet-theory) distinguishes this exponential instability from algebraic growth at a repeated multiplier.

#### Primary parametric resonance of a two-to-one oscillator pair

↑ **Parent:** [Parametric resonance](#parametric-resonance)

For weak quadratic coupling between [frequencies](wave.md#frequency) one and two, the first oscillator's [complex amplitude](wave.md#complex-amplitude) can obey $2iA_T+\alpha A+b\overline A=0$ with a constant real second-oscillator amplitude $b$. In real coordinates this is a linear slow system with squared growth rate $(b^2-\alpha^2)/4$. Exponential amplification occurs when the modulation amplitude exceeds detuning, $|b|>|\alpha|$. The [method of multiple scales](#method-of-multiple-scales) is valid over bounded slow time while the physical amplitudes remain in the weak-coupling regime. At equality the slow matrix can have a [Jordan block](linear-operator-theory.md#jordan-block) and produce linear growth for some initial phases.

#### Second instability tongue of a weak Mathieu oscillator

↑ **Parent:** [Parametric resonance](#parametric-resonance)

For $u''+[1+\epsilon\sin t+\epsilon^2f]u=0$, the second parametric-instability tongue is $-1/12<f<5/12$ to leading order. Outside its closure every leading slow amplitude is oscillatory.

##### Slow amplitudes for the second Mathieu instability tongue

↑ **Parent:** [Second instability tongue of a weak Mathieu oscillator](#second-instability-tongue-of-a-weak-mathieu-oscillator)

For $x''+[1+\epsilon\cos t+f\epsilon^2]x=0$, let $T=\epsilon^2t$ and $x_0=a(T)\cos t+b(T)\sin t$. First-order forcing produces a constant and second harmonics, not a resonant harmonic. Their feedback at second order gives the displayed [solvability condition in the method of multiple scales](#solvability-condition-in-the-method-of-multiple-scales). The slow squared growth rate is $(f+1/12)(5/12-f)/4$. Consequently the leading instability interval is $-1/12<f<5/12$; outside its closure the slow amplitudes oscillate. The endpoints are degenerate and require the [fourth-order edges of the second Mathieu instability tongue](#fourth-order-edges-of-the-second-mathieu-instability-tongue) for exact small-parameter stability.

##### Fourth-order edges of the second Mathieu instability tongue

↑ **Parent:** [Second instability tongue of a weak Mathieu oscillator](#second-instability-tongue-of-a-weak-mathieu-oscillator)

For $u''+[1+k\epsilon^2+\epsilon\cos t]u=0$, set $t=2s$. The [Mathieu equation](linear-ordinary-differential-equation.md#mathieu-equation) has $a=4+4k\epsilon^2$ and $q=-2\epsilon$. Near the value $4$, the orthonormal even [Fourier series](fourier-series.md) basis $1,\cos2s,\cos4s,\cos6s$ gives diagonal entries $0,4,16,36$ and adjacent couplings $\sqrt2q,q,q$. The odd basis $\sin2s,\sin4s,\sin6s$ gives diagonal entries $4,16,36$ and adjacent couplings $q,q$. Higher modes require at least six coupling steps to affect the root near $4$, so these truncations determine its coefficients through $q^4$.

Substituting $a=4+c_2q^2+c_4q^4$ into the two [characteristic polynomials](linear-operator-theory.md#characteristic-polynomial) and equating coefficients yields

$$
a_2=4+\frac5{12}q^2-\frac{763}{13824}q^4+O(q^6),\qquad
b_2=4-\frac1{12}q^2+\frac5{13824}q^4+O(q^6).
$$

Converting back gives the displayed gap edges with remainders $O(\epsilon^4)$ in $k$. In a fixed bounded neighborhood of this [parametric resonance](#parametric-resonance), the true unstable gap is $k_-<k<k_+$. The leading slow-amplitude calculation cannot decide exact stability at $k=-1/12$ or $5/12$; the fourth-order shifts put those fixed values just outside the gap for sufficiently small positive $\epsilon$. This does not provide a bound uniform in $\epsilon$ for their transient amplification.

## ↑ Ancestors (6)

1. [Ordinary differential equation](differential-equation.md#ordinary-differential-equation)
2. [Differential equation](differential-equation.md)
3. [Analysis](analysis.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (15)

- [Additive composite expansion](#additive-composite-expansion)
- [Boundary layer](continuum-mechanics.md#boundary-layer)
- [Divergent algebraic root in a singular perturbation](asymptotic-expansion.md#divergent-algebraic-root-in-a-singular-perturbation)
- [Gaussian drift primitives](integral.md#gaussian-drift-primitives)
- [Inner variable](#inner-variable)
- [Matched asymptotic expansion](#matched-asymptotic-expansion)
- [Outer expansion](#outer-expansion)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-50.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-48.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-76.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-67.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4.md#6c/c/solution)
- [Regular perturbation](asymptotic-expansion.md#regular-perturbation)
- [Singular perturbation](singular-perturbation.md)
- [Square-root-degenerate endpoint layer](#square-root-degenerate-endpoint-layer)
