# Continuous probability distribution

↑ **Parent:** [Probability distribution](probability-theory.md#probability-distribution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Continuous_probability_distribution)

A continuous probability distribution is described by a density with respect to Lebesgue measure.

**Table of contents**

- [Distance between two uniform points in a three-dimensional ball](#distance-between-two-uniform-points-in-a-three-dimensional-ball)
- [Beta-prime distribution](#beta-prime-distribution)
- [Triangular distribution](#triangular-distribution)
- [Arcsine distribution](#arcsine-distribution)
- [Log-uniform distribution](#log-uniform-distribution)
- [Pareto distribution](#pareto-distribution)
  - [One-big-jump polynomial lower bound](#one-big-jump-polynomial-lower-bound)
- [Rayleigh distribution](#rayleigh-distribution)
- [Hypoexponential distribution](#hypoexponential-distribution)
  - [Sum of exponential variables with linearly increasing rates](#sum-of-exponential-variables-with-linearly-increasing-rates)
  - [Conditional split of two exponential times](#conditional-split-of-two-exponential-times)
- [Student's t-distribution](#student-s-t-distribution)
  - [Normal scale mixture representation of Student t](#normal-scale-mixture-representation-of-student-t)
  - [Noncentral t-distribution](#noncentral-t-distribution)
- [F-distribution](#f-distribution)
- [Probability density function](#probability-density-function)
  - [Central angle between independent uniform sphere points](#central-angle-between-independent-uniform-sphere-points)
    - [Connectivity of three acute-angle sphere points](#connectivity-of-three-acute-angle-sphere-points)
    - [Pairwise acute central angles of three uniform sphere points](#pairwise-acute-central-angles-of-three-uniform-sphere-points)
  - [Normalizing constant](#normalizing-constant)
  - [Density ratio](#density-ratio)
  - [Log-concave probability density](#log-concave-probability-density)
  - [Lipschitz density height bound](#lipschitz-density-height-bound)
  - [Joint probability density](#joint-probability-density)
  - [Change-of-variables formula for a probability density](#change-of-variables-formula-for-a-probability-density)
- [Gamma distribution](#gamma-distribution)
  - [Shifted gamma distribution](#shifted-gamma-distribution)
  - [Beta-gamma independence](#beta-gamma-independence)
  - [Additivity of independent gamma distributions with a common rate](#additivity-of-independent-gamma-distributions-with-a-common-rate)
  - [Gamma exponential dispersion family](#gamma-exponential-dispersion-family)
  - [Cumulant-generating function of a gamma distribution](#cumulant-generating-function-of-a-gamma-distribution)
  - [Inverse-gamma distribution](#inverse-gamma-distribution)
    - [Gamma prior for an inverse-gamma scale](#gamma-prior-for-an-inverse-gamma-scale)
  - [Erlang distribution](#erlang-distribution)
  - [Sampling an integer-shape gamma distribution](#sampling-an-integer-shape-gamma-distribution)
- [Dirichlet distribution](#dirichlet-distribution)
- [Exponential distribution](#exponential-distribution)
  - [Slow exponential plus an exponential sample mean](#slow-exponential-plus-an-exponential-sample-mean)
  - [Maximum of two exponentials as a scaled sum](#maximum-of-two-exponentials-as-a-scaled-sum)
  - [Integer and fractional parts of an exponential variable](#integer-and-fractional-parts-of-an-exponential-variable)
  - [Laplace transform of an exponential distribution](#laplace-transform-of-an-exponential-distribution)
  - [Memorylessness of the exponential distribution](#memorylessness-of-the-exponential-distribution)
  - [Uniform ratio of independent exponential variables](#uniform-ratio-of-independent-exponential-variables)
  - [Competing exponential clocks](#competing-exponential-clocks)
  - [Geometric sum of exponential variables](#geometric-sum-of-exponential-variables)
- [Continuous uniform distribution](#continuous-uniform-distribution)
  - [Coverage of antipodal points by a randomly oriented sector](#coverage-of-antipodal-points-by-a-randomly-oriented-sector)
  - [Random quadratic with uniform coefficients](#random-quadratic-with-uniform-coefficients)
  - [Uniform random variable](#uniform-random-variable)
  - [Steinhaus random variable](#steinhaus-random-variable)
    - [Steinhaus first-moment lower bound](#steinhaus-first-moment-lower-bound)
  - [Squared uniform distribution](#squared-uniform-distribution)
  - [Sum of two independent uniform variables](#sum-of-two-independent-uniform-variables)
  - [Uniform split of a random total](#uniform-split-of-a-random-total)
    - [Exponential characterization by a uniform random split](#exponential-characterization-by-a-uniform-random-split)
- [Laplace distribution](#laplace-distribution)
  - [Laplace prior for sparse images](#laplace-prior-for-sparse-images)
  - [Laplace regression](#laplace-regression)

## Distance between two uniform points in a three-dimensional ball

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution.md)

For two [independent random variables](random-variable.md#independent-random-variables) taking values in a three-dimensional [ball](topological-analysis.md#ball-mathematics) with constant volume [probability density](quantum-mechanics.md#probability-density), the density of their distance is the displayed expression for $0\leq r\leq2R$, and zero otherwise. Both [independence](random-variable.md#independent-random-variables) and the common radius $R>0$ are essential. To derive it, put $u=|\mathbf r_1|$, $v=|\mathbf r_2|$ and integrate the product volume [differential form](differential-form.md) over orientations. The [law of cosines](geometry-and-topology.md#law-of-cosines) gives the angular [Jacobian determinant](calculus.md#jacobian-determinant) $v/(ur)$, leaving $f_R(r)=9r\int uv\,du\,dv/(2R^6)$ over $0\leq u,v\leq R$, $|u-v|\leq r\leq u+v$. With $x=u+v$, $y=u-v$, the integrand becomes $(x^2-y^2)\,dx\,dy/8$. Direct integration gives $\int uv\,du\,dv=2R^3r/3-R^2r^2/2+r^4/24$. An independent geometric derivation uses the overlap volume of two radius-$R$ balls displaced by $r$, namely $\pi(4R+r)(2R-r)^2/12$, multiplied by $4\pi r^2$ and divided by the square of $4\pi R^3/3$. The density integrates to one and has mean $36R/35$.

## Beta-prime distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution.md)

For $a,b>0$, this [probability density function](#probability-density-function) is obtained from a [Beta distribution](probability-theory.md#beta-distribution) variable $U$ by $X=U/(1-U)$. Indeed $u=x/(1+x)$ and $du/dx=(1+x)^{-2}$, and the [change of variables formula](calculus.md#change-of-variables-formula) gives the displayed density. In particular, the ratio of two [independent](random-variable.md#independent-random-variables) equal-rate [exponential distributions](#exponential-distribution) has $a=b=1$, density $(1+x)^{-2}$ and [cumulative distribution function](probability-theory.md#cumulative-distribution-function) $x/(1+x)$.

## Triangular distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Triangular_distribution)

A triangular [probability density function](#probability-density-function) rises linearly from zero at $a$ to its mode $c$, then falls linearly to zero at $b$. Its peak is $2/(b-a)$. Its [inverse transform sampling](probability-theory.md#inverse-transform-sampling) rule is $a+\sqrt{u(b-a)(c-a)}$ for $u\le(c-a)/(b-a)$, and $b-\sqrt{(1-u)(b-a)(b-c)}$ otherwise.

## Arcsine distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Arcsine_distribution)

The standard arcsine law has [probability density function](#probability-density-function) $1/[\pi\sqrt{x(1-x)}]$ on $(0,1)$. Substituting $x=\sin^2v$ in its integral gives [cumulative distribution function](probability-theory.md#cumulative-distribution-function) $F(x)=2\arcsin\sqrt{x}/\pi$. Hence [inverse transform sampling](probability-theory.md#inverse-transform-sampling) uses $X=\sin^2(\pi U/2)$ for $U$ with a continuous [uniform distribution](#continuous-uniform-distribution). The law places most of its density near the two endpoints rather than the middle.

## Log-uniform distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution.md)

For $0<A<B<\infty$, this density makes $\log X$ uniform between $\log A$ and $\log B$. It is a proper finite-interval version of the [scale-invariant prior](statistical-inference.md#scale-invariant-prior). The chosen logarithm base changes only the endpoint coordinates.

## Pareto distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution.md)

In the shape–minimum parameterization, the density is $\alpha\beta^\alpha x^{-\alpha-1}\mathbf1_{\{x>\beta\}}$, with $\alpha,\beta>0$. The survival function is $(\beta/x)^\alpha$ for $x\ge\beta$. Large shape concentrates the distribution near its lower bound. This convention is useful for [uniform-Pareto conjugacy](exponential-family.md#uniform-pareto-conjugacy).

### One-big-jump polynomial lower bound

↑ **Parent:** [Pareto distribution](#pareto-distribution)

For nonnegative [independent](random-variable.md#independent-random-variables) identically distributed summands with polynomial upper tail $\mathbb P(X_1\geq x)=x^{-\beta}$ for $x\geq1$, positivity gives $\mathbb P(S_n\geq na)\geq(na)^{-\beta}$ for fixed $a>0$ and large $n$. Since this [probability](probability-theory.md#probability) is also at most one, its logarithm divided by $n$ tends to zero. No positive exponential moment exists, so the exponential-moment form of the [Cramér theorem](probability-theory.md#cramer-s-theorem) cannot be applied. The bound proves a logarithmic rate and does not assert an exact tail asymptotic.

## Rayleigh distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution.md)

At unit scale the [probability density function](#probability-density-function) is $r\exp(-r^2/2)$ for $r>0$. Its square has an [exponential distribution](#exponential-distribution) of rate $1/2$. Thus $\sqrt{-2\log U}$ has this distribution for a [uniform distribution](#continuous-uniform-distribution) variable $U$ on $(0,1)$.

## Hypoexponential distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hypoexponential_distribution)

A hypoexponential distribution is the distribution of a sum of [independent](random-variable.md#independent-random-variables) variables with [exponential distributions](#exponential-distribution). For two positive unequal rates $\lambda,\mu$, [convolution of independent random variables](probability-theory.md#convolution-of-independent-random-variables) gives the [probability density function](#probability-density-function)

$$
f(s)=\frac{\lambda\mu}{\mu-\lambda}(e^{-\lambda s}-e^{-\mu s}),\qquad s\geq0.
$$

It is zero for negative $s$. Its equal-rate limit is the shape-two [gamma distribution](#gamma-distribution) with rate $\lambda$.

### Sum of exponential variables with linearly increasing rates

↑ **Parent:** [Hypoexponential distribution](#hypoexponential-distribution)

If the [independent](random-variable.md#independent-random-variables) [exponential random variables](#exponential-distribution) $T_i$ have rates $i\lambda$, then

$$
\sum_{i=1}^N T_i\ \overset{d}{=}\ \max_{1\leq i\leq N}E_i,\qquad
\mathbb P\!\left(\sum_{i=1}^NT_i\leq t\right)=(1-e^{-\lambda t})^N\quad(t\geq0),
$$

where the $E_i$ are [independent](random-variable.md#independent-random-variables) [exponential random variables](#exponential-distribution) of rate $\lambda$. To see this, the first of $N$ independent exponential clocks rings at rate $N\lambda$; after it rings, the [memoryless property](#memorylessness-of-the-exponential-distribution) leaves $N-1$ independent rate-$\lambda$ clocks. The successive [order statistic](probability-theory.md#order-statistic) gaps are therefore independent with rates $N\lambda,(N-1)\lambda,\ldots,\lambda$. Their sum has the same distribution as $\sum T_i$. In particular, for $x>0$, the tail at $Nx$ has logarithm $-\lambda Nx+o(N)$, since $1-(1-e^{-\lambda Nx})^N\sim N e^{-\lambda Nx}$. The sum divided by $N$ has a [large deviation principle](convergence-of-random-variables.md#large-deviation-principle) with speed $N$ and [rate function](convergence-of-random-variables.md#rate-function) $\lambda x$ on $x\geq0$, infinity otherwise.

### Conditional split of two exponential times

↑ **Parent:** [Hypoexponential distribution](#hypoexponential-distribution)

For [independent](random-variable.md#independent-random-variables) [exponential distributions](#exponential-distribution) with rates $\lambda_1>\lambda_2>0$, let $T=S_1+S_2$. Dividing the joint density of $(S_1,T)$ by the [hypoexponential distribution](#hypoexponential-distribution) density of $T$ gives a [truncated exponential distribution](probability-theory.md#truncated-exponential-distribution) on $(0,t)$ with rate $\lambda_1-\lambda_2$. Its displayed [conditional expectation](measure-theory.md#conditional-expectation) supplies an E-step when only pair totals are observed. At equal rates the conditional split is uniform, with mean $t/2$.

// Target: probability-and-statistics.bigb

<h2 id="student-s-t-distribution">Student's t-distribution</h2>

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Student's_t-distribution)

Student's t-distribution with $\nu$ degrees of freedom is the distribution of $Z/\sqrt{V/\nu}$ for independent $Z\sim N(0,1)$ and $V\sim\chi^2_\nu$.

### Normal scale mixture representation of Student t

↑ **Parent:** [Student's t-distribution](#student-s-t-distribution)

For independent $Z\sim N(0,1)$ and $\Lambda\sim\chi_\nu^2$, the displayed ratio has the [Student t-distribution](#student-s-t-distribution) with $\nu$ degrees of freedom. Equivalently, $T\mid\Lambda\sim N(0,\nu/\Lambda)$. Integrating the normal conditional density against the [chi-squared distribution](probability-theory.md#chi-squared-distribution) gives a density proportional to $(1+t^2/\nu)^{-(\nu+1)/2}$. A latent scale therefore supplies heavy tails while retaining convenient normal conditional calculations. For $\nu>2$, its variance is $\nu/(\nu-2)$, so its scale parameter is not its standard deviation.

### Noncentral t-distribution

↑ **Parent:** [Student's t-distribution](#student-s-t-distribution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Noncentral_t-distribution)

If $Z\sim N(0,1)$ and $U\sim\chi^2_\nu$ are [independent](random-variable.md#independent-random-variables), then $(Z+\delta)/\sqrt{U/\nu}$ has the noncentral t-distribution with [degrees of freedom](classical-mechanics.md#degree-of-freedom) $\nu$ and noncentrality $\delta$. It describes the [test statistic](statistical-modelling.md#test-statistic) of a [Student's t-test](statistical-modelling.md#student-s-t-test) under a shifted alternative.

## F-distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/F-distribution)

The F-distribution with degrees of freedom $(d_1,d_2)$ is the distribution of $(U_1/d_1)/(U_2/d_2)$ for independent chi-squared random variables $U_1\sim\chi^2_{d_1}$ and $U_2\sim\chi^2_{d_2}$.

## Probability density function

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Probability_density_function)

A probability density function is a nonnegative measurable function $f_X$ satisfying

$$
\mathbb P(X\in A)=\int_A f_X(x)\,dx.
$$

Its integral over the whole sample space is one.

### Central angle between independent uniform sphere points

↑ **Parent:** [Probability density function](#probability-density-function)

For two independent uniform points on the surface of a [sphere](geometry-and-topology.md#sphere), rotational invariance permits fixing the first at the north pole. The [surface area](differential-geometry.md#surface-area) of a latitude band of angular width $d\theta$ is $2\pi R^2\sin\theta\,d\theta$, yielding the displayed density for their central angle. Equivalently their unit position [vectors](vector-space.md#vector) have a [dot product](linear-algebra.md#dot-product) uniformly distributed on $[-1,1]$. The law is independent of sphere radius.

#### Connectivity of three acute-angle sphere points

↑ **Parent:** [Central angle between independent uniform sphere points](#central-angle-between-independent-uniform-sphere-points)

Join three independent uniform points on a [sphere](geometry-and-topology.md#sphere) when their central angle is acute. Given angle $\gamma$ between the first pair, the third point's two favorable [hemispheres](geometry-and-topology.md#hemisphere) overlap in a [spherical lune](geometry-and-topology.md#spherical-lune) of area fraction $(\pi-\gamma)/(2\pi)$. If $\gamma<\pi/2$, connection requires membership in their union, of probability $1/2+\gamma/(2\pi)$. If $\gamma>\pi/2$, it requires membership in their intersection, of probability $1/2-\gamma/(2\pi)$. Integrating these against the central-angle density $\sin\gamma/2$ proves the displayed probability. Connectivity is weaker than all three pairwise angles being acute.

#### Pairwise acute central angles of three uniform sphere points

↑ **Parent:** [Central angle between independent uniform sphere points](#central-angle-between-independent-uniform-sphere-points)

For three independent uniform points on a [sphere](geometry-and-topology.md#sphere), condition on the central angle $\theta$ between the first two. The third point makes acute angles with both exactly when it lies in the intersection of their positive [hemispheres](geometry-and-topology.md#hemisphere). That intersection is a [spherical lune](geometry-and-topology.md#spherical-lune) of opening $\pi-\theta$, hence has probability $(\pi-\theta)/(2\pi)$. The first two points also need $\theta<\pi/2$. Integrating against the [central angle between independent uniform sphere points](#central-angle-between-independent-uniform-sphere-points) density gives $(4\pi)^{-1}\int_0^{\pi/2}(\pi-\theta)\sin\theta\,d\theta=(\pi-1)/(4\pi)$.

### Normalizing constant

↑ **Parent:** [Probability density function](#probability-density-function)

A [normalizing constant](#normalizing-constant) makes a nonnegative integrable [function](function.md) into a [probability density function](#probability-density-function): if $0<Z=\int h<\infty$, then $h/Z$ is a [probability density function](#probability-density-function).

### Density ratio

↑ **Parent:** [Probability density function](#probability-density-function)

A [density ratio](#density-ratio) compares two [probability density functions](#probability-density-function) relative to the same underlying [measure](measure-theory.md#measure). More generally it is a [Radon-Nikodym derivative](measure-theory.md#radon-nikodym-derivative) when one [probability measure](probability-theory.md#probability-measure) has [absolute continuity of measures](measure-theory.md#absolute-continuity-of-measures) with respect to the other.

### Log-concave probability density

↑ **Parent:** [Probability density function](#probability-density-function)

A probability density is log-concave when its logarithm is a [concave function](real-analysis.md#concave-function) on its support. Tangent lines to a differentiable concave log density lie above its graph, giving exponential envelopes for [rejection sampling](probability-and-statistics.md#rejection-sampling).

### Lipschitz density height bound

↑ **Parent:** [Probability density function](#probability-density-function)

For a [probability density function](#probability-density-function) $f$ on $\mathbb R$ with [Lipschitz bound](real-analysis.md#lipschitz-bound) $L>0$, the triangular lower envelope $f(x+u)\geq(f(x)-L|u|)_+$ gives $f(x)^2\leq L$. If $f$ is strictly positive everywhere, the inequality is strict. Equality forces the entire [probability density function](#probability-density-function) to coincide with the triangular envelope, which vanishes outside a finite interval.

### Joint probability density

↑ **Parent:** [Probability density function](#probability-density-function)

A joint probability density $f_{X,Y}$ satisfies

$$
\mathbb P((X,Y)\in A)=\iint_A f_{X,Y}(x,y)\,dx\,dy.
$$

Its coordinate integrals are the [marginal densities](probability-theory.md#marginal-distribution), and integrating it over a rectangle gives the corresponding [joint distribution function](probability-theory.md#joint-distribution-function).

### Change-of-variables formula for a probability density

↑ **Parent:** [Probability density function](#probability-density-function)

If $Y=g(X)$ for a differentiable bijection, then

$$
f_Y(y)=f_X(g^{-1}(y))\left|\det Dg^{-1}(y)\right|.
$$

This is the [change of variables formula](calculus.md#change-of-variables-formula) applied to probability density.

## Gamma distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gamma_distribution)

The gamma distribution with shape $a>0$ and rate $r>0$ has density

$$
f(x)=\frac{r^a}{\Gamma(a)}x^{a-1}e^{-rx},
\qquad x>0.
$$

### Shifted gamma distribution

↑ **Parent:** [Gamma distribution](#gamma-distribution)

A [gamma distribution](#gamma-distribution) translated by a real constant $k$. With shape $\alpha>0$ and rate $\nu>0$, its support is $(k,\infty)$ and its first three [cumulants](probability-theory.md#cumulant) are $k+\alpha/\nu$, $\alpha/\nu^2$, and $2\alpha/\nu^3$. Its [skewness](probability-theory.md#skewness) is $2/\sqrt\alpha$. A negative shift permits negative values; introducing a shift does not automatically respect the nonnegative support of an insurance loss.

### Beta-gamma independence

↑ **Parent:** [Gamma distribution](#gamma-distribution)

If $X$ and $Y$ are [independent random variables](random-variable.md#independent-random-variables) with [Gamma distributions](#gamma-distribution) of shapes $a,b>0$ and the same rate $\theta>0$, then $U=X/(X+Y)$ has the [Beta distribution](probability-theory.md#beta-distribution) with parameters $(a,b)$, and $V=X+Y$ has the [Gamma distribution](#gamma-distribution) of shape $a+b$ and rate $\theta$. Moreover $U$ and $V$ are independent. The inverse [change of variables](calculus.md#change-of-variables-formula) $(x,y)=(uv,(1-u)v)$ has absolute [Jacobian determinant](calculus.md#jacobian-determinant) $v$, which makes the [joint probability density](#joint-probability-density) factorize on the product domain $0<u<1$, $v>0$. The common rate is essential for this factorization.

### Additivity of independent gamma distributions with a common rate

↑ **Parent:** [Gamma distribution](#gamma-distribution)

If independent random variables $X_i$ have [gamma distributions](#gamma-distribution) with shapes $a_i$ and one common rate $r$, then

$$
\sum_{i=1}^nX_i\sim\operatorname{Gamma}\left(\sum_{i=1}^na_i,r\right).
$$

Their [Laplace transforms of nonnegative random variables](probability-theory.md#laplace-transform-of-a-nonnegative-random-variable) multiply to $(r/(r+s))^{\sum_i a_i}$, which is the transform of the displayed gamma distribution; uniqueness of the Laplace transform proves the claim.

### Gamma exponential dispersion family

↑ **Parent:** [Gamma distribution](#gamma-distribution)

Writing $\phi=1/a$, $\theta=-r/a<0$, and $b(\theta)=-\log(-\theta)$ puts the gamma density into [exponential dispersion family](exponential-family.md#exponential-dispersion-model) form

$$
f(y;\theta,\phi)=a(y,\phi)
\exp\left(\frac{y\theta-b(\theta)}{\phi}\right),
\qquad
a(y,\phi)=\frac{y^{1/\phi-1}}{\Gamma(1/\phi)\phi^{1/\phi}}.
$$

Its mean is $a/r$ and its variance is $a/r^2$.

### Cumulant-generating function of a gamma distribution

↑ **Parent:** [Gamma distribution](#gamma-distribution)

For a gamma random variable of shape $a$ and rate $r$,

$$
K_Y(t)=\log\mathbb E[e^{tY}]
=-a\log\left(1-\frac tr\right),
\qquad t<r.
$$

### Inverse-gamma distribution

↑ **Parent:** [Gamma distribution](#gamma-distribution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse-gamma_distribution)

An inverse-gamma random variable is the reciprocal of a [gamma distribution](#gamma-distribution) random variable up to scale. In shape-scale parameters its density is proportional to $x^{-a-1}e^{-b/x}$ on $x>0$.

#### Gamma prior for an inverse-gamma scale

↑ **Parent:** [Inverse-gamma distribution](#inverse-gamma-distribution)

For [inverse-gamma distribution](#inverse-gamma-distribution) observations of known shape $k$ and scale $\Theta$, their [likelihood function](statistical-modelling.md#likelihood-function) in $\Theta$ is proportional to $\Theta^{nk}\exp(-\Theta\sum_i x_i^{-1})$. A shape-$\alpha$, rate-$\lambda$ [gamma distribution](#gamma-distribution) [conjugate prior](exponential-family.md#conjugate-prior) therefore gives the displayed [Bayesian posterior](statistical-inference.md#bayesian-posterior). The [Bayes estimator under squared error loss](statistical-inference.md#bayes-estimator-under-squared-error-loss) of the conditional claim [expected value](probability-theory.md#expected-value) $\Theta/(k-1)$ is $(\alpha+nk)/[(k-1)(\lambda+\sum_i x_i^{-1})]$. It depends on reciprocals, rather than the [sample mean](variance.md#sample-mean) of the claims.

### Erlang distribution

↑ **Parent:** [Gamma distribution](#gamma-distribution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Erlang_distribution)

The sum of $n$ independent exponential variables of rate $r$ has the Erlang distribution with density

$$
f_n(x)=\frac{r^nx^{n-1}}{(n-1)!}e^{-rx},
\qquad x>0.
$$

Convolving with one more exponential proves the formula inductively.

### Sampling an integer-shape gamma distribution

↑ **Parent:** [Gamma distribution](#gamma-distribution)

If $m$ is a positive integer and $U_1,\ldots,U_m$ are independent uniform variables, then

$$
-\frac1r\sum_{j=1}^m\log U_j
$$

has the gamma distribution with shape $m$ and rate $r$, because each summand is exponential with rate $r$.

## Dirichlet distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirichlet_distribution)

The Dirichlet distribution is a probability distribution on vectors $(p_1,\ldots,p_K)$ with nonnegative entries summing to one and density proportional to $\prod_kp_k^{\alpha_k-1}$.

## Exponential distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exponential_distribution)

The exponential distribution with rate $c>0$ has density

$$
f(x)=ce^{-cx}\mathbf 1_{\{x\geq0\}}.
$$

It is the gamma distribution with shape one.

### Slow exponential plus an exponential sample mean

↑ **Parent:** [Exponential distribution](#exponential-distribution)

Let $S$ be a fixed sum of [independent](random-variable.md#independent-random-variables) [exponential random variables](#exponential-distribution) with smallest rate $\lambda>0$, and let $Z_N$ be the sum of $N-k$ independent rate-$r$ [exponential random variables](#exponential-distribution), independent of $S$, with fixed $k$ and $r>\lambda$. At [large-deviation speed](convergence-of-random-variables.md#large-deviation-speed) $N$, $S/N$ has [rate function](convergence-of-random-variables.md#rate-function) $\lambda y$ for $y\geq0$; the sample mean has [rate function](convergence-of-random-variables.md#rate-function) $K_r(z)=rz-1-\log(rz)$ for $z>0$. The [product large-deviation principle](convergence-of-random-variables.md#product-large-deviation-principle) and [contraction principle for large deviations](convergence-of-random-variables.md#contraction-principle-for-large-deviations) give

$$
I(x)=\inf_{0<z\leq x}\{\lambda(x-z)+rz-1-\log(rz)\}
=\begin{cases}
rx-1-\log(rx),&0<x\leq(r-\lambda)^{-1},\\
\lambda x+\log((r-\lambda)/r),&x\geq(r-\lambda)^{-1},\\
\infty,&x\leq0.
\end{cases}
$$

Indeed the derivative of the quantity minimized with respect to $z$ is $r-\lambda-1/z$. Its minimizer is $\min(x,(r-\lambda)^{-1})$. Beyond that transition, a single slow [exponential random variable](#exponential-distribution) carries the extra excursion; the [rate function](convergence-of-random-variables.md#rate-function) becomes affine.

### Maximum of two exponentials as a scaled sum

↑ **Parent:** [Exponential distribution](#exponential-distribution)

For independent [exponential random variables](#exponential-distribution) $X,Y$ with the same rate $\lambda>0$, the [convolution](fourier-analysis.md#convolution) density of $X+Y/2$ is $2\lambda(e^{-\lambda v}-e^{-2\lambda v})$ for $v>0$. The [cumulative distribution function](probability-theory.md#cumulative-distribution-function) of $\max(X,Y)$ is $(1-e^{-\lambda v})^2$, whose derivative is the same density. This is equality of [probability distributions](probability-theory.md#probability-distribution), not an almost-sure equality of the two expressions formed from the same sample.

### Integer and fractional parts of an exponential variable

↑ **Parent:** [Exponential distribution](#exponential-distribution)

For exponential rate $\lambda>0$, the integer part has mass $(1-e^{-\lambda})e^{-\lambda m}$ on nonnegative integers. The fractional part has density $\lambda e^{-\lambda u}/(1-e^{-\lambda})$ for $0\leq u<1$. The mixed joint density factors into those marginals, proving [independence](random-variable.md#independent-random-variables). The integer part is a [geometric distribution](discrete-probability-distribution.md#geometric-distribution) on zero-based support, with [expectation](probability-theory.md#expected-value) $1/(e^\lambda-1)$.

### Laplace transform of an exponential distribution

↑ **Parent:** [Exponential distribution](#exponential-distribution)

If $X\sim\operatorname{Exp}(\lambda)$, then direct integration gives

$$
\mathbb E[e^{-sX}]=\frac{\lambda}{\lambda+s},
\qquad \operatorname{Re}s>-\lambda.
$$

### Memorylessness of the exponential distribution

↑ **Parent:** [Exponential distribution](#exponential-distribution)

If $T\sim\operatorname{Exp}(\mu)$, then

$$
\mathbb P(T>s+t\mid T>s)=\mathbb P(T>t)=e^{-\mu t}.
$$

Thus an exponential remaining lifetime has the same law regardless of the elapsed lifetime.

### Uniform ratio of independent exponential variables

↑ **Parent:** [Exponential distribution](#exponential-distribution)

If $A$ and $B$ are independent exponential variables with the same rate, then $A/(A+B)$ is uniform on $(0,1)$ and is independent of $A+B$.

### Competing exponential clocks

↑ **Parent:** [Exponential distribution](#exponential-distribution)

For independent exponential variables $S_i$ of rates $q_i$ and $Q=\sum_iq_i$, let $T=\min_iS_i$ and let $K$ be the minimizing index. Then

$$
\mathbb P(K=k,T\geq t)=\frac{q_k}{Q}e^{-Qt}.
$$

Consequently $T$ is exponential with rate $Q$, $\mathbb P(K=k)=q_k/Q$, and $K$ and $T$ are independent.

### Geometric sum of exponential variables

↑ **Parent:** [Exponential distribution](#exponential-distribution)

If $N$ is geometric on $\{1,2,\ldots\}$ with parameter $p$, independently of unit-rate exponential variables $S_i$, then

$$
\sum_{i=1}^NS_i
$$

is exponential with rate $p$. Its moment-generating function is $p/(p-\theta)$ for $\theta<p$.

## Continuous uniform distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Continuous_uniform_distribution)

A continuous uniform distribution has constant density on its interval of support.

### Coverage of antipodal points by a randomly oriented sector

↑ **Parent:** [Continuous uniform distribution](#continuous-uniform-distribution)

For a sector of width $\phi$ and an independent uniformly distributed central bearing, a specified bearing is covered with probability $\phi/(2\pi)$. Two antipodal bearings cannot both be covered when $\phi<\pi$. For $\phi\ge\pi$, the allowable centre arcs overlap in two components of length $\phi-\pi$, proving the displayed [conditional probability](probability-theory.md#conditional-probability). Averaging over the width's [probability density function](#probability-density-function) gives unconditional coverage probabilities.

### Random quadratic with uniform coefficients

↑ **Parent:** [Continuous uniform distribution](#continuous-uniform-distribution)

For independent $U,V$ uniform on $[0,1]$, real roots occur on $U\leq V^2$, a region of [probability](probability-theory.md#probability) $1/3$. On that region both roots are nonpositive. Both lie in $[-1,0]$ exactly when $\max(0,2V-1)\leq U\leq V^2$. Its area is $1/12$, so the conditional [probability](probability-theory.md#probability) of both absolute values being at most one is $1/4$. [Joint probability density](#joint-probability-density) integration turns algebraic [discriminant](polynomial.md#discriminant) and root constraints into simple planar areas.

### Uniform random variable

↑ **Parent:** [Continuous uniform distribution](#continuous-uniform-distribution)

A uniform random variable has a [uniform distribution](#continuous-uniform-distribution). Independent such variables can supply independent [inverse transform sampling](probability-theory.md#inverse-transform-sampling); reusing a single variable for two transforms generally creates dependence.

### Steinhaus random variable

↑ **Parent:** [Continuous uniform distribution](#continuous-uniform-distribution)

A Steinhaus random variable is uniformly distributed on the complex unit circle. It can be generated as $\epsilon\cos\theta+i\delta\sin\theta$ using independent signs $\epsilon,\delta$ and an independent uniform angle $\theta\in[0,\pi/2]$. This conditional sign representation transfers [Rademacher sum](probability-theory.md#rademacher-sum) inequalities to random complex phases.

#### Steinhaus first-moment lower bound

↑ **Parent:** [Steinhaus random variable](#steinhaus-random-variable)

For independent [Steinhaus random variables](#steinhaus-random-variable), condition on their acute angles and use the [sharp Rademacher second-moment inequality](fourier-analysis.md#sharp-rademacher-second-moment-inequality) on the $2d$ sign coefficients $a_i\cos\theta_i,ia_i\sin\theta_i$. Their squared moduli sum to $\sum_i|a_i|^2$ independently of the angles, so the conditional first moment is at least the same fixed square-root bound. Averaging proves the assertion.

### Squared uniform distribution

↑ **Parent:** [Continuous uniform distribution](#continuous-uniform-distribution)

The square of a [uniform distribution](#continuous-uniform-distribution) variable on $(0,1)$ has [cumulative distribution function](probability-theory.md#cumulative-distribution-function) $\sqrt{x}$ and an integrable inverse-square-root [probability density function](#probability-density-function). Reflection replaces $x$ by $1-x$ in that density.

### Sum of two independent uniform variables

↑ **Parent:** [Continuous uniform distribution](#continuous-uniform-distribution)

For independent $U_1,U_2\sim\operatorname{Uniform}(0,1)$, the sum has triangular density

$$
f(s)=
\begin{cases}
s,&0\leq s\leq1,\\
2-s,&1\leq s\leq2,\\
0,&\text{otherwise}.
\end{cases}
$$

Its upper tail for $1\leq c\leq2$ is $(2-c)^2/2$.

### Uniform split of a random total

↑ **Parent:** [Continuous uniform distribution](#continuous-uniform-distribution)

Let $X\geq0$ have density $g$, let $U$ be independent and uniform on $[0,1]$, and set

$$
Y=XU,\qquad Z=X(1-U).
$$

Then

$$
f_{Y,Z}(y,z)=\frac{g(y+z)}{y+z}\mathbf 1_{\{y,z\geq0\}},
\qquad
f_Y(y)=f_Z(y)=\int_y^\infty\frac{g(t)}t\,dt.
$$

#### Exponential characterization by a uniform random split

↑ **Parent:** [Uniform split of a random total](#uniform-split-of-a-random-total)

Write $h(y)=\int_y^\infty g(t)/t\,dt$. The two pieces in a uniform split are independent exactly when

$$
-h'(y+z)=h(y)h(z).
$$

Setting $z=0$ shows that $h(y)=ce^{-cy}$ for some $c>0$. Thus the pieces are independent exactly when they are independent exponential variables of the same rate; equivalently, the total has gamma density $c^2xe^{-cx}$.

## Laplace distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laplace_distribution)

The centred Laplace distribution with rate $\theta$ has density $\theta e^{-\theta|x|}/2$.

### Laplace prior for sparse images

↑ **Parent:** [Laplace distribution](#laplace-distribution)

Independent centered [Laplace distributions](#laplace-distribution) for pixel intensities give the [prior distribution](statistical-inference.md#prior-probability)

$$
\pi_0(u)=(\lambda/2)^d e^{-\lambda\sum_{j=1}^d|u_j|},\qquad\lambda>0.
$$

This prior favors small intensities through its sharp peak at zero, while its tails permit isolated appreciable pixels. Its negative log density is an [L1 norm](functional-analysis.md#l1-norm) penalty, so with a [Gaussian likelihood](statistical-modelling.md#gaussian-likelihood) a [maximum a posteriori estimate](statistical-inference.md#maximum-a-posteriori-estimate) minimizes a sum of squared residuals plus that penalty. A draw from this continuous prior has no exactly zero coordinate with positive probability; sparsity of a maximizing estimate and concentration of prior mass near zero are different statements. The product prior also does not encode spatial contiguity. [Inverse transform sampling](probability-theory.md#inverse-transform-sampling) produces each coordinate from an independent [uniform distribution](#continuous-uniform-distribution) by $\lambda^{-1}\log(2U)$ for $U\leq1/2$ and $-\lambda^{-1}\log(2(1-U))$ otherwise, ignoring the probability-zero endpoints.

### Laplace regression

↑ **Parent:** [Laplace distribution](#laplace-distribution)

In the model

$$
Y_i\mid X_i\sim\operatorname{Laplace}(X_i^T\beta,\sigma),
$$

maximum likelihood minimizes the sum of absolute residuals

$$
S(\beta)=\sum_i|Y_i-X_i^T\beta|.
$$

The scale estimate is $\widehat\sigma=S(\widehat\beta)/n$.

## ↑ Ancestors (6)

1. [Probability distribution](probability-theory.md#probability-distribution)
2. [Probability theory](probability-theory.md)
3. [Probability and statistics](probability-and-statistics.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (7)

- [First ascent in independent continuous observations](probability-theory.md#first-ascent-in-independent-continuous-observations)
- [Order-statistic confidence interval for a median](statistical-inference.md#order-statistic-confidence-interval-for-a-median)
- [Order symmetry of independent random variables](probability-theory.md#order-symmetry-of-independent-random-variables)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-34.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-34.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2.md#3f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4.md#19h/b/solution)
