# Gaussian process

↑ **Parent:** [Stochastic process](stochastic-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_process)

A Gaussian process is a [stochastic process](stochastic-process.md) whose every finite vector of values has a [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution). Its law is determined by its mean and covariance functions.

**Table of contents**

- [Gaussian process regression](#gaussian-process-regression)
- [Gaussian exponential martingale with deterministic variance](#gaussian-exponential-martingale-with-deterministic-variance)
- [Covariance criterion for a stationary Gaussian Markov process](#covariance-criterion-for-a-stationary-gaussian-markov-process)
- [Gaussian process construction from square-summable features](#gaussian-process-construction-from-square-summable-features)
- [Canonical pseudometric of a Gaussian process](#canonical-pseudometric-of-a-gaussian-process)
- [Fractional Brownian motion](#fractional-brownian-motion)
  - [Hurst exponent](#hurst-exponent)
- [Sudakov-Fernique inequality](#sudakov-fernique-inequality)
- [Slepian's lemma](#slepian-s-lemma)
- [Mean-square derivative of a Gaussian process](#mean-square-derivative-of-a-gaussian-process)
  - [Differentiable modification of a stationary Gaussian process](#differentiable-modification-of-a-stationary-gaussian-process)
  - [Mean-square fundamental theorem of calculus](#mean-square-fundamental-theorem-of-calculus)
- [Gaussian process classification](#gaussian-process-classification)
- [Periodic covariance function](#periodic-covariance-function)
  - [Periodic Gaussian process with zero period average](#periodic-gaussian-process-with-zero-period-average)
- [Gaussian-process marginal likelihood](#gaussian-process-marginal-likelihood)
- [Gaussian concentration inequality](#gaussian-concentration-inequality)
  - [Brownian martingale proof of Gaussian concentration](#brownian-martingale-proof-of-gaussian-concentration)
  - [Gaussian rotation interpolation inequality](#gaussian-rotation-interpolation-inequality)
- [Dudley entropy integral](#dudley-entropy-integral)
- [Borell-TIS inequality](#borell-tis-inequality)
- [Isonormal Gaussian process](#isonormal-gaussian-process)
  - [Exponential tilting of an isonormal Gaussian process](#exponential-tilting-of-an-isonormal-gaussian-process)
- [Gaussian white noise](#gaussian-white-noise)
  - [Gaussian white noise model](#gaussian-white-noise-model)
  - [White-noise likelihood for a square-integrable shift](#white-noise-likelihood-for-a-square-integrable-shift)
  - [Gaussian sequence model](#gaussian-sequence-model)
    - [Bernstein-von Mises theorem](#bernstein-von-mises-theorem)
    - [Gaussian net test](#gaussian-net-test)
    - [Gaussian least-squares contrast](#gaussian-least-squares-contrast)
- [Independent increments of a Gaussian martingale](#independent-increments-of-a-gaussian-martingale)
  - [Gaussian continuous martingale](#gaussian-continuous-martingale)
    - [Deterministic quadratic variation characterizes a Gaussian continuous local martingale](#deterministic-quadratic-variation-characterizes-a-gaussian-continuous-local-martingale)
- [Exponential covariance function](#exponential-covariance-function)
- [Gaussian random field](#gaussian-random-field)
  - [Brownian sheet](#brownian-sheet)
  - [Gaussian marginals do not imply a Gaussian random field](#gaussian-marginals-do-not-imply-a-gaussian-random-field)
  - [Centered quadratic Gaussian transformation](#centered-quadratic-gaussian-transformation)
  - [Exponential moment of a Gaussian linear functional](#exponential-moment-of-a-gaussian-linear-functional)
    - [Gaussian quadratic exponential moment](#gaussian-quadratic-exponential-moment)
  - [Stationary Gaussian random field](#stationary-gaussian-random-field)
    - [Autocorrelation function of a random field](#autocorrelation-function-of-a-random-field)
      - [Covariance of a squared random field](#covariance-of-a-squared-random-field)
  - [Novikov's theorem](#novikov-s-theorem)
  - [Markov approximation for a random medium](#markov-approximation-for-a-random-medium)
  - [Gaussian free field](#gaussian-free-field)
    - [Discrete Gaussian free field](#discrete-gaussian-free-field)
      - [Gaussian free field with Dirichlet boundary condition](#gaussian-free-field-with-dirichlet-boundary-condition)
        - [Gibbs-Markov property of the discrete Gaussian free field](#gibbs-markov-property-of-the-discrete-gaussian-free-field)
        - [Spatial Markov property of the Gaussian free field](#spatial-markov-property-of-the-gaussian-free-field)
    - [Continuum Gaussian free field](#continuum-gaussian-free-field)
      - [Conformal invariance of the two-dimensional Gaussian free field](#conformal-invariance-of-the-two-dimensional-gaussian-free-field)
      - [Zero-boundary Gaussian free field](#zero-boundary-gaussian-free-field)
        - [SLE4 coupling with a Gaussian free field](#sle4-coupling-with-a-gaussian-free-field)
          - [Gaussian characteristic-function martingale from covariance loss](#gaussian-characteristic-function-martingale-from-covariance-loss)
          - [Gaussian free field level line](#gaussian-free-field-level-line)
        - [Test-function pairing with a Gaussian free field](#test-function-pairing-with-a-gaussian-free-field)
        - [Green-kernel expansion in the Dirichlet space](#green-kernel-expansion-in-the-dirichlet-space)
          - [Finite-Green-energy measure pairing with a Gaussian free field](#finite-green-energy-measure-pairing-with-a-gaussian-free-field)
        - [Domain Markov property of the Gaussian free field](#domain-markov-property-of-the-gaussian-free-field)
          - [Local set of a Gaussian free field](#local-set-of-a-gaussian-free-field)
        - [Circle-average process of the Gaussian free field](#circle-average-process-of-the-gaussian-free-field)
          - [Circle-average process of the Gaussian free field is Brownian motion](#circle-average-process-of-the-gaussian-free-field-is-brownian-motion)
    - [Green energy](#green-energy)
    - [Pinned Gaussian free field](#pinned-gaussian-free-field)
- [Gaussian zero-one law for measurable linear subspaces](#gaussian-zero-one-law-for-measurable-linear-subspaces)
- [Gaussian measure](#gaussian-measure)
  - [Fernique's theorem](#fernique-s-theorem)
  - [First Gaussian chaos](#first-gaussian-chaos)
  - [Gaussian random variable in a Banach space](#gaussian-random-variable-in-a-banach-space)
    - [Strict increase of a Gaussian norm distribution](#strict-increase-of-a-gaussian-norm-distribution)
  - [Cameron-Martin theorem for a Gaussian measure](#cameron-martin-theorem-for-a-gaussian-measure)
    - [Symmetric Gaussian translation lower bound](#symmetric-gaussian-translation-lower-bound)
  - [Cameron-Martin space of a Gaussian measure](#cameron-martin-space-of-a-gaussian-measure)
    - [Cameron-Martin space of a Gaussian random variable in a Banach space](#cameron-martin-space-of-a-gaussian-random-variable-in-a-banach-space)
  - [Covariance operator of a Gaussian measure](#covariance-operator-of-a-gaussian-measure)
    - [Hilbert-space Gaussian series](#hilbert-space-gaussian-series)
  - [Bayesian inverse problem](#bayesian-inverse-problem)
    - [Bayes formula for a dominated observation model](#bayes-formula-for-a-dominated-observation-model)
    - [Well-posed Bayesian inverse problem in total variation](#well-posed-bayesian-inverse-problem-in-total-variation)
    - [Well-posed Bayesian inverse problem in Hellinger distance](#well-posed-bayesian-inverse-problem-in-hellinger-distance)
- [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)
  - [Stationary trapped Brownian displacement](#stationary-trapped-brownian-displacement)
  - [Ornstein-Uhlenbeck transition distribution](#ornstein-uhlenbeck-transition-distribution)
  - [Ornstein-Uhlenbeck stationary initialization](#ornstein-uhlenbeck-stationary-initialization)
  - [Exact sampling of an Ornstein-Uhlenbeck process](#exact-sampling-of-an-ornstein-uhlenbeck-process)
  - [Stationary drift saturation](#stationary-drift-saturation)
    - [Same-noise stationary Ornstein-Uhlenbeck processes](#same-noise-stationary-ornstein-uhlenbeck-processes)
  - [Exponential Brownian time change to a stationary Ornstein-Uhlenbeck process](#exponential-brownian-time-change-to-a-stationary-ornstein-uhlenbeck-process)
  - [Ornstein-Uhlenbeck stochastic differential equation](#ornstein-uhlenbeck-stochastic-differential-equation)
  - [Ornstein-Uhlenbeck multiplicative amplification](#ornstein-uhlenbeck-multiplicative-amplification)
    - [Tilted Ornstein-Uhlenbeck oscillator transformation](#tilted-ornstein-uhlenbeck-oscillator-transformation)
  - [Integrated Ornstein-Uhlenbeck displacement](#integrated-ornstein-uhlenbeck-displacement)
  - [Explicit Ornstein-Uhlenbeck solution](#explicit-ornstein-uhlenbeck-solution)
    - [Zero-start Ornstein-Uhlenbeck covariance](#zero-start-ornstein-uhlenbeck-covariance)
  - [Multivariate Ornstein-Uhlenbeck process](#multivariate-ornstein-uhlenbeck-process)
    - [Ornstein-Uhlenbeck power spectrum](#ornstein-uhlenbeck-power-spectrum)
      - [Overdamped harmonic-trap power spectrum](#overdamped-harmonic-trap-power-spectrum)
        - [Variance of a long-time mean in a harmonic trap](#variance-of-a-long-time-mean-in-a-harmonic-trap)
        - [Graphical corner frequency of a Lorentzian spectrum](#graphical-corner-frequency-of-a-lorentzian-spectrum)
  - [Colored noise](#colored-noise)

## Gaussian process regression

↑ **Parent:** [Gaussian process](gaussian-process.md)

Gaussian process regression estimates an unknown [function](function.md) by assigning its values a [Gaussian process](gaussian-process.md) law, then conditioning on observed values, often with independent [Gaussian noise](probability-distribution.md#gaussian-noise). The [covariance function](stochastic-process.md#covariance-function) expresses the proposed relation between nearby inputs; the [conditional multivariate normal distribution](probability-and-statistics.md#conditional-multivariate-normal-distribution) gives the resulting [Gaussian process regression posterior](probability-and-statistics.md#gaussian-process-regression-posterior). Its conditional [mean](expected-value.md) provides a prediction and its conditional [variance](variance.md) quantifies uncertainty under the chosen model. The [index set](computability-theory.md#index-set) can represent spatial locations or other inputs as well as time.

## Gaussian exponential martingale with deterministic variance

↑ **Parent:** [Gaussian process](gaussian-process.md)

Let $X_0=0$ and let $X$ be a centered [Gaussian process](gaussian-process.md) whose increments are independent of the past [filtration](stochastic-process.md#filtration-probability-theory), with deterministic variance $v(t)$. Its displayed exponential is a positive [martingale](martingale.md). Indeed, $X_t-X_s$ is a centered [Gaussian random variable](probability-distribution.md#gaussian-random-variable) with variance $v(t)-v(s)$, so the [Gaussian moment-generating function](probability-distribution.md#moment-generating-function-of-a-normal-distribution) gives

$$
\mathbb E[M_t\mid\mathcal F_s]=M_s\mathbb E\exp(X_t-X_s-(v(t)-v(s))/2)=M_s.
$$

The sign-reversed process has the same variance and the same conclusion. Continuity of paths is unnecessary for this conditional-expectation argument.

## Covariance criterion for a stationary Gaussian Markov process

↑ **Parent:** [Gaussian process](gaussian-process.md)

A centered continuous stationary scalar [Gaussian process](gaussian-process.md) of positive variance can be [Markov](markov-chain.md#markov-property) only if its covariance satisfies the displayed equation for $s,t\geq0$. Gaussian conditioning makes the future conditional mean $C(t)X_s/C(0)$; the [Markov property](markov-chain.md#markov-property) then forces the equation by conditioning a future observation on the present and past. Conversely this equation makes the Gaussian residual future independent of the past, proving the [Markov property](markov-chain.md#markov-property). In the nondegenerate decaying case the covariance is a single exponential. A sum $c_1e^{-a_1|t|}+c_2e^{-a_2|t|}$ with positive coefficients and distinct positive decay rates fails the equation and hence is not scalar Markov.

## Gaussian process construction from square-summable features

↑ **Parent:** [Gaussian process](gaussian-process.md)

For independent standard normal variables $\xi_i$ and $\sum_i k_i(t)^2<\infty$ at each fixed time, the series defines $X_t$ in $L^2$. Every finite linear combination is an $L^2$ limit of Gaussian variables and is Gaussian. Thus this constructs a [Gaussian process](gaussian-process.md) with the Gram [covariance kernel](random-variable.md#covariance-kernel) $K$. It supplies no sample-path continuity without additional assumptions.

## Canonical pseudometric of a Gaussian process

↑ **Parent:** [Gaussian process](gaussian-process.md)

The canonical distance is the [L2 norm](real-analysis.md#l2-norm) of an increment of a [Gaussian process](gaussian-process.md). It is a [pseudometric](topological-analysis.md#pseudometric), since distinct parameters may represent equal [random variables](random-variable.md) almost surely. Its [metric covering number](topological-analysis.md#metric-covering-number) appears in the [Dudley entropy integral](#dudley-entropy-integral). For standard [fractional Brownian motion](#fractional-brownian-motion), $d(s,t)=|s-t|^H$; a normalization with twice the [covariance function](stochastic-process.md#covariance-function) multiplies this distance by $\sqrt2$.

## Fractional Brownian motion

↑ **Parent:** [Gaussian process](gaussian-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fractional_Brownian_motion)

A fractional Brownian motion with [Hurst exponent](#hurst-exponent) $H\in(0,1)$ is a centered [Gaussian process](gaussian-process.md) with the displayed standard [covariance function](stochastic-process.md#covariance-function) and a [continuous modification](stochastic-process.md#continuous-modification). Its increment [variance](variance.md) is $|s-t|^{2H}$. Some sources omit the factor $1/2$, multiplying the process by $\sqrt2$; the corresponding increment [variance](variance.md) is then $2|s-t|^{2H}$. Its [canonical pseudometric of a Gaussian process](#canonical-pseudometric-of-a-gaussian-process) is proportional to $|s-t|^H$, which gives finite [expected value](expected-value.md) of its absolute [supremum](real-analysis.md#supremum) on compact intervals through the [Dudley entropy integral](#dudley-entropy-integral).

### Hurst exponent

↑ **Parent:** [Fractional Brownian motion](#fractional-brownian-motion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hurst_exponent)

For [fractional Brownian motion](#fractional-brownian-motion), $H\in(0,1)$ controls the [variance](variance.md) $|t-s|^{2H}$ of increments and the scaling of its [finite-dimensional distributions](stochastic-process.md#finite-dimensional-distribution). Larger $H$ means smaller increment [variance](variance.md) on intervals shorter than one and greater sample-path [Hölder continuity](sobolev-space.md#holder-condition).

## Sudakov-Fernique inequality

↑ **Parent:** [Gaussian process](gaussian-process.md)

For centered [multivariate normal distributions](probability-and-statistics.md#multivariate-normal-distribution), if $\mathbb E(U_i-U_j)^2\leq\mathbb E(V_i-V_j)^2$ for every pair, then the displayed comparison holds. For a quick proof, make $U,V$ [independent](random-variable.md#independent-random-variables) and set $Z_r=\sqrt{1-r}U+\sqrt rV$. Apply [Gaussian integration by parts](probability-distribution.md#stein-s-lemma-probability) to $F_\tau(z)=\tau^{-1}\log\sum_i e^{\tau z_i}$. With [softmax function](statistical-learning.md#softmax-function) weights $p_i$ and $D=\operatorname{Cov}(V)-\operatorname{Cov}(U)$, the derivative of $\mathbb EF_\tau(Z_r)$ is $\tfrac\tau4\mathbb E\sum_{i,j}p_ip_j(D_{ii}+D_{jj}-2D_{ij})\geq0$. Since $\max z_i\leq F_\tau(z)\leq\max z_i+\tau^{-1}\log n$, let $\tau\to\infty$. Singular [covariance matrices](variance.md#covariance-matrix) follow by adding identical small [independent](random-variable.md#independent-random-variables) [normal](probability-distribution.md#normal-distribution) noise to both vectors and taking a limit.

<h2 id="slepian-s-lemma">Slepian's lemma</h2>

↑ **Parent:** [Gaussian process](gaussian-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Slepian's_lemma)

For centered [multivariate normal distributions](probability-and-statistics.md#multivariate-normal-distribution) represented by vectors $U,V$ with equal corresponding [variances](variance.md) and $\mathbb E[U_iU_j]\geq\mathbb E[V_iV_j]$ for all distinct indices, $\mathbb P(U_i\leq u_i\text{ for all }i)\geq\mathbb P(V_i\leq u_i\text{ for all }i)$ for every threshold vector. In particular the [supremum](real-analysis.md#supremum) of $U$ is stochastically smaller than the [supremum](real-analysis.md#supremum) of $V$. Equal corresponding [variances](variance.md) are essential to this formulation. The related [Sudakov-Fernique inequality](#sudakov-fernique-inequality) compares [expected values](expected-value.md) of maxima using [variances](variance.md) of increments and does not require equal pointwise [variances](variance.md).

## Mean-square derivative of a Gaussian process

↑ **Parent:** [Gaussian process](gaussian-process.md)

A [Gaussian process](gaussian-process.md) has a mean-square derivative at $t$ when its difference quotients converge in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space). The [mean-square convergence](convergence-of-random-variables.md#convergence-in-l2) need not give differentiable sample paths. For a centered [stationary process](time-series.md#stationary-process) with twice continuously differentiable [covariance function](stochastic-process.md#covariance-function) $K(t-s)$, the difference quotients are Cauchy in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space), since their [covariance](variance.md#covariance) is a rectangular average of $-K''$. Their limits form a [Gaussian process](gaussian-process.md) with [covariance function](stochastic-process.md#covariance-function) $\mathbb E[Y(s)Y(t)]=-K''(s-t)$.

### Differentiable modification of a stationary Gaussian process

↑ **Parent:** [Mean-square derivative of a Gaussian process](#mean-square-derivative-of-a-gaussian-process)

For a centered [Gaussian process](gaussian-process.md) with [covariance function](stochastic-process.md#covariance-function) $K(s-t)$, twice continuous differentiability of $K$ and differentiability of $K''$ at zero imply a differentiable [modification of a stochastic process](stochastic-process.md#modification-of-a-stochastic-process) on compact intervals. The [even function](calculus.md#even-function) $K''$ satisfies $K'''(0)=0$, so the mean-square derivative $Y$ has [variance](variance.md) of increments $2(K''(h)-K''(0))=o(|h|)$. A [normal distribution](probability-distribution.md#normal-distribution) has fourth absolute moment three times the square of its [variance](variance.md), so [Kolmogorov continuity theorem](stochastic-process.md#kolmogorov-continuity-theorem) gives a [continuous modification](stochastic-process.md#continuous-modification) of $Y$. The [mean-square fundamental theorem of calculus](#mean-square-fundamental-theorem-of-calculus) identifies its path integral with a [modification of a stochastic process](stochastic-process.md#modification-of-a-stochastic-process) of $X$. This argument does not require integrability of $K$ or continuity of $K'''$.

### Mean-square fundamental theorem of calculus

↑ **Parent:** [Mean-square derivative of a Gaussian process](#mean-square-derivative-of-a-gaussian-process)

If an [L2 space](measure-theory.md#l2-space-is-a-hilbert-space)-valued map $X$ has a continuous mean-square derivative $Y$, then its increments equal the [Bochner integral](measure-theory.md#bochner-integral) of $Y$. To see this, for each partition interval $[t_j,t_{j+1}]$, continuous linear observations and the scalar mean-value bound give $\|X(t_{j+1})-X(t_j)-(t_{j+1}-t_j)Y(t_j)\|_2\leq(t_{j+1}-t_j)\sup_{u\in[t_j,t_{j+1}]}\|Y(u)-Y(t_j)\|_2$. Sum these errors. Uniform continuity of $Y$ makes the total error tend to zero as the mesh tends to zero, while the [Riemann sums](real-analysis.md#riemann-sum) converge to the [Bochner integral](measure-theory.md#bochner-integral). This proves the [fundamental theorem of calculus](calculus.md#fundamental-theorem-of-calculus) in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space). If a [Gaussian process](gaussian-process.md) derivative also has a [continuous modification](stochastic-process.md#continuous-modification), its anchored path integral $X(s)+\int_s^t\widetilde Y(u)\,du$ therefore produces a differentiable [modification of a stochastic process](stochastic-process.md#modification-of-a-stochastic-process) of the original [Gaussian process](gaussian-process.md).

## Gaussian process classification

↑ **Parent:** [Gaussian process](gaussian-process.md)

[Gaussian process classification](#gaussian-process-classification) links [latent variables](latent-variable.md) from a [Gaussian process](gaussian-process.md) to class [probabilities](probability-theory.md#probability). A binary [probit regression](generalized-linear-model.md#probit-model) likelihood is $\prod_i\Phi((2y_i-1)f_i)$ under [conditional independence](random-variable.md#conditional-independence). The [posterior distribution](bayesian-statistics.md#bayesian-posterior) of the latent values is not a [normal distribution](probability-distribution.md#normal-distribution).

## Periodic covariance function

↑ **Parent:** [Gaussian process](gaussian-process.md)

This [covariance function](stochastic-process.md#covariance-function) is periodic with period $P>0$. Map time to the circle $u(t)=(\cos(2\pi t/P),\sin(2\pi t/P))$ and pull back a [Gaussian kernel](positive-semidefinite-kernel.md#gaussian-kernel); since $\|u(t)-u(t')\|^2=4\sin^2(\pi(t-t')/P)$, this proves positive semidefiniteness. A [Gaussian process](gaussian-process.md) with this kernel has $\operatorname{Var}(f(t+P)-f(t))=0$ and therefore repeats at every fixed phase. Replacing the inner $\pi$ by $2\pi$ changes the actual period to $P/2$.

### Periodic Gaussian process with zero period average

↑ **Parent:** [Periodic covariance function](#periodic-covariance-function)

A zero-mean [Gaussian process](gaussian-process.md) need not have zero average in each realization. For the [periodic covariance function](#periodic-covariance-function), the constant Fourier component is

$$
c_0=\frac1P\int_0^Pk_P(t,u)\,du=A^2e^{-\ell^{-2}}I_0(\ell^{-2}),
$$

where $I_0$ is a [modified Bessel function](bessel-function.md#modified-bessel-function). Replacing $f(t)$ by $f(t)-P^{-1}\int_0^Pf(u)\,du$ gives a Gaussian process with kernel $k_P(t,t')-c_0$. This is a [positive-semidefinite kernel](positive-semidefinite-kernel.md) because it is a covariance after a linear transformation, and each sample has zero period average. The [real integral representation of the modified Bessel function I0](bessel-function.md#real-integral-representation-of-the-modified-bessel-function-i0) yields the displayed constant.

## Gaussian-process marginal likelihood

↑ **Parent:** [Gaussian process](gaussian-process.md)

For Gaussian-process latent values with mean vector $m$ and covariance matrix $K$, observed with independent Gaussian noise covariance $E$, integrating out the latent values gives the marginal distribution $N(m,K+E)$. Its density as a function of the mean and kernel parameters is the Gaussian-process marginal likelihood.

## Gaussian concentration inequality

↑ **Parent:** [Gaussian process](gaussian-process.md)

A Lipschitz function of a Gaussian vector has sub-Gaussian deviations from its mean, with scale controlled by the covariance operator and the Lipschitz constant. In particular, if the covariance operator norm is at most one and $f$ is one-Lipschitz, then universal constants $c,C>0$ give

$$
\mathbb P(f(X)>\mathbb Ef(X)+u)\leq C e^{-cu^2}.
$$

### Brownian martingale proof of Gaussian concentration

↑ **Parent:** [Gaussian concentration inequality](#gaussian-concentration-inequality)

For a standard Gaussian vector $G$ and a smooth [Lipschitz function](real-analysis.md#lipschitz-continuity) with $\lVert\nabla f\rVert\le K$, represent its centered value as the terminal [martingale](martingale.md) $P_{1-t}f(B_t)-P_1f(0)$. The [Itô formula](stochastic-calculus.md#ito-s-lemma) gives gradient integrand $P_{1-t}\nabla f$, whose norm is at most $K$. Its terminal [quadratic variation](stochastic-calculus.md#quadratic-variation) is therefore at most $K^2$. The [Dambis-Dubins-Schwarz theorem](martingale.md#dambis-dubins-schwarz-theorem) bounds the terminal deviation by a maximum of [Brownian motion](brownian-motion.md) over $[0,K^2]$. Symmetry, the [Brownian reflection principle](brownian-motion.md#reflection-principle-wiener-process), and the [Gaussian tail bound](probability-and-statistics.md#gaussian-tail-bound) give the displayed inequality. The square on the Lipschitz constant is essential by scaling.

### Gaussian rotation interpolation inequality

↑ **Parent:** [Gaussian concentration inequality](#gaussian-concentration-inequality)

For [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) $X,Y$ with a centered [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution), a [continuously differentiable function](multivariable-calculus.md#continuously-differentiable-function) $f$ with bounded [gradient](multivariable-calculus.md#gradient), and a [convex function](real-analysis.md#convex-function) $\Psi$ for which the expressions are integrable, the displayed inequality holds. First apply [Jensen inequality](real-analysis.md#jensen-s-inequality) conditionally to $f(X)-f(Y)$. For the [Gaussian rotation of independent copies](probability-and-statistics.md#gaussian-rotation-of-independent-copies), the [chain rule](calculus.md#chain-rule) gives $f(X)-f(Y)=\int_0^{\pi/2}\langle\nabla f(U_\theta),V_\theta\rangle\,d\theta$. A second application of [Jensen inequality](real-analysis.md#jensen-s-inequality) to the uniform measure on $[0,\pi/2]$, followed by the [Gaussian rotation of independent copies](probability-and-statistics.md#gaussian-rotation-of-independent-copies), proves the inequality. The useful choice $\Psi(v)=e^{\lambda|v|}$ yields a [Gaussian concentration inequality](#gaussian-concentration-inequality) through an [exponential moment of an absolute standard normal variable](probability-distribution.md#exponential-moment-of-an-absolute-standard-normal-variable).

## Dudley entropy integral

↑ **Parent:** [Gaussian process](gaussian-process.md)

For a centered Gaussian process $(X_t)_{t\in T}$ with canonical pseudometric $d(s,t)^2=\mathbb E|X_s-X_t|^2$,

$$
\mathbb E\sup_{t\in T}X_t
\leq C\int_0^{\operatorname{diam}(T)}
\sqrt{\log N(\epsilon,T,d)}\,d\epsilon,
$$

where $N(\epsilon,T,d)$ is the covering number.

## Borell-TIS inequality

↑ **Parent:** [Gaussian process](gaussian-process.md)

If a centered separable Gaussian process has finite expected supremum $m$ and $\sigma^2=\sup_t\operatorname{Var}(X_t)$, then

$$
\mathbb P\left(\sup_tX_t>m+u\right)
\leq e^{-u^2/(2\sigma^2)}.
$$

## Isonormal Gaussian process

↑ **Parent:** [Gaussian process](gaussian-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Isonormal_Gaussian_process)

An isonormal Gaussian process over a real [Hilbert space](hilbert-space.md) $H$ is a centered [Gaussian process](gaussian-process.md) $(W(h))_{h\in H}$ satisfying

$$
\mathbb E[W(f)W(g)]=\langle f,g\rangle_H.
$$

It turns the geometry of $H$ into the [covariance](variance.md#covariance) structure of a Gaussian family.

### Exponential tilting of an isonormal Gaussian process

↑ **Parent:** [Isonormal Gaussian process](#isonormal-gaussian-process)

For an [isonormal Gaussian process](#isonormal-gaussian-process) $X$ on a real [Hilbert space](hilbert-space.md) $H$ and $k\in H$, the positive density $\exp(X(k)-\|k\|^2/2)$ has expectation one and defines an [equivalent probability measure](measure-theory.md#equivalent-probability-measure). Under this measure, $X(h)$ has mean $\langle h,k\rangle$ and the same [covariance](variance.md#covariance) as before. The shifted family $X(h)-\langle h,k\rangle$ is again an [isonormal Gaussian process](#isonormal-gaussian-process). This follows by evaluating the joint Gaussian exponential formula for any finite collection of arguments. It is the Hilbert-space version of [exponential tilting](probability-distribution.md#exponential-tilting).

## Gaussian white noise

↑ **Parent:** [Gaussian process](gaussian-process.md)

Gaussian white noise is a generalized Gaussian process with zero mean and covariance proportional to a [Dirac delta function](distribution-theory.md#dirac-delta-function) in time, and possibly in space. It is the formal time derivative of [Brownian motion](brownian-motion.md) and has independent fluctuations on disjoint time intervals.

### Gaussian white noise model

↑ **Parent:** [Gaussian white noise](#gaussian-white-noise)

Observe $Y(t)=\int_0^tf(s)\,ds+\sigma W(t)$ on $[0,1]$, where $f\in L^2[0,1]$ is an unknown deterministic drift and $W$ is standard [Brownian motion](brownian-motion.md). The observation against a deterministic test [function](function.md) is $Y(h)=\langle f,h\rangle+\sigma W(h)$, with [covariance](variance.md#covariance) $\sigma^2\langle h,g\rangle$. [Gaussian white noise](#gaussian-white-noise) is represented by an [isonormal Gaussian process](#isonormal-gaussian-process) on test [functions](function.md) rather than a pointwise noise [function](function.md). Taking $\sigma=n^{-1/2}$ is the usual statistical scaling.

### White-noise likelihood for a square-integrable shift

↑ **Parent:** [Gaussian white noise](#gaussian-white-noise)

Generalized [Gaussian white noise](#gaussian-white-noise) over a real [Hilbert space](hilbert-space.md) $H=L^2$ is an [isonormal Gaussian process](#isonormal-gaussian-process) $W(h)$ with covariance $\langle h,g\rangle_H$. Its law $P_0$ is carried on a larger observation space; the identity is not the covariance of an infinite-dimensional $H$-valued [Gaussian measure](#gaussian-measure) because it is not a [trace-class operator](compact-operator.md#trace-class-operator). A deterministic signal $h\in H$ defines a translated observation law $P_h$ with [Radon-Nikodym derivative](measure-theory.md#radon-nikodym-derivative)

$$
\frac{dP_h}{dP_0}(m)=\exp\left(W_m(h)-\tfrac12\|h\|_H^2\right).
$$

In an [orthonormal basis](inner-product.md#orthonormal-basis), $W_m(h)=\sum_jm_jh_j$ is a stochastic series with total [variance](variance.md) $\|h\|_H^2$, not an inner product of two $H$-valued observations. The formula follows from the [Cameron-Martin theorem for a Gaussian measure](#cameron-martin-theorem-for-a-gaussian-measure) in its generalized white-noise version, or from finite-dimensional Gaussian likelihood ratios. On $\mathbb R^2$, generalized noise can be realized on [tempered distributions](fourier-analysis.md#tempered-distribution); an unweighted global negative [Sobolev space](sobolev-space.md) is not automatically a suitable almost-sure support on an unbounded domain. The stochastic series avoids imposing that unsupported regularity.

### Gaussian sequence model

↑ **Parent:** [Gaussian white noise](#gaussian-white-noise)

The Gaussian sequence model observes

$$
Y_k=\theta_k+n^{-1/2}g_k,
\qquad k\geq1,
$$

where the $g_k$ are independent standard normal variables and the unknown signal commonly lies in $\ell^2$. It is the coordinate representation of a Gaussian white-noise experiment.

#### Bernstein-von Mises theorem

↑ **Parent:** [Gaussian sequence model](#gaussian-sequence-model)

A Bernstein-von Mises theorem says that a suitably centered and scaled posterior distribution converges to the normal distribution prescribed by the local likelihood. For a fixed linear functional in a Gaussian sequence model and a prior with locally flat positive density, the limiting posterior variance is the squared $\ell^2$ norm of the functional's coefficient vector.

#### Gaussian net test

↑ **Parent:** [Gaussian sequence model](#gaussian-sequence-model)

A Gaussian net test covers a composite alternative by finitely many metric balls and takes the maximum of the likelihood-ratio tests against their centers. Gaussian tail bounds control each test, while a union bound costs the logarithm of the covering number.

#### Gaussian least-squares contrast

↑ **Parent:** [Gaussian sequence model](#gaussian-sequence-model)

Because Gaussian white noise is not an $\ell^2$ vector, least squares over $\Theta\subset\ell^2$ is defined by maximizing

$$
2\langle Y,\theta\rangle-\lVert\theta\rVert_2^2
$$

over $\theta\in\Theta$, with the noise pairing interpreted through an [isonormal Gaussian process](#isonormal-gaussian-process). Differences of this contrast equal the formal differences of squared residual norms.

## Independent increments of a Gaussian martingale

↑ **Parent:** [Gaussian process](gaussian-process.md)

A centered continuous [Gaussian process](gaussian-process.md) that is also a [martingale](martingale.md) has independent increments. Every future increment has zero [covariance](variance.md#covariance) with every finite vector of past values by the martingale property; [uncorrelated jointly normal variables are independent](probability-and-statistics.md#uncorrelated-jointly-normal-variables-are-independent).

### Gaussian continuous martingale

↑ **Parent:** [Independent increments of a Gaussian martingale](#independent-increments-of-a-gaussian-martingale)

Every centered continuous Gaussian martingale starting at zero is a deterministic time change of [Brownian motion](brownian-motion.md). Its clock is the continuous increasing function $f(t)=\mathbb E[M_t^2]$, and $[M]_t=f(t)$.

#### Deterministic quadratic variation characterizes a Gaussian continuous local martingale

↑ **Parent:** [Gaussian continuous martingale](#gaussian-continuous-martingale)

If a continuous local martingale starts at zero and has deterministic continuous [quadratic variation](stochastic-calculus.md#quadratic-variation) $[M]_t=f(t)$, the [Dambis-Dubins-Schwarz theorem](martingale.md#dambis-dubins-schwarz-theorem) gives $M_t=B_{f(t)}$. It is therefore a centered [Gaussian process](gaussian-process.md). The converse follows from [independent increments of a Gaussian martingale](#independent-increments-of-a-gaussian-martingale).

## Exponential covariance function

↑ **Parent:** [Gaussian process](gaussian-process.md)

The stationary exponential covariance function is

$$
k(s,t)=R\exp(-|t-s|/\tau).
$$

The corresponding [Gaussian process](gaussian-process.md) is Markov and is a stationary [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process).

## Gaussian random field

↑ **Parent:** [Gaussian process](gaussian-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_random_field)

A Gaussian random field is a spatially indexed [Gaussian process](gaussian-process.md); its law is determined by its mean and covariance kernel.

### Brownian sheet

↑ **Parent:** [Gaussian random field](#gaussian-random-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brownian_sheet)

A centered [Gaussian random field](#gaussian-random-field) with the displayed covariance. It has independent increments over disjoint rectangles. At fixed positive $T$, $W(t,T)/\sqrt T$ is standard [Brownian motion](brownian-motion.md) in $t$. It provides one possible maturity-correlated Gaussian noise for a [Gaussian forward-rate field](mathematical-finance.md#gaussian-forward-rate-field); the forward-rate drift must still satisfy the [Heath-Jarrow-Morton model](mathematical-finance.md#heath-jarrow-morton-model) restriction.

### Gaussian marginals do not imply a Gaussian random field

↑ **Parent:** [Gaussian random field](#gaussian-random-field)

Let $X$ be a standard [Gaussian random variable](probability-distribution.md#gaussian-random-variable) and $S_j$ independent symmetric signs, independent of $X$. The stationary sequence $W_j=S_jX$ has standard Gaussian marginals and identity covariance, but is not jointly Gaussian. For two coordinates its [moment-generating function](probability-distribution.md#moment-generating-function) is $(1+e^{2t^2})/2$, rather than $e^{t^2}$. Consequently a field's Gaussian one-point densities and two-point covariance alone do not justify an [exponential moment of a Gaussian linear functional](#exponential-moment-of-a-gaussian-linear-functional).

### Centered quadratic Gaussian transformation

↑ **Parent:** [Gaussian random field](#gaussian-random-field)

If $G$ is a centered [Gaussian random field](#gaussian-random-field), the transformation $G+\alpha(G^2-\langle G^2\rangle)$ retains zero mean and introduces a three-point [connected correlation function](critical-phenomenon.md#connected-correlation-function) at first order in $\alpha$. [Wick contractions](perturbative-quantum-field-theory.md#wick-contraction) give $2\alpha$ times the sum of products of two covariances. The corresponding local cosmological model uses $\alpha=3f_{\mathrm{NL}}/5$.

### Exponential moment of a Gaussian linear functional

↑ **Parent:** [Gaussian random field](#gaussian-random-field)

If a linear functional $Z=\int a(\mathbf r)V(\mathbf r)\,d\mathbf r$ of a real [Gaussian random field](#gaussian-random-field) exists in mean square, it is a [Gaussian random variable](probability-distribution.md#gaussian-random-variable). Completing the square in its density gives

$$
\mathbb E e^Z=\exp\left(\mathbb EZ+\frac12\operatorname{Var}Z\right),\qquad \operatorname{Var}Z=\iint a(\mathbf r)a(\mathbf r')\operatorname{Cov}[V(\mathbf r),V(\mathbf r')]\,d\mathbf r\,d\mathbf r'.
$$

For a complex linear functional $\phi$, apply this to $Z=2\operatorname{Re}\phi$; then $\tfrac12\operatorname{Var}Z=\mathbb E|\phi-\mathbb E\phi|^2+\operatorname{Re}\mathbb E(\phi-\mathbb E\phi)^2$.

#### Gaussian quadratic exponential moment

↑ **Parent:** [Exponential moment of a Gaussian linear functional](#exponential-moment-of-a-gaussian-linear-functional)

For a real standard [Gaussian random vector](probability-and-statistics.md#gaussian-random-vector) $Z$, a real symmetric matrix $Q$, and $I-2Q$ strictly positive,

$$
\mathbb E e^{b^TZ+Z^TQZ}=\det(I-2Q)^{-1/2}\exp\left[\frac12b^T(I-2Q)^{-1}b\right].
$$

Diagonalize $Q$ and complete the square in each coordinate. Failure of strict positivity makes the positive exponential integral divergent. The same formula extends to a self-adjoint trace-class quadratic form of an isonormal [Gaussian process](gaussian-process.md), with square-summable linear coefficients and a [Fredholm determinant](compact-operator.md#fredholm-determinant). A linear-plus-quadratic [Gaussian random field](#gaussian-random-field) functional is reduced to this form by its covariance square root.

### Stationary Gaussian random field

↑ **Parent:** [Gaussian random field](#gaussian-random-field)

A stationary Gaussian random field has Gaussian finite-dimensional distributions invariant under common spatial translations. Its mean is constant and its two-point covariance depends only on the separation of the points.

#### Autocorrelation function of a random field

↑ **Parent:** [Stationary Gaussian random field](#stationary-gaussian-random-field)

For a zero-mean [stationary Gaussian random field](#stationary-gaussian-random-field) $V(\mathbf r)$, the autocorrelation function is

$$
C_V(\mathbf s)
=\mathbb E[V(\mathbf r)V(\mathbf r+\mathbf s)],
$$

which is independent of $\mathbf r$. Its [Fourier transform](fourier-transform.md) is the spatial power spectral density.

##### Covariance of a squared random field

↑ **Parent:** [Autocorrelation function of a random field](#autocorrelation-function-of-a-random-field)

For $W=n^2-\langle n^2\rangle$, the [covariance function](stochastic-process.md#covariance-function) is $\langle n^2n'^2\rangle-\langle n^2\rangle\langle n'^2\rangle$. It involves fourth moments and is not determined by the two-point correlation of $n$ in general. For a centered Gaussian pair the fourth-moment identity reduces it to $2\langle nn'\rangle^2$. This extra Gaussian hypothesis must be stated before using that reduction.

<h3 id="novikov-s-theorem">Novikov's theorem</h3>

↑ **Parent:** [Gaussian random field](#gaussian-random-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Novikov's_theorem)

For a centered [Gaussian random field](#gaussian-random-field) $W$ with covariance $C$ and a sufficiently regular functional $F[W]$, the Furutsu--Novikov formula is the functional [integration by parts](calculus.md#integration-by-parts) identity

$$
\mathbb E[W(x)F[W]]
=\int C(x,y)\mathbb E\left[\frac{\delta F}{\delta W(y)}\right]dy.
$$

It closes moment equations for systems driven multiplicatively by Gaussian fluctuations.

### Markov approximation for a random medium

↑ **Parent:** [Gaussian random field](#gaussian-random-field)

When a random medium's longitudinal correlation length is much shorter than the scale on which a propagating envelope changes, the Markov approximation replaces the longitudinal covariance by white noise with the same integrated covariance. Field-moment equations then become local in propagation distance.

### Gaussian free field

↑ **Parent:** [Gaussian random field](#gaussian-random-field)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_free_field)

The Gaussian free field is a centered [Gaussian random field](#gaussian-random-field) whose covariance is the Green kernel of a Laplace operator. It has discrete versions on graphs and continuum versions as a random generalized function on a domain.

#### Discrete Gaussian free field

↑ **Parent:** [Gaussian free field](#gaussian-free-field)

The discrete Gaussian free field on a transient weighted graph is the centered [Gaussian random field](#gaussian-random-field) whose covariance kernel is the random-walk [Green function of a transient weighted graph](random-walk.md#green-function-of-a-transient-weighted-graph).

##### Gaussian free field with Dirichlet boundary condition

↑ **Parent:** [Discrete Gaussian free field](#discrete-gaussian-free-field)

A Gaussian free field with Dirichlet boundary condition is fixed to zero on a boundary set and has density proportional to the exponential of minus one half of its discrete Dirichlet energy on the remaining vertices.

###### Gibbs-Markov property of the discrete Gaussian free field

↑ **Parent:** [Gaussian free field with Dirichlet boundary condition](#gaussian-free-field-with-dirichlet-boundary-condition)

Conditionally on all other values, a discrete Gaussian free field value is Gaussian with mean equal to the weighted average of its neighbors and variance equal to the reciprocal local precision.

###### Spatial Markov property of the Gaussian free field

↑ **Parent:** [Gaussian free field with Dirichlet boundary condition](#gaussian-free-field-with-dirichlet-boundary-condition)

Conditioning a Gaussian free field on its values along a boundary leaves an independent zero-boundary Gaussian free field plus the harmonic extension of those boundary values in each remaining component.

#### Continuum Gaussian free field

↑ **Parent:** [Gaussian free field](#gaussian-free-field)

The continuum Gaussian free field on a planar domain $D$ is a centered [Gaussian process](gaussian-process.md) indexed by finite-energy [measures](measure.md) or [test functions](distribution-theory.md#test-function), with [covariance](variance.md#covariance) given by the [Green function of the Laplacian](partial-differential-equation.md#green-function-of-the-laplacian) on $D$.

##### Conformal invariance of the two-dimensional Gaussian free field

↑ **Parent:** [Continuum Gaussian free field](#continuum-gaussian-free-field)

If $\phi:D\to\widetilde D$ is a [conformal map](geometry-and-topology.md#conformal-map), pulling back a zero-boundary Gaussian free field on $\widetilde D$ gives a zero-boundary Gaussian free field on $D$. This follows from the conformal invariance of the planar Dirichlet Green function.

##### Zero-boundary Gaussian free field

↑ **Parent:** [Continuum Gaussian free field](#continuum-gaussian-free-field)

For finite Borel measures $\rho,\nu$ of finite Green energy, the zero-boundary Gaussian free field $h$ on $D$ is characterized by

$$
\mathbb E[(h,\rho)(h,\nu)]=\iint_{D\times D}G_D(x,y)\rho(dx)\nu(dy),
$$

where $G_D$ is the zero-Dirichlet [Green function of the Laplacian](partial-differential-equation.md#green-function-of-the-laplacian).

###### SLE4 coupling with a Gaussian free field

↑ **Parent:** [Zero-boundary Gaussian free field](#zero-boundary-gaussian-free-field)

For a [Gaussian free field](#gaussian-free-field) with boundary heights $-\lambda$ and $+\lambda$ on the two sides of the starting point, its distinguished zero-height interface has chordal $\operatorname{SLE}_4$ law. Conditional on an initial curve segment, the field is a zero-boundary field in the slit domain plus $m_t(z)=\lambda-(2\lambda/\pi)\arg(g_t(z)-W_t)$. Its mean bracket equals minus the variation of its conditional Green [covariance](variance.md#covariance). Subtracting the initial [harmonic function](partial-differential-equation.md#harmonic-function) gives the corresponding coupling to a zero-boundary field.

###### Gaussian characteristic-function martingale from covariance loss

↑ **Parent:** [SLE4 coupling with a Gaussian free field](#sle4-coupling-with-a-gaussian-free-field)

If a continuous mean [martingale](martingale.md) $M$ and a nonnegative finite-variation process $V$ satisfy $d\langle M\rangle=-dV$, then the [Itô formula](stochastic-calculus.md#ito-s-lemma) shows $\exp(iM-V/2)$ is a bounded complex [martingale](martingale.md). Its terminal expectation establishes an entire [Gaussian distribution](probability-distribution.md#normal-distribution) with the initial mean and variance. This is stronger than matching only the first two moments in a random-domain field construction.

###### Gaussian free field level line

↑ **Parent:** [SLE4 coupling with a Gaussian free field](#sle4-coupling-with-a-gaussian-free-field)

A continuum field level line is specified by the harmonic boundary heights it creates and the conditional zero-boundary field remaining on each side. Since a [Continuum Gaussian free field](#continuum-gaussian-free-field) is a random distribution, this is not the pointwise set of its zeros. For the height jump appropriate to the Green-function normalization, the zero-height line between opposite Dirichlet heights is chordal $\operatorname{SLE}_4$.

###### Test-function pairing with a Gaussian free field

↑ **Parent:** [Zero-boundary Gaussian free field](#zero-boundary-gaussian-free-field)

For a [test function](distribution-theory.md#test-function) $\phi$ on $D$, let $f_\phi=-2\pi\Delta^{-1}\phi\in H_0^1(D)$. The pairing

$$
(h,\phi):=(h,f_\phi)_\nabla
$$

is a centered [Gaussian random variable](probability-distribution.md#gaussian-random-variable) with variance

$$
\iint_{D\times D}\phi(x)G_D(x,y)\phi(y)\,dx\,dy.
$$

###### Green-kernel expansion in the Dirichlet space

↑ **Parent:** [Zero-boundary Gaussian free field](#zero-boundary-gaussian-free-field)

For an [orthonormal basis](inner-product.md#orthonormal-basis) $(e_n)$ of $H_0^1(D)$, the zero-Dirichlet [Green function of the Laplacian](partial-differential-equation.md#green-function-of-the-laplacian) is the weak kernel represented by

$$
G_D(x,y)=\sum_{n\geq1}e_n(x)e_n(y).
$$

Consequently, whenever the terms are defined and the right side is finite,

$$
\sum_{n\geq1}\left(\int_De_n\,d\rho\right)^2
=\iint_{D\times D}G_D(x,y)\rho(dx)\rho(dy).
$$

###### Finite-Green-energy measure pairing with a Gaussian free field

↑ **Parent:** [Green-kernel expansion in the Dirichlet space](#green-kernel-expansion-in-the-dirichlet-space)

If a measure $\rho$ has finite [Green energy](#green-energy), then

$$
(h,\rho)=\sum_{n\geq1}\xi_n\int_De_n\,d\rho
$$

converges in $L^2$ for any [orthonormal basis](inner-product.md#orthonormal-basis) $(e_n)$ of $H_0^1(D)$ and independent standard normal coefficients $\xi_n$. The limit is centered Gaussian with variance equal to the Green energy of $\rho$ and does not depend on the chosen basis.

###### Domain Markov property of the Gaussian free field

↑ **Parent:** [Zero-boundary Gaussian free field](#zero-boundary-gaussian-free-field)

For an open $U\subset D$, the field decomposes as $h=h_U+h^{D\setminus U}$, where $h_U$ is an independent zero-boundary Gaussian free field on $U$ and $h^{D\setminus U}$ is harmonic on $U$ and agrees with the outside field in the distributional sense.

###### Local set of a Gaussian free field

↑ **Parent:** [Domain Markov property of the Gaussian free field](#domain-markov-property-of-the-gaussian-free-field)

A random set is local for a [Gaussian free field](#gaussian-free-field) if, conditionally on the set and its associated [harmonic function](partial-differential-equation.md#harmonic-function), the remaining field is an independent zero-boundary field in its complement. This extends the deterministic [Domain Markov property of the Gaussian free field](#domain-markov-property-of-the-gaussian-free-field) to appropriate random revealed domains. Arbitrary field-dependent random sets need not have this property.

###### Circle-average process of the Gaussian free field

↑ **Parent:** [Zero-boundary Gaussian free field](#zero-boundary-gaussian-free-field)

Let $\rho_t$ be uniform measure on the circle of radius $e^{-t}$ around the origin in the unit disc. The process $X_t=(h,\rho_t)$ is the circle-average process. The [Domain Markov property of the Gaussian free field](#domain-markov-property-of-the-gaussian-free-field) and the [mean value property for harmonic functions](partial-differential-equation.md#mean-value-property-for-harmonic-functions) imply that its increments are independent and stationary.

###### Circle-average process of the Gaussian free field is Brownian motion

↑ **Parent:** [Circle-average process of the Gaussian free field](#circle-average-process-of-the-gaussian-free-field)

The circle-average process of a zero-boundary Gaussian free field in the unit disc has the law of a constant multiple of [Brownian motion](brownian-motion.md). It is a continuous centered [Gaussian process](gaussian-process.md) with [stationary increments](stochastic-process.md#stationary-increments) and [independent increments](stochastic-process.md#independent-increments) and starts at zero.

#### Green energy

↑ **Parent:** [Gaussian free field](#gaussian-free-field)

For a measure $\mu$ and Green kernel $G$, its Green energy is

$$
I_G(\mu)=\iint G(x,y)d\mu(x)d\mu(y).
$$

Finite Green energy is the variance condition needed to pair a Gaussian free field with $\mu$.

#### Pinned Gaussian free field

↑ **Parent:** [Gaussian free field](#gaussian-free-field)

Pinning a Gaussian free field at a vertex $o$ gives the field with value zero at $o$ and covariance

$$
g^{\{o\}^c}(x,y)=g(x,y)-\frac{g(x,o)g(o,y)}{g(o,o)}.
$$

It is independent of the removed scalar Gaussian mode at $o$.

## Gaussian zero-one law for measurable linear subspaces

↑ **Parent:** [Gaussian process](gaussian-process.md)

Every linear subspace that is measurable for the [cylinder sigma-algebra](probability-space.md#cylinder-sigma-algebra) has probability zero or one under a centered Gaussian process.

## Gaussian measure

↑ **Parent:** [Gaussian process](gaussian-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gaussian_measure)

A Gaussian measure on a real topological vector space is a Borel probability measure whose image under every continuous linear functional is a one-dimensional normal distribution.

<h3 id="fernique-s-theorem">Fernique's theorem</h3>

↑ **Parent:** [Gaussian measure](#gaussian-measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fernique's_theorem)

A [Gaussian random variable in a Banach space](#gaussian-random-variable-in-a-banach-space) taking values in a [separable Banach space](banach-space.md#separable-banach-space) satisfies the displayed exponential-integrability bound for some positive $a$. In particular every finite power of its [norm](normed-vector-space.md#norm) has a finite [expected value](expected-value.md). The value of $a$ depends on the [Gaussian measure](#gaussian-measure); the theorem does not assert this for every positive $a$.

### First Gaussian chaos

↑ **Parent:** [Gaussian measure](#gaussian-measure)

For a centered [Gaussian random variable in a Banach space](#gaussian-random-variable-in-a-banach-space), its first Gaussian chaos is the closed [linear subspace](vector-space.md#vector-subspace) of [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) generated by its continuous linear observations. Every element is a centered [Gaussian random variable](probability-distribution.md#gaussian-random-variable), and every finite collection has a [multivariate normal distribution](probability-and-statistics.md#multivariate-normal-distribution): approximate in [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) and pass to the [characteristic function](characteristic-function.md). The first Gaussian chaos supplies the scalar coordinates of its [Cameron-Martin space of a Gaussian random variable in a Banach space](#cameron-martin-space-of-a-gaussian-random-variable-in-a-banach-space).

### Gaussian random variable in a Banach space

↑ **Parent:** [Gaussian measure](#gaussian-measure)

A random variable $X$ in a real [separable Banach space](banach-space.md#separable-banach-space) $B$ is Gaussian when $\ell(X)$ has a [normal distribution](probability-distribution.md#normal-distribution) for every [continuous linear functional](topological-vector-space.md#continuous-linear-functional) $\ell\in B^*$. It is centered when all these [expected values](expected-value.md) vanish. Its [probability law](probability-distribution.md) is a [Gaussian measure](#gaussian-measure). Degenerate [normal distributions](probability-distribution.md#normal-distribution) are allowed.

#### Strict increase of a Gaussian norm distribution

↑ **Parent:** [Gaussian random variable in a Banach space](#gaussian-random-variable-in-a-banach-space)

Suppose $B$ is a nonzero [separable Banach space](banach-space.md#separable-banach-space), the [Cameron-Martin space of a Gaussian random variable in a Banach space](#cameron-martin-space-of-a-gaussian-random-variable-in-a-banach-space) is a [dense subset](topology.md#dense-set) of $B$, and every centered ball of positive radius has positive [probability](probability-theory.md#probability). Then $t\mapsto\mathbb P(\|X\|_B\leq t)$ is strictly increasing on $(0,\infty)$. For $0<a<b$, choose $h$ in that [Cameron-Martin space of a Gaussian random variable in a Banach space](#cameron-martin-space-of-a-gaussian-random-variable-in-a-banach-space) with $\|h\|_B=(a+b)/2$ and $0<\delta<(b-a)/2$. The closed ball of radius $\delta$ centered at $h$ lies in the annulus $a<\|x\|_B<b$ and has positive [probability](probability-theory.md#probability) by the [symmetric Gaussian translation lower bound](#symmetric-gaussian-translation-lower-bound). The nonzero assumption is necessary: on $B=\{0\}$ the distribution function equals one everywhere.

### Cameron-Martin theorem for a Gaussian measure

↑ **Parent:** [Gaussian measure](#gaussian-measure)

For $\mu=\mathcal N(0,\Sigma)$ with injective [covariance operator of a Gaussian measure](#covariance-operator-of-a-gaussian-measure), its translated law $\mu_h=\mathcal N(h,\Sigma)$ is an [equivalent probability measure](measure-theory.md#equivalent-probability-measure) to $\mu$ if and only if $h\in E_\mu$, the [Cameron-Martin space of a Gaussian measure](#cameron-martin-space-of-a-gaussian-measure). For such $h$,

$$
\frac{d\mu_h}{d\mu}(x)=\exp\left(\ell_h(x)-\tfrac12\|h\|_{E_\mu}^2\right),\qquad
\ell_h(x)=\sum_j\frac{h_jx_j}{\lambda_j}.
$$

The series has [mean-square convergence](convergence-of-random-variables.md#convergence-in-l2) and converges [almost surely](convergence-of-random-variables.md#almost-sure-convergence) under $\mu$, with [normal distribution](probability-distribution.md#normal-distribution) $\mathcal N(0,\|h\|_{E_\mu}^2)$. Its exponential density has [expected value](expected-value.md) one by the [moment-generating function of a normal distribution](probability-distribution.md#moment-generating-function-of-a-normal-distribution). Finite-dimensional projections give the formula by ratios of [multivariate normal densities](probability-and-statistics.md#multivariate-normal-density); convergence of these likelihood ratios gives the infinite-dimensional result. The expression $\langle h,x\rangle_{E_\mu}$ is only formal when the sample is outside $E_\mu$. For $h\notin E_\mu$, translation gives [mutually singular measures](measure-theory.md#mutually-singular-measures).

#### Symmetric Gaussian translation lower bound

↑ **Parent:** [Cameron-Martin theorem for a Gaussian measure](#cameron-martin-theorem-for-a-gaussian-measure)

For a centered [Gaussian random variable in a Banach space](#gaussian-random-variable-in-a-banach-space), a [Borel set](measure-theory.md#borel-set) $C=-C$, and $h$ in its [Cameron-Martin space of a Gaussian random variable in a Banach space](#cameron-martin-space-of-a-gaussian-random-variable-in-a-banach-space), the [Cameron-Martin theorem for a Gaussian measure](#cameron-martin-theorem-for-a-gaussian-measure) gives the translated density $e^{-\widehat h(X)-\|h\|_H^2/2}$. The joint law of $(X,\widehat h(X))$ is invariant under simultaneous negation. Averaging the two density formulas therefore replaces $e^{-\widehat h(X)}$ by $\cosh\widehat h(X)\geq1$, proving the lower bound. No [convexity](real-analysis.md#convex-function) of $C$ is required.

### Cameron-Martin space of a Gaussian measure

↑ **Parent:** [Gaussian measure](#gaussian-measure)

For a centered [Gaussian measure](#gaussian-measure) on a real [Hilbert space](hilbert-space.md) with injective [covariance operator of a Gaussian measure](#covariance-operator-of-a-gaussian-measure) $\Sigma$, its Cameron-Martin space is $E_\mu=\operatorname{Ran}\Sigma^{1/2}$, with [inner product](inner-product.md) $\langle h,g\rangle_{E_\mu}=\langle\Sigma^{-1/2}h,\Sigma^{-1/2}g\rangle$. In an [orthonormal basis](inner-product.md#orthonormal-basis) satisfying $\Sigma e_j=\lambda_je_j$, it consists of exactly the vectors $h$ for which $\sum_jh_j^2/\lambda_j<\infty$. It is complete in this stronger norm even if its range is not closed in the ambient norm. Its importance is that it describes precisely the translations that preserve the null sets of the [Gaussian measure](#gaussian-measure), as in the [Cameron-Martin theorem for a Gaussian measure](#cameron-martin-theorem-for-a-gaussian-measure). For generalized [Gaussian white noise](#gaussian-white-noise) over $L^2$, the corresponding Cameron-Martin space is [L2 space](measure-theory.md#l2-space-is-a-hilbert-space) itself.

#### Cameron-Martin space of a Gaussian random variable in a Banach space

↑ **Parent:** [Cameron-Martin space of a Gaussian measure](#cameron-martin-space-of-a-gaussian-measure)

Let $\mathcal G$ be the [first Gaussian chaos](#first-gaussian-chaos) of a centered [Gaussian random variable in a Banach space](#gaussian-random-variable-in-a-banach-space). By [Fernique's theorem](#fernique-s-theorem), $Sg=\mathbb E[Xg]$ is a [Bochner integral](measure-theory.md#bochner-integral) in $B$. The map $S$ is injective, because $Sg=0$ implies $\mathbb E[g\ell(X)]=0$ for every [continuous linear functional](topological-vector-space.md#continuous-linear-functional) $\ell$, hence $g=0$. Its range becomes a [Hilbert space](hilbert-space.md) under $\langle Sg,Sv\rangle_H=\mathbb E[gv]$. The embedding in $B$ is continuous by [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality). Its [reproducing property](positive-semidefinite-kernel.md#reproducing-property) is $\langle h,S\ell(X)\rangle_H=\ell(h)$. Thus this is the [Reproducing kernel Hilbert space](positive-semidefinite-kernel.md#reproducing-kernel-hilbert-space) of the random variable, including degenerate laws. For $h=Sg$, the scalar coordinate $\widehat h(X)=g$ has [variance](variance.md) $\|h\|_H^2$; it is generally a measurable linear coordinate rather than a continuous functional on $B$.

### Covariance operator of a Gaussian measure

↑ **Parent:** [Gaussian measure](#gaussian-measure)

The covariance operator $K$ of a Gaussian measure on a real Hilbert space satisfies $\langle Kh,g\rangle=\operatorname{Cov}(\langle U,h\rangle,\langle U,g\rangle)$. A positive self-adjoint operator is the covariance of a Hilbert-space-valued Gaussian random variable exactly when it is trace class.

#### Hilbert-space Gaussian series

↑ **Parent:** [Covariance operator of a Gaussian measure](#covariance-operator-of-a-gaussian-measure)

If $Ke_j=\lambda_je_j$ with $\lambda_j\geq0$ and $\sum_j\lambda_j<\infty$, then

$$
U=m+\sum_j\sqrt{\lambda_j}\,\xi_je_j
$$

converges in mean square and almost surely in the Hilbert space, and has Gaussian law $N(m,K)$.

### Bayesian inverse problem

↑ **Parent:** [Gaussian measure](#gaussian-measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bayesian_inverse_problem)

A Bayesian inverse problem combines a prior measure $\mu_0$ on an unknown $u$ with a likelihood for observed data $y$. When the likelihood is proportional to $e^{-\Phi(u;y)}$, Bayes' formula gives

$$
\frac{d\mu^y}{d\mu_0}(u)=\frac1{Z(y)}e^{-\Phi(u;y)}.
$$

#### Bayes formula for a dominated observation model

↑ **Parent:** [Bayesian inverse problem](#bayesian-inverse-problem)

Suppose an unknown has [prior distribution](bayesian-statistics.md#prior-probability) $\Pi$ and its conditional observation law $P_u$ has jointly measurable [Radon-Nikodym derivative](measure-theory.md#radon-nikodym-derivative) $L(u,m)$ relative to a fixed observation law $P_0$. If $L>0$ for $\Pi(du)P_0(dm)$-almost every pair, then

$$
Z(m)=\int L(u,m)\Pi(du),\qquad
\frac{d\Pi^m}{d\Pi}(u)=\frac{L(u,m)}{Z(m)}
$$

defines the [posterior distribution](bayesian-statistics.md#bayesian-posterior) for almost every observation. Indeed, $\int L(u,m)P_0(dm)=1$ for almost every $u$, so [Tonelli theorem](measure-theory.md#tonelli-theorem) gives $\int Z(m)P_0(dm)=1$. Hence $Z$ is finite almost everywhere, and positivity of $L$ and [Fubini's theorem](measure-theory.md#fubini-s-theorem) give $Z>0$ almost everywhere. The data law is $ZP_0$, and integration of the proposed posterior against this data law recovers the joint law. This proves the [conditional distribution](probability-theory.md#conditional-distribution) property and also shows that the data law is an [equivalent probability measure](measure-theory.md#equivalent-probability-measure) to $P_0$.

#### Well-posed Bayesian inverse problem in total variation

↑ **Parent:** [Bayesian inverse problem](#bayesian-inverse-problem)

A Bayesian inverse problem is well posed in total variation when a unique posterior exists for every datum and the map from data to posterior is continuous in [total variation distance](probability-and-statistics.md#total-variation-distance).

#### Well-posed Bayesian inverse problem in Hellinger distance

↑ **Parent:** [Bayesian inverse problem](#bayesian-inverse-problem)

A Bayesian inverse problem is well posed in Hellinger distance when every datum determines a unique posterior and the posterior depends continuously on the data in [Hellinger distance](f-divergence.md#hellinger-distance). Since posterior measures are dominated by the prior and squared Hellinger distance is at most twice [total variation distance](probability-and-statistics.md#total-variation-distance), total-variation well-posedness implies Hellinger well-posedness.

## Ornstein-Uhlenbeck process

↑ **Parent:** [Gaussian process](gaussian-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ornstein–Uhlenbeck_process)

An Ornstein-Uhlenbeck process combines [mean reversion](stochastic-process.md#mean-reversion) with continuing random fluctuations. In the scalar model, its [stochastic differential equation](stochastic-calculus.md#stochastic-differential-equation) is

$$
dX_t=-\theta(X_t-\mu)\,dt+\sigma\,dW_t,\qquad \theta>0,\quad \sigma>0,\quad \mu\in\mathbb R,
$$

where $W$ is a standard [Brownian motion](brownian-motion.md). The [drift](stochastic-calculus.md#drift-coefficient) points towards $\mu$: it is negative above $\mu$ and positive below it. The coefficient $\theta$ sets the speed of [mean reversion](stochastic-process.md#mean-reversion), while $\sigma$ sets the strength of the random forcing. We consider a fixed or [normal](probability-distribution.md#normal-distribution) initial value independent of future [Brownian increments](brownian-motion.md#brownian-increment), giving a [Gaussian process](gaussian-process.md) and a [Markov process](markov-process.md).

For a stipulated example, use $\theta=1$, $\mu=2$, $\sigma=\sqrt2$ and the fixed initial value $X_0=6$, in arbitrary consistent state and time units. Then the [expected value](expected-value.md) relaxes as $2+4e^{-t}$ and the [variance](variance.md) grows as $1-e^{-2t}$. At time one they are about $3.4715$ and $0.8647$; the limiting [variance](variance.md) is one. The [sample paths](stochastic-process.md#sample-path) keep fluctuating even after the [expected value](expected-value.md) is close to two. The [Ornstein-Uhlenbeck transition distribution](#ornstein-uhlenbeck-transition-distribution) describes this evolving uncertainty; [Ornstein-Uhlenbeck stationary initialization](#ornstein-uhlenbeck-stationary-initialization) instead starts with that limiting [normal distribution](probability-distribution.md#normal-distribution) already in place.

A physical motivation is the [velocity](classical-mechanics.md#velocity) of a particle undergoing [Brownian motion](brownian-motion.md): [linear drag](fluid-mechanics.md#linear-drag) removes a persistent initial [velocity](classical-mechanics.md#velocity), while random forcing continually renews it. The original calculation gives a [normal distribution](probability-distribution.md#normal-distribution) for the [velocity](classical-mechanics.md#velocity) after subtracting its exponentially decaying initial contribution, with decay rate equal to the friction coefficient divided by the particle's [mass](classical-mechanics.md#mass).[On the Theory of the Brownian Motion, abstract: velocity minus its decaying initial contribution; friction coefficient divided by mass](mathematics-bibliography.md#on-the-theory-of-the-brownian-motion-by-g-e-uhlenbeck-and-l-s-ornstein) A position coordinate in an overdamped [harmonic optical trap](optics.md#harmonic-optical-trap) gives another interpretation of the same scalar equation, with $\theta=k/\zeta$ for [spring constant](elasticity-physics.md#spring-constant) $k$ and drag coefficient $\zeta$. Its physical assumptions and connection to measurements are developed in [thermal calibration of an optical trap](optics.md#thermal-calibration-of-an-optical-trap).

### Stationary trapped Brownian displacement

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

For overdamped [Brownian motion](brownian-motion.md) in potential $\kappa x^2/2$, the [relaxation time](markov-chain.md#relaxation-time) is $\tau=\zeta/\kappa$ and the equilibrium [correlation](variance.md#pearson-correlation-coefficient) is $(k_BT/\kappa)e^{-|t|/\tau}$. Expanding the squared displacement between two equilibrium samples gives the title expression. Initializing the particle exactly at the centre instead gives [variance](variance.md) $(k_BT/\kappa)(1-e^{-2t/\tau})$. Both are valid but concern different initial ensembles; their saturation values differ by a factor of two. These formulas neglect inertia and require times long compared with [momentum](momentum.md) relaxation.

### Ornstein-Uhlenbeck transition distribution

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

For a fixed initial value $X_0=x_0$, the [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process) has the [normal distribution](probability-distribution.md#normal-distribution)

$$
X_t\sim\mathcal N\!\left(\mu+(x_0-\mu)e^{-\theta t},\ \frac{\sigma^2}{2\theta}(1-e^{-2\theta t})\right),\qquad t>0.
$$

The two parameters of $\mathcal N(m,v)$ are the [expected value](expected-value.md) and [variance](variance.md), not the [standard deviation](variance.md#standard-deviation). At $t=0$ the [variance](variance.md) is zero and the value is fixed. More generally, its [transition kernel](markov-chain.md#markov-kernel) over any interval of length $h>0$ has [conditional expected value](measure-theory.md#conditional-expectation) $\mu+(x-\mu)e^{-\theta h}$ and conditional [variance](variance.md) $\sigma^2(1-e^{-2\theta h})/(2\theta)$ when the current value is $x$. The coefficients depend on elapsed time; the initial [probability distribution](probability-distribution.md) determines whether the resulting [stochastic process](stochastic-process.md) is stationary.[Applied Stochastic Differential Equations, Example 6.2, printed p. 81, equations (6.27)–(6.30); centered model with diffusion constant q](mathematics-bibliography.md#applied-stochastic-differential-equations-by-simo-sarkka-and-arno-solin)

In the stipulated example $\theta=1$, $\mu=2$, $\sigma=\sqrt2$, $x_0=6$, the [expected value](expected-value.md) at time two is $2+4e^{-2}\approx2.5413$ and the [variance](variance.md) is $1-e^{-4}\approx0.9817$. The initial distance from two has fallen by a factor $e^{-2}$, but the [standard deviation](variance.md#standard-deviation) has grown to about $0.9908$. Approaching the reference level in [expected value](expected-value.md) is compatible with growing uncertainty from a perfectly known initial value.

<a id="image-ornstein-uhlenbeck-transition-densities-mean-relaxation-and-variance-growth-from-a-fixed-initial-value"></a>
![](ornstein-uhlenbeck-transition-moments.png)

**[Figure 1](#image-ornstein-uhlenbeck-transition-densities-mean-relaxation-and-variance-growth-from-a-fixed-initial-value). Ornstein-Uhlenbeck transition densities, mean relaxation and variance growth from a fixed initial value**.

The solid [probability density functions](continuous-probability-distribution.md#probability-density-function) use times $0.25$, $1$ and $2$; the dashed curve is the limiting [normal distribution](probability-distribution.md#normal-distribution) with [expected value](expected-value.md) two and [variance](variance.md) one. The curves are exact model predictions. There is no ordinary density for the fixed value at time zero.

A short derivation uses the [integrating factor](linear-ordinary-differential-equation.md#integrating-factor) $e^{\theta t}$. The [Itô product rule](stochastic-calculus.md#ito-product-rule) gives $d[e^{\theta t}(X_t-\mu)]=\sigma e^{\theta t}\,dW_t$, hence

$$
X_t=\mu+(x_0-\mu)e^{-\theta t}+\sigma\int_0^t e^{-\theta(t-u)}\,dW_u.
$$

The [stochastic integral](stochastic-calculus.md#stochastic-integral) has zero [expected value](expected-value.md). The [Itô isometry](stochastic-calculus.md#ito-isometry) gives its [variance](variance.md) as $\sigma^2\int_0^t e^{-2\theta(t-u)}du$. Its deterministic integrand makes it a [Gaussian random variable](probability-distribution.md#gaussian-random-variable), yielding the displayed [normal distribution](probability-distribution.md#normal-distribution). Shifting the integration interval gives the same [transition kernel](markov-chain.md#markov-kernel) from any later time.

### Ornstein-Uhlenbeck stationary initialization

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

Set $v_\infty=\sigma^2/(2\theta)$ and draw $X_0\sim\mathcal N(\mu,v_\infty)$ independently of future [Brownian increments](brownian-motion.md#brownian-increment). The [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process) is then a [strictly stationary process](time-series.md#strictly-stationary-process), with

$$
\mathbb E X_t=\mu,\qquad \operatorname{Var}(X_t)=v_\infty,\qquad \operatorname{Cov}(X_s,X_t)=v_\infty e^{-\theta|t-s|}.
$$

Every time has the same [normal distribution](probability-distribution.md#normal-distribution), and the [covariance function](stochastic-process.md#covariance-function) depends only on the time lag. For a [Gaussian process](gaussian-process.md) these properties also make all its [finite-dimensional distributions](stochastic-process.md#finite-dimensional-distribution) invariant under a common time shift. The [stationary distribution](markov-chain.md#stationary-distribution) balances the continual random forcing against the contracting [drift](stochastic-calculus.md#drift-coefficient).[Applied Stochastic Differential Equations, Example 6.8, printed pp. 91–92, equations (6.73)–(6.76): steady-state variance and covariance](mathematics-bibliography.md#applied-stochastic-differential-equations-by-simo-sarkka-and-arno-solin)

With a fixed $X_0=x_0$, the [covariance function](stochastic-process.md#covariance-function) instead is

$$
\operatorname{Cov}(X_s,X_t)=v_\infty\left(e^{-\theta|t-s|}-e^{-\theta(s+t)}\right),\qquad s,t\ge0.
$$

In particular, it is zero when $s=0$, since the initial value has no uncertainty. The second term records the fixed start; it is the general scaling of the [zero-start Ornstein-Uhlenbeck covariance](#zero-start-ornstein-uhlenbeck-covariance). The pure [exponential covariance function](#exponential-covariance-function) displayed above assumes stationary initialization. For a fixed start, that function emerges as the late-time limit at fixed lag, while the one-time [probability distributions](probability-distribution.md) approach $\mathcal N(\mu,v_\infty)$ by [convergence in distribution](convergence-of-random-variables.md#convergence-in-distribution).

For the stipulated $\theta=1$, $\mu=2$, $\sigma=\sqrt2$, stationary initialization has [variance](variance.md) one from the outset. Its [autocorrelation](time-series.md#autocorrelation) is $e^{-|h|}$, so the [correlation time](time-series.md#correlation-time) is one: a lag of one reduces the [autocorrelation](time-series.md#autocorrelation) to $e^{-1}\approx0.3679$. Its raw second moment $\mathbb E[X_sX_t]=4+e^{-|t-s|}$ includes the squared [expected value](expected-value.md); it must not be confused with the [covariance](variance.md#covariance).

<a id="image-simulated-stationary-ornstein-uhlenbeck-samples-and-analytic-covariance-compared-with-a-fixed-start"></a>
![](ornstein-uhlenbeck-stationary-covariance-samples.png)

**[Figure 2](#image-simulated-stationary-ornstein-uhlenbeck-samples-and-analytic-covariance-compared-with-a-fixed-start). Simulated stationary Ornstein-Uhlenbeck samples and analytic covariance compared with a fixed start**.

The upper panel shows three simulated sequences with independent stationary initial values and exact transitions at spacing $0.05$. Joining their points only guides the eye; it does not simulate a continuous [sample path](stochastic-process.md#sample-path) between those points. The lower panel shows analytic [covariance functions](stochastic-process.md#covariance-function): the stationary curve and, for comparison, $\operatorname{Cov}(X_s,X_{s+h})$ for fixed initialization at two different ages $s$. These are simulated samples and model curves, not measured trajectories or empirical [covariance](variance.md#covariance) estimates.

### Exact sampling of an Ornstein-Uhlenbeck process

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

For any step $\Delta>0$, set $a=e^{-\theta\Delta}$. The [Ornstein-Uhlenbeck transition distribution](#ornstein-uhlenbeck-transition-distribution) gives the exact update

$$
X_{t+\Delta}=\mu+a(X_t-\mu)+\sqrt{\frac{\sigma^2}{2\theta}(1-a^2)}\,Z,\qquad Z\sim\mathcal N(0,1),
$$

using a fresh independent [standard normal random variable](probability-distribution.md#standard-normal-random-variable) for each interval. The update reproduces the [joint probability distribution](probability-distribution.md#joint-probability-distribution) on the selected time grid. It can start from a fixed value or use [Ornstein-Uhlenbeck stationary initialization](#ornstein-uhlenbeck-stationary-initialization). On an equally spaced grid it is an [autoregressive process of order one](time-series.md#autoregressive-process-of-order-one) after subtracting $\mu$. Its stationary [variance](variance.md) follows directly from $v=a^2v+v_\infty(1-a^2)$.

For the stipulated example with $\Delta=0.1$, $a=e^{-0.1}\approx0.90484$ and the innovation [variance](variance.md) is $1-e^{-0.2}\approx0.18127$. Given $X_t=6$, the next [conditional expected value](measure-theory.md#conditional-expectation) is about $5.61935$ and the conditional [standard deviation](variance.md#standard-deviation) is about $0.42576$.

The [Euler-Maruyama method](stochastic-calculus.md#euler-maruyama-method) instead approximates the same [stochastic differential equation](stochastic-calculus.md#stochastic-differential-equation) by

$$
X_{t+\Delta}^{\mathrm E}=\mu+(1-\theta\Delta)(X_t^{\mathrm E}-\mu)+\sigma\sqrt\Delta\,Z.
$$

For $0<\theta\Delta<2$ its stationary [variance](variance.md) solves $v=(1-\theta\Delta)^2v+\sigma^2\Delta$, giving

$$
v_{\mathrm E}=\frac{\sigma^2}{2\theta-\theta^2\Delta}=\frac{v_\infty}{1-\theta\Delta/2}.
$$

At $\Delta=0.1$ in the example, this is $1/0.95\approx1.05263$, about $5.26\%$ above the continuous model's stationary [variance](variance.md). If $\theta\Delta\ge2$, this Euler recurrence has no finite stationary [variance](variance.md) despite the stable continuous model. Exact transitions avoid this discretization error at sampled times; neither update alone determines the unresolved motion between samples.

### Stationary drift saturation

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

For an adapted [stationary process](time-series.md#stationary-process) with the displayed bounds, the [Itô formula](stochastic-calculus.md#ito-s-lemma) and stationarity give $\int_0^t(\mathbb E[Z_sg_s]+\lambda)ds=0$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) makes each integrand nonnegative, so equality holds almost everywhere. Then $\mathbb E(g_s+\lambda Z_s)^2\le0$, proving $g=-\lambda Z$ for almost every time and outcome. Thus the process solves the [Ornstein-Uhlenbeck stochastic differential equation](#ornstein-uhlenbeck-stochastic-differential-equation) and its initial value, rather than stationarity alone, determines its coupling with W.

#### Same-noise stationary Ornstein-Uhlenbeck processes

↑ **Parent:** [Stationary drift saturation](#stationary-drift-saturation)

Two [Ornstein-Uhlenbeck processes](#ornstein-uhlenbeck-process) with the same driving [Brownian motion](brownian-motion.md) have the displayed difference. If $Y_0$ is standard normal and independent of future Brownian increments, replacing it by $-Y_0$ produces another [stationary process](time-series.md#stationary-process) with the same covariance and second moment, but a different pathwise coupling. Equal initial values are necessary for [indistinguishability of stochastic processes](stochastic-process.md#indistinguishability-of-stochastic-processes).

### Exponential Brownian time change to a stationary Ornstein-Uhlenbeck process

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

For $\lambda>0$, set $\mathcal G_t=\mathcal F_{e^{2\lambda t}}$ and $W_t=(2\lambda)^{-1/2}\int_1^{e^{2\lambda t}}u^{-1/2}dB_u$. This is a [Brownian motion](brownian-motion.md) in the new [filtration](stochastic-process.md#filtration-probability-theory); its independent Gaussian increments have variance equal to elapsed time. The [Itô product rule](stochastic-calculus.md#ito-product-rule) gives $dY=\sqrt{2\lambda}\,dW-\lambda Y\,dt$. Its initial value is $B_1$, independent of future W increments, and its [covariance function](stochastic-process.md#covariance-function) is $e^{-\lambda|t-s|}$. Consequently it is a stationary [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process). The quadratic variation of the unscaled time change is $e^{2\lambda t}-1$, not $e^{2\lambda t}$.

### Ornstein-Uhlenbeck stochastic differential equation

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

The linear [stochastic differential equation](stochastic-calculus.md#stochastic-differential-equation) has the explicit solution $Y_t=e^{-\lambda t}Y_0+\sigma\int_0^te^{-\lambda(t-s)}dW_s$. Its integrating factor is $e^{\lambda t}$. For $\lambda>0$, an independent initial normal variable of variance $\sigma^2/(2\lambda)$ makes its zero-mean [Gaussian process](gaussian-process.md) stationary.

### Ornstein-Uhlenbeck multiplicative amplification

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

Let $d\sigma=-\sigma\,dt/\tau+\sqrt\kappa\,dW$, $\sigma_0=0$, and $\dot B=\sigma B$, $B_0>0$. The logarithm $\log(B_t/B_0)=\int_0^t\sigma_sds$ is a centered [Gaussian random variable](probability-distribution.md#gaussian-random-variable) of [variance](variance.md) $V(t)=\kappa\tau^2[t-2\tau(1-e^{-t/\tau})+\tau(1-e^{-2t/\tau})/2]$. Squaring the stochastic kernel $\sqrt\kappa\tau[1-e^{-(t-u)/\tau}]$ and integrating proves this formula. The [exponential moment of a Gaussian linear functional](#exponential-moment-of-a-gaussian-linear-functional) gives $\mathbb E B_t^n=B_0^ne^{n^2V(t)/2}$ and the displayed long-time growth exponent. Positive moment growth with zero mean strain reflects the breadth of the [log-normal distribution](probability-distribution.md#log-normal-distribution); it does not imply positive growth of the mean logarithm.

#### Tilted Ornstein-Uhlenbeck oscillator transformation

↑ **Parent:** [Ornstein-Uhlenbeck multiplicative amplification](#ornstein-uhlenbeck-multiplicative-amplification)

The weighted strain density in [Ornstein-Uhlenbeck multiplicative amplification](#ornstein-uhlenbeck-multiplicative-amplification) evolves under $\mathcal L_np=(\kappa/2)p''+\tau^{-1}(\sigma p)'+n\sigma p$. Setting $p=e^{-\sigma^2/(2\kappa\tau)}\psi$ eliminates its first derivative. Shifting and scaling to $x=(\sigma-\kappa n\tau^2)/\sqrt{\kappa\tau}$ gives $\psi_{xx}+[1+\kappa n^2\tau^3-2\gamma\tau-x^2]\psi=0$. The [quantum harmonic oscillator](quantum-harmonic-oscillator.md) levels yield the displayed [eigenvalues](linear-operator-theory.md#eigenvalue). Its [ground state](quantum-mechanics.md#ground-state) is the dominant positive mode; higher sign-changing modes may occur in a transient expansion.

### Integrated Ornstein-Uhlenbeck displacement

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

For a thermal inertial [Langevin equation](stochastic-process.md#langevin-dynamics) conditioned on fixed initial position and velocity, the centered displacement is $R_i=\zeta^{-1}\int_0^t[1-e^{-\zeta(t-s)}]A_i(s)ds$. With the [fluctuation-dissipation relation for a Langevin particle](stochastic-thermodynamics.md#fluctuation-dissipation-relation-for-a-langevin-particle), $D=k_BT/(m\zeta)$ and integrating the squared kernel gives the displayed [variance](variance.md). At short times it is $2D\zeta^2t^3/3$ per component; at long times it is $2Dt+O(1)$. Averaging initial velocity over thermal equilibrium adds a ballistic contribution and gives $2D[t-(1-e^{-\zeta t})/\zeta]$ per component.

### Explicit Ornstein-Uhlenbeck solution

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

The solution of

$$
dX_t=-\lambda X_t\,dt+dB_t,\qquad X_0=x,
$$

is

$$
X_t=xe^{-\lambda t}+\int_0^te^{-\lambda(t-s)}\,dB_s.
$$

It has variance $(1-e^{-2\lambda t})/(2\lambda)$. Starting from $N(0,(2\lambda)^{-1})$ makes it stationary with covariance $e^{-\lambda|t-s|}/(2\lambda)$.

#### Zero-start Ornstein-Uhlenbeck covariance

↑ **Parent:** [Explicit Ornstein-Uhlenbeck solution](#explicit-ornstein-uhlenbeck-solution)

For $d\sigma=-\sigma\,dt/\tau+\sqrt\kappa\,dW$ with $\sigma_0=0$, the explicit [stochastic integral](stochastic-calculus.md#stochastic-integral) is $\sigma_t=\sqrt\kappa\int_0^te^{-(t-u)/\tau}dW_u$. The [Itô isometry](stochastic-calculus.md#ito-isometry) on the overlap of the two integration intervals gives the displayed [covariance](variance.md#covariance). The second exponential records the zero initial condition; removing it gives the stationary [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process) covariance.

### Multivariate Ornstein-Uhlenbeck process

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)

A multivariate Ornstein-Uhlenbeck process obeys $dX=-AX\,dt+b\,dW$. If every eigenvalue of $A$ has positive real part, its stationary covariance $\Sigma$ is the unique solution of $A\Sigma+\Sigma A^T=bb^T$.

#### Ornstein-Uhlenbeck power spectrum

↑ **Parent:** [Multivariate Ornstein-Uhlenbeck process](#multivariate-ornstein-uhlenbeck-process)

The stationary spectral-density matrix of $dX=-AXdt+b\,dW$ is

$$
S(\omega)=(A+i\omega I)^{-1}bb^T(A^T-i\omega I)^{-1}.
$$

##### Overdamped harmonic-trap power spectrum

↑ **Parent:** [Ornstein-Uhlenbeck power spectrum](#ornstein-uhlenbeck-power-spectrum)

In the classical thermal model, a coordinate in a [harmonic potential](energy.md#harmonic-potential) obeys $\gamma\dot x+kx=\xi$, where $\gamma$ is the drag coefficient and $\langle\xi(t)\xi(t')\rangle=2\gamma k_BT\delta(t-t')$. Its stationary [one-sided spectral density](time-series.md#one-sided-spectral-density-of-a-real-stationary-time-series) per hertz is the displayed [Lorentzian line shape](stellar-astrophysics.md#lorentzian-line-shape). The integral over positive [frequencies](wave.md#frequency) equals $k_BT/k$, consistent with the [equipartition theorem](canonical-ensemble.md#equipartition-theorem). On a [log-log plot](calculus.md#log-log-plot) the spectrum is flat for $f\ll f_c$ and has slope $-2$ for $f\gg f_c$. The crossover is determined by the restoring stiffness and drag; an added detector response multiplies the mechanical spectrum by the squared magnitude of its transfer function.

###### Variance of a long-time mean in a harmonic trap

↑ **Parent:** [Overdamped harmonic-trap power spectrum](#overdamped-harmonic-trap-power-spectrum)

For stationary covariance $C(t)=(k_BT/k)e^{-|t|/\tau_k}$, the [mean](expected-value.md) over duration $\mathcal T$ has [variance](variance.md) $2(k_BT/k)[\tau_k/\mathcal T-(\tau_k/\mathcal T)^2(1-e^{-\mathcal T/\tau_k})]$. At $\mathcal T\gg\tau_k$ this becomes $2(k_BT/k)\tau_k/\mathcal T$. Closely sampled positions remain correlated and cannot be counted as independent.

###### Graphical corner frequency of a Lorentzian spectrum

↑ **Parent:** [Overdamped harmonic-trap power spectrum](#overdamped-harmonic-trap-power-spectrum)

For [power spectral density](electrical-engineering.md#power-spectral-density) $P(f)=C/(f^2+f_c^2)$, the low-frequency plateau is $P_0=C/f_c^2$ and the high-frequency asymptote is $C/f^2$. Their intersection on a [log-log plot](calculus.md#log-log-plot) gives the displayed corner [frequency](wave.md#frequency). Equivalently $P(f_c)=P_0/2$. Use the range unaffected by additional low-frequency [noise](electrical-engineering.md#noise-signal-processing) or high-frequency filtering; a measurement chain can otherwise shift an apparent corner.

### Colored noise

↑ **Parent:** [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Colored_noise)

Colored noise has nonzero temporal correlation away from equal times. An Ornstein-Uhlenbeck noise has exponential covariance and approaches white noise when its correlation time tends to zero at fixed integrated covariance.

## ↑ Ancestors (6)

1. [Stochastic process](stochastic-process.md)
2. [Probability theory](probability-theory.md)
3. [Probability and statistics](probability-and-statistics.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (84)

- [Autocorrelation](time-series.md#autocorrelation)
- [Autocovariance of an MA(1) process](time-series.md#autocovariance-of-an-ma-1-process)
- [Brownian motion transform by three times its running average](brownian-motion.md#brownian-motion-transform-by-three-times-its-running-average)
- [Brownian snake](stochastic-process.md#brownian-snake)
- [Canonical identifiability of Gaussian ARMA models](time-series.md#canonical-identifiability-of-gaussian-arma-models)
- [Canonical pseudometric of a Gaussian process](#canonical-pseudometric-of-a-gaussian-process)
- [Circle-average process of the Gaussian free field is Brownian motion](#circle-average-process-of-the-gaussian-free-field-is-brownian-motion)
- [Continuum Gaussian free field](#continuum-gaussian-free-field)
- [Covariance criterion for a stationary Gaussian Markov process](#covariance-criterion-for-a-stationary-gaussian-markov-process)
- [Covariance function](stochastic-process.md#covariance-function)
- [Cylindrical Brownian motion](brownian-motion.md#cylindrical-brownian-motion)
- [Deterministic quadratic variation characterizes a Gaussian continuous local martingale](#deterministic-quadratic-variation-characterizes-a-gaussian-continuous-local-martingale)
- [Differentiable modification of a stationary Gaussian process](#differentiable-modification-of-a-stationary-gaussian-process)
- [Exponential covariance function](#exponential-covariance-function)
- [F-Brownian bridge](brownian-motion.md#f-brownian-bridge)
- [Fractional Brownian motion](#fractional-brownian-motion)
- [Gaussian exponential martingale with deterministic variance](#gaussian-exponential-martingale-with-deterministic-variance)
- [Gaussian phase-screen correlation](partial-differential-equation.md#gaussian-phase-screen-correlation)
- [Gaussian-process characterization of Brownian motion](brownian-motion.md#gaussian-process-characterization-of-brownian-motion)
- [Gaussian process classification](#gaussian-process-classification)
- [Gaussian process construction from square-summable features](#gaussian-process-construction-from-square-summable-features)
- [Gaussian process regression](#gaussian-process-regression)
- [Gaussian process regression posterior](probability-and-statistics.md#gaussian-process-regression-posterior)
- [Gaussian quadratic exponential moment](#gaussian-quadratic-exponential-moment)
- [Gaussian random field](#gaussian-random-field)
- [Independent increments of a Gaussian martingale](#independent-increments-of-a-gaussian-martingale)
- [Inferring a binary from a detector network](gravitational-wave.md#inferring-a-binary-from-a-detector-network)
- [Innovation process](time-series.md#innovation-process)
- [Integrated Brownian motion](brownian-motion.md#integrated-brownian-motion)
- [Isonormal Gaussian process](#isonormal-gaussian-process)
- [Mathematical model](mathematics.md#mathematical-model)
- [Mean-square derivative of a Gaussian process](#mean-square-derivative-of-a-gaussian-process)
- [Mean-square fundamental theorem of calculus](#mean-square-fundamental-theorem-of-calculus)
- [Mean-square integral](measure-theory.md#mean-square-integral)
- [Ornstein-Uhlenbeck process](#ornstein-uhlenbeck-process)
- [Ornstein-Uhlenbeck stationary initialization](#ornstein-uhlenbeck-stationary-initialization)
- [Ornstein-Uhlenbeck stochastic differential equation](#ornstein-uhlenbeck-stochastic-differential-equation)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-34.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-36.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-83.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28.md#2/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28.md#2/b/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-30.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-30.md#6/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-37.md#1/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#1/1/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#1/1/7/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-217.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-217.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219.md#3/i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-219.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-219.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-219.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-220.md#2/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-202.md#6/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#29k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-203.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-203.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-207.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-207.md#3/c/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-219.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-201.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-217.md#4/solution)
- [Periodic covariance function](#periodic-covariance-function)
- [Periodic Gaussian process with zero period average](#periodic-gaussian-process-with-zero-period-average)
- [Phase folding of a light curve](astrophysics.md#phase-folding-of-a-light-curve)
- [Reproducing-kernel Hilbert space of a stationary Gaussian process](positive-semidefinite-kernel.md#reproducing-kernel-hilbert-space-of-a-stationary-gaussian-process)
- [Self-similar Gaussian workload rate](queueing-theory.md#self-similar-gaussian-workload-rate)
- [Stationary process](time-series.md#stationary-process)
- [Time reversal of a Brownian bridge](brownian-motion.md#time-reversal-of-a-brownian-bridge)
