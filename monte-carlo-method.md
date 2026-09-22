# Monte Carlo method

↑ **Parent:** [Probability and statistics](probability-and-statistics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Monte_Carlo_method)

A Monte Carlo method approximates a deterministic quantity using averages of simulated random variables and controls the approximation with probabilistic limit theorems.

**Table of contents**

- [Quantum Monte Carlo](#quantum-monte-carlo)
- [Pseudorandom number generator](#pseudorandom-number-generator)
  - [Random seed](#random-seed)
  - [Lagged Fibonacci generator](#lagged-fibonacci-generator)
  - [Pseudorandom number](#pseudorandom-number)
  - [Linear congruential generator](#linear-congruential-generator)
    - [Full-period criterion for a mixed congruential generator](#full-period-criterion-for-a-mixed-congruential-generator)
- [Monte Carlo integration](#monte-carlo-integration)
  - [Antithetic variates](#antithetic-variates)
    - [Antithetic Cauchy-tail integration on a finite interval](#antithetic-cauchy-tail-integration-on-a-finite-interval)
    - [Minimum-variance combination of unbiased sample means](#minimum-variance-combination-of-unbiased-sample-means)
      - [Cross-fitted combination of unbiased sample means](#cross-fitted-combination-of-unbiased-sample-means)
- [Conditional Monte Carlo](#conditional-monte-carlo)
- [Box-Muller transform](#box-muller-transform)
- [Nested Monte Carlo](#nested-monte-carlo)
- [Monte Carlo estimator](#monte-carlo-estimator)
  - [Summing before taking a mean changes Monte Carlo normalization](#summing-before-taking-a-mean-changes-monte-carlo-normalization)
  - [Proposal-budget variance comparison of importance and rejection sampling](#proposal-budget-variance-comparison-of-importance-and-rejection-sampling)
    - [Variance reversal under additive shifts of an importance-sampling integrand](#variance-reversal-under-additive-shifts-of-an-importance-sampling-integrand)
  - [Control variates](#control-variates)
    - [Multivariate control variates](#multivariate-control-variates)
    - [Cauchy tail control variate on a bounded interval](#cauchy-tail-control-variate-on-a-bounded-interval)
    - [Posterior score control variate](#posterior-score-control-variate)
- [Monte Carlo error](#monte-carlo-error)
  - [Monte Carlo standard error](#monte-carlo-standard-error)
- [Rejection sampling](#rejection-sampling)
  - [Acceptance mass for an unnormalized rejection envelope](#acceptance-mass-for-an-unnormalized-rejection-envelope)
  - [Truncated gamma rejection sampling with a Pareto envelope](#truncated-gamma-rejection-sampling-with-a-pareto-envelope)
  - [Uniform-envelope rejection sampling for a beta distribution](#uniform-envelope-rejection-sampling-for-a-beta-distribution)
  - [Bayesian rejection sampling for a segregating-site count](#bayesian-rejection-sampling-for-a-segregating-site-count)
    - [Joint posterior of mutation rate and coalescent times](#joint-posterior-of-mutation-rate-and-coalescent-times)
  - [Match-biased reshuffling preserves uniform rank marginals](#match-biased-reshuffling-preserves-uniform-rank-marginals)
  - [Exponential-envelope rejection sampling for a chi-squared variable](#exponential-envelope-rejection-sampling-for-a-chi-squared-variable)
  - [Ratio-of-uniforms method](#ratio-of-uniforms-method)
    - [Laplace ratio-of-uniforms envelope](#laplace-ratio-of-uniforms-envelope)
    - [Normal ratio-of-uniforms envelope](#normal-ratio-of-uniforms-envelope)
    - [Finite-area envelope for a ratio-of-uniforms region](#finite-area-envelope-for-a-ratio-of-uniforms-region)
  - [Normal rejection sampling with an exponential envelope](#normal-rejection-sampling-with-an-exponential-envelope)
  - [Marsaglia polar method](#marsaglia-polar-method)
  - [Binomial count and iid values in fixed-budget rejection sampling](#binomial-count-and-iid-values-in-fixed-budget-rejection-sampling)
    - [Random-count central limit theorem for accepted rejection samples](#random-count-central-limit-theorem-for-accepted-rejection-samples)
  - [Rejected-proposal distribution](#rejected-proposal-distribution)
  - [Adaptive rejection sampling](#adaptive-rejection-sampling)
- [Importance sampling](#importance-sampling)
  - [Importance sampling of a Cauchy tail](#importance-sampling-of-a-cauchy-tail)
  - [Rao-Blackwell identity for a fixed-denominator rejection estimator](#rao-blackwell-identity-for-a-fixed-denominator-rejection-estimator)
  - [Bounded-weight importance-sampling moment bound](#bounded-weight-importance-sampling-moment-bound)
  - [Minimum-variance importance distribution](#minimum-variance-importance-distribution)
  - [Support condition for importance sampling](#support-condition-for-importance-sampling)
  - [Importance weight](#importance-weight)
  - [Self-normalized importance sampling](#self-normalized-importance-sampling)
  - [Optimal importance density for a single integral](#optimal-importance-density-for-a-single-integral)
  - [Effective sample size of importance sampling](#effective-sample-size-of-importance-sampling)

## Quantum Monte Carlo

↑ **Parent:** [Monte Carlo method](monte-carlo-method.md)

Stochastic methods for quantum many-particle expectation values or ground-state projection. Variational and diffusion approaches can include correlations beyond a single [Slater determinant](tensor-product-of-quantum-systems.md#slater-determinant); [fermion](tensor-product-of-quantum-systems.md#fermion) signs or nodal constraints and finite-system extrapolation require explicit control.

## Pseudorandom number generator

↑ **Parent:** [Monte Carlo method](monte-carlo-method.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pseudorandom_number_generator)

A [pseudorandom number generator](#pseudorandom-number-generator) is a deterministic state-update algorithm producing numbers intended to imitate an independent sequence from a prescribed [probability distribution](probability-distribution.md). For [Monte Carlo integration](#monte-carlo-integration), desirable features include good one-dimensional and multidimensional uniformity, a period far longer than the calculation, negligible detectable dependence, reproducible seeds, sufficient numerical precision and fast generation. Uniform marginal distributions alone do not provide independent draws.

### Random seed

↑ **Parent:** [Pseudorandom number generator](#pseudorandom-number-generator)

A value initializing a pseudorandom generator. Repeating a seed need not reproduce a parallel stochastic calculation unless the generator, stream assignment and implementation are also controlled.

### Lagged Fibonacci generator

↑ **Parent:** [Pseudorandom number generator](#pseudorandom-number-generator)

A [pseudorandom number generator](#pseudorandom-number-generator) whose state sequence combines earlier values at two fixed lags, for example $S_n=(S_{n-j}+S_{n-k})\bmod m$ with $0<j<k$. A seed supplies the first $k$ values. A circular buffer of $k$ entries suffices for generation because each update uses only the retained lag window.

### Pseudorandom number

↑ **Parent:** [Pseudorandom number generator](#pseudorandom-number-generator)

A pseudorandom number is an output of a deterministic algorithm chosen to imitate samples from a specified [probability](probability-theory.md#probability) law. For example, a [linear congruential generator](#linear-congruential-generator) returns fractions $S_i/M$ on a finite grid in $[0,1)$. Their intended [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) is an approximation, and their serial dependence must be assessed separately from the generator's period.

### Linear congruential generator

↑ **Parent:** [Pseudorandom number generator](#pseudorandom-number-generator)

Choose integers $M>1$, $a$, $c$ and a seed $S_0$. Iterate $S_{n+1}=(aS_n+c)\bmod M$ and return $U_n=S_n/M$. This gives a deterministic finite-state [pseudorandom number generator](#pseudorandom-number-generator) with output in $[0,1)$. A nonzero increment gives a mixed generator; $c=0$ gives a multiplicative generator. Its period is at most $M$, but even a full period does not guarantee good multidimensional uniformity or statistical [independence](random-variable.md#independent-random-variables).

#### Full-period criterion for a mixed congruential generator

↑ **Parent:** [Linear congruential generator](#linear-congruential-generator)

A [linear congruential generator](#linear-congruential-generator) has period $M$ for every seed if and only if $\gcd(c,M)=1$, every prime dividing $M$ divides $a-1$, and $4\mid M$ implies $4\mid a-1$. The coprimality of $c$ prevents the orbit from being trapped in a residue class; the multiplier conditions permit full-period lifting through each prime power. Combining the prime-power periods by the [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) gives period $M$. For $M=12^k=2^{2k}3^k$, the multiplier criterion reduces to $a\equiv1\pmod{12}$, together with $\gcd(c,6)=1$. A positive increment alone is insufficient.

## Monte Carlo integration

↑ **Parent:** [Monte Carlo method](monte-carlo-method.md)

To calculate $I=\int h(x)p(x)\,dx$, generate independent $X_s$ with density $p$ and average $h(X_s)$. Integrability gives convergence by the [strong law of large numbers](convergence-of-random-variables.md#strong-law-of-large-numbers); finite [variance](variance.md) gives an unbiased estimate with variance $\operatorname{Var}(h(X))/S$. Applying this to indicators estimates probabilities. Correlated [Markov chain Monte Carlo](bayesian-statistics.md#markov-chain-monte-carlo) samples can also approximate the integral, but their error is determined by the chain's dependence rather than the independent-sample variance formula.

### Antithetic variates

↑ **Parent:** [Monte Carlo integration](#monte-carlo-integration)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Antithetic_variates)

[Antithetic variates](#antithetic-variates) deliberately couple [unbiased estimators](statistical-modelling.md#unbiased-estimator) of the same [expectation](expected-value.md) with negative [covariance](variance.md#covariance). Their average can have smaller [variance](variance.md) than an average using independent draws. For example, evaluating a monotone integrand at $U$ and $1-U$, where $U$ has a [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution), gives opposite fluctuations while preserving both marginal distributions.

#### Antithetic Cauchy-tail integration on a finite interval

↑ **Parent:** [Antithetic variates](#antithetic-variates)

For standard [Cauchy distribution](probability-distribution.md#cauchy-distribution) [probability density function](continuous-probability-distribution.md#probability-density-function) $f$ and $k>0$, this estimates its upper-tail [probability](probability-theory.md#probability) without sampling a heavy tail. The function $f(ku)$ decreases on $[0,1]$, while $f(k(1-u))$ increases, so their [covariance](variance.md#covariance) is nonpositive. The paired estimator is unbiased and has no larger [variance](variance.md) than an estimator using the same number $2r$ of [independent](random-variable.md#independent-random-variables) [probability density function](continuous-probability-distribution.md#probability-density-function) evaluations.

#### Minimum-variance combination of unbiased sample means

↑ **Parent:** [Antithetic variates](#antithetic-variates)

For two [unbiased estimators](statistical-modelling.md#unbiased-estimator) $A,B$ of the same parameter with [variances](variance.md) $V_X,V_Y$ and [covariance](variance.md#covariance) $C$, the fixed-weight estimator $wA+(1-w)B$ is unbiased and has [variance](variance.md) $w^2V_X+(1-w)^2V_Y+2w(1-w)C$. Completing the square gives $w_*=(V_Y-C)/(V_X+V_Y-2C)$ and minimum [variance](variance.md) $(V_XV_Y-C^2)/(V_X+V_Y-2C)$ when the denominator is positive. These are optimal among fixed linear unbiased combinations. Substituting weights estimated from the same observations need not preserve unbiasedness.

##### Cross-fitted combination of unbiased sample means

↑ **Parent:** [Minimum-variance combination of unbiased sample means](#minimum-variance-combination-of-unbiased-sample-means)

Split independent observational blocks into two folds. Use one fold to estimate the combination weight for the two [sample means](variance.md#sample-mean) in the other fold, and conversely. Each held-out combination is an [unbiased estimator](statistical-modelling.md#unbiased-estimator) conditionally on its training fold because its two held-out [sample means](variance.md#sample-mean) have the same [expectation](expected-value.md). A deterministic average of the two combinations remains unbiased. Under consistency of the moment estimates and balanced fold sizes, the weights approach those of the [minimum-variance combination of unbiased sample means](#minimum-variance-combination-of-unbiased-sample-means). Paired observations must stay together when splitting or [bootstrapping](statistical-modelling.md#bootstrapping-statistics) so their [covariance](variance.md#covariance) is preserved.

## Conditional Monte Carlo

↑ **Parent:** [Monte Carlo method](monte-carlo-method.md)

Replacing a simulated quantity $H$ by $E[H\mid\mathcal G]$ preserves its expectation and reduces variance by the [law of total variance](probability-theory.md#law-of-total-variance). This is [Rao-Blackwellization](probability-and-statistics.md#rao-blackwellization). For a random sum, conditioning on the count and all but one summand replaces an event indicator by a [cumulative distribution function](probability-distribution.md#cumulative-distribution-function) evaluation. The resulting estimator needs that conditional expectation to be computable.

## Box-Muller transform

↑ **Parent:** [Monte Carlo method](monte-carlo-method.md)

Independent [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) draws $U_1,U_2$ on $(0,1)$ produce independent standard [normal distribution](probability-distribution.md#normal-distribution) draws $X_1=\sqrt{-2\log U_1}\cos(2\pi U_2)$ and $X_2=\sqrt{-2\log U_1}\sin(2\pi U_2)$. The proof transforms an independent uniform angle and radial density $re^{-r^2/2}$ through the polar-coordinate Jacobian.

## Nested Monte Carlo

↑ **Parent:** [Monte Carlo method](monte-carlo-method.md)

[Nested Monte Carlo](#nested-monte-carlo) approximates an outer [expected value](expected-value.md) whose integrand contains another [expected value](expected-value.md). A nonlinear transformation, such as a [logarithm](calculus.md#logarithm), of an inner sample average usually introduces finite-sample bias. Increasing both sample sizes requires suitable integrability controls to establish consistency; an [unbiased estimator](statistical-modelling.md#unbiased-estimator) of the inner quantity does not make its [logarithm](calculus.md#logarithm) unbiased.

## Monte Carlo estimator

↑ **Parent:** [Monte Carlo method](monte-carlo-method.md)

A Monte Carlo estimator is a random approximation obtained from simulated samples, commonly a sample average or a weighted sample average.

### Summing before taking a mean changes Monte Carlo normalization

↑ **Parent:** [Monte Carlo estimator](#monte-carlo-estimator)

For $n$ observations, taking the mean of their scalar sum returns that sum, not their sample mean. If $a-b\overline H$ is unbiased for a target, replacing the mean by a sum gives expected value $a-bn\mathbb EH$ and multiplies its variance by $n^2$. A mean-zero [control variate](#control-variates) changes variance but cannot correct this missing normalization factor.

### Proposal-budget variance comparison of importance and rejection sampling

↑ **Parent:** [Monte Carlo estimator](#monte-carlo-estimator)

At equal proposal count, compare $\int\phi^2f^2/g-\theta^2$ for unnormalized importance sampling with $M(\int\phi^2f-\theta^2)$ for the accepted-sample mean. There is no universal ordering for nonzero target mean. For zero mean, the bounded-weight inequality gives importance sampling no larger asymptotic variance. Empty rejected samples and per-proposal computational cost are separate considerations.

#### Variance reversal under additive shifts of an importance-sampling integrand

↑ **Parent:** [Proposal-budget variance comparison of importance and rejection sampling](#proposal-budget-variance-comparison-of-importance-and-rejection-sampling)

An additive constant leaves the target variance and accepted-sample mean variance unchanged, but changes the variance of unnormalized importance sampling because its random weights do not sum to one. With g uniform on (0,1), f(x)=2x and M=2, phi(x)=x gives importance variance 16/45 versus rejection proposal-budget variance 1/9. Replacing phi by x-1 gives importance variance 1/45 with the same rejection variance, reversing preference.

### Control variates

↑ **Parent:** [Monte Carlo estimator](#monte-carlo-estimator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Control_variates)

A control variate is a [random variable](random-variable.md) with known [expected value](expected-value.md) whose centered value is subtracted from a [Monte Carlo estimator](#monte-carlo-estimator) to reduce its [variance](variance.md). For a mean-zero vector $G$, put $S=\operatorname{Cov}(G)$ and $c=\operatorname{Cov}(G,H)$. When $S$ is invertible, the optimal estimator averages $H-c^TS^{-1}G$ and has variance $(\operatorname{Var}(H)-c^TS^{-1}c)/N$ for $N$ independent draws. Improvement is strict exactly when $c\ne0$.

#### Multivariate control variates

↑ **Parent:** [Control variates](#control-variates)

If $Y$ is an unbiased estimator and a vector $C$ has known mean, then $Y-\beta^T(C-\mathbb EC)$ remains unbiased for a deterministic coefficient vector. Its variance is $\operatorname{Var}Y-2\beta^T c+\beta^T\Sigma\beta$, where $c=\operatorname{Cov}(C,Y)$ and $\Sigma=\operatorname{Cov}(C)$. For invertible $\Sigma$, completing the square gives the displayed optimum and minimum variance $\operatorname{Var}Y-c^T\Sigma^{-1}c$. With singular $\Sigma$, use a generalized inverse on its range. Estimating coefficients from the same simulation can introduce finite-sample bias; fixed pilot coefficients or independent training preserve the elementary unbiasedness assertion.

#### Cauchy tail control variate on a bounded interval

↑ **Parent:** [Control variates](#control-variates)

For $Y$ uniform on $(0,2)$, put $g(y)=1/(\pi(1+y^2))$ and $H(y)=y^2-4/3$. Then $\mathbb EH=0$, and $1/2-2\overline{g-\beta H}$ estimates the standard [Cauchy distribution](probability-distribution.md#cauchy-distribution) probability above two. Its variance is $4\operatorname{Var}(g-\beta H)/n$, minimized by the displayed coefficient. Here $\operatorname{Var}(H)=64/45$ and $\operatorname{Cov}(g,H)=1/\pi-7\arctan(2)/(6\pi)$, so the optimal coefficient is negative. A coefficient estimated using a separate pilot can be fixed for a fresh unbiased production sample.

#### Posterior score control variate

↑ **Parent:** [Control variates](#control-variates)

If a smooth [posterior density](bayesian-statistics.md#posterior-density) has vanishing boundary terms, its [log-posterior](bayesian-statistics.md#log-posterior) gradient satisfies $\mathbb E[g]=0$ and

$$
\mathbb E[g(\beta)h(\beta)]=-\mathbb E[\nabla h(\beta)].
$$

This is a posterior integration-by-parts identity; it concerns differentiation in the random parameter, distinct from the usual [mean-zero score identity](statistical-modelling.md#mean-zero-score-identity) for sampling distributions. It makes $g$ a vector [control variate](#control-variates). Finite moments and known coefficients preserve unbiasedness of the [Monte Carlo estimator](#monte-carlo-estimator).

## Monte Carlo error

↑ **Parent:** [Monte Carlo method](monte-carlo-method.md)

Monte Carlo error is the random difference between a simulation estimate and the exact quantity it approximates. For an average of independent finite-variance draws, its standard deviation is proportional to the inverse square root of the number of draws.

### Monte Carlo standard error

↑ **Parent:** [Monte Carlo error](#monte-carlo-error)

The [Monte Carlo standard error](#monte-carlo-standard-error) estimates the [standard deviation](variance.md#standard-deviation) of a simulation-based estimate across repeated simulation runs. For an average of $N$ [independent random variables](random-variable.md#independent-random-variables) with finite [variance](variance.md) $\sigma_h^2$, it is $\sigma_h/\sqrt N$. Under a suitable [central limit theorem](convergence-of-random-variables.md#central-limit-theorem) for [Markov chain Monte Carlo](bayesian-statistics.md#markov-chain-monte-carlo), correlated draws instead give the approximation $\sigma_h/\sqrt{N_{\rm eff}}$, where $N_{\rm eff}$ is the [effective sample size of a Markov chain](bayesian-statistics.md#effective-sample-size-of-a-markov-chain) for the particular estimated function $h$. This measures numerical uncertainty in an estimate, not uncertainty in the unknown parameter itself.

## Rejection sampling

↑ **Parent:** [Monte Carlo method](monte-carlo-method.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rejection_sampling)

Suppose $f$ is a target probability density and $h$ is a proposal density with $f(x)\leq Mh(x)$. Draw $X\sim h$ and an independent $U\sim\operatorname{Uniform}[0,1]$, and accept $X$ when

$$
U\leq\frac{f(X)}{Mh(X)}.
$$

The accepted value has density $f$, the acceptance probability is $1/M$, and the expected number of proposals is $M$.

### Acceptance mass for an unnormalized rejection envelope

↑ **Parent:** [Rejection sampling](#rejection-sampling)

If $f\geq0$, $C=\int f\in(0,\infty)$ and $f(x)\leq Mg(x)$ for a proposal [probability density function](continuous-probability-distribution.md#probability-density-function) $g$, accept a proposal $Y$ when an [independent](random-variable.md#independent-random-variables) [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) value is at most $f(Y)/(Mg(Y))$. Integrating the joint acceptance [probability density function](continuous-probability-distribution.md#probability-density-function) gives $p_{\rm acc}=C/M$ and conditional accepted [probability density function](continuous-probability-distribution.md#probability-density-function) $f/C$. For $n$ [independent](random-variable.md#independent-random-variables) proposals the accepted count has [binomial distribution](discrete-probability-distribution.md#binomial-distribution) with parameters $n,C/M$.

### Truncated gamma rejection sampling with a Pareto envelope

↑ **Parent:** [Rejection sampling](#rejection-sampling)

For target density proportional to $x^{\alpha-1}e^{-\beta x}$ on $x>a>0$, use the [Pareto distribution](continuous-probability-distribution.md#pareto-distribution) proposal $g(x)=ba^bx^{-b-1}$ with $b>0$. Its density ratio is proportional to $x^{\alpha+b}e^{-\beta x}$, maximized at $(\alpha+b)/\beta$ if that point exceeds $a$. The tight envelope yields the highest acceptance probability for this fixed proposal. An inverse draw is $aU^{-1/b}$ with $U$ [uniformly distributed](continuous-probability-distribution.md#continuous-uniform-distribution) on $(0,1)$.

### Uniform-envelope rejection sampling for a beta distribution

↑ **Parent:** [Rejection sampling](#rejection-sampling)

For $a,b>1$, the maximum of $r$ on $[0,1]$ occurs at $(a-1)/(a+b-2)$. If one parameter is one, the maximum is attained at the corresponding endpoint; if both are one, $r$ is constant. Let $M=\sup r$. Accept an [independent](random-variable.md#independent-random-variables) [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) proposal $X$ when another uniform draw is at most $r(X)/M$. The accepted [probability density function](continuous-probability-distribution.md#probability-density-function) is the [beta distribution](probability-distribution.md#beta-distribution), and acceptance [probability](probability-theory.md#probability) is $B(a,b)/M$.

### Bayesian rejection sampling for a segregating-site count

↑ **Parent:** [Rejection sampling](#rejection-sampling)

With proper prior $\pi(\theta)$ independent of the neutral [Kingman's coalescent](continuous-time-markov-chain.md#kingman-s-coalescent) times, propose $(\theta,T)$ from their joint prior and accept with probability $e^{-\theta L/2}(\theta L/2)^k/k!$. The accepted density is proportional to the prior times the observed-count likelihood, hence is the posterior given $S=k$. The acceptance rate is the prior predictive probability $P(S=k)$. For $k>0$, divide the acceptance function by its maximum $M_k=e^{-k}k^k/k!$, achieved at $\theta L/2=k$, to improve the rate to $P(S=k)/M_k$ without altering the accepted distribution. For $k=0$, $M_0=1$.

#### Joint posterior of mutation rate and coalescent times

↑ **Parent:** [Bayesian rejection sampling for a segregating-site count](#bayesian-rejection-sampling-for-a-segregating-site-count)

For a proper [prior distribution](bayesian-statistics.md#prior-probability) $\pi(\theta)$ independent of coalescent times $T$, let $q(T)=\prod_{j=2}^n\lambda_j e^{-\lambda_jT_j}$ with $\lambda_j=\binom j2$ and $L=\sum jT_j$. Observing $S=k$ under an [infinite sites mutation model](population-genetics.md#infinite-sites-mutation-model) gives [posterior density](bayesian-statistics.md#posterior-density) $\pi(\theta)q(T)e^{-\theta L/2}(\theta L/2)^k/(k!m_k)$, where $m_k$ is the prior predictive [probability](probability-theory.md#probability) of $S=k$. Multiplication by the conditional Poisson mass and normalization is an application of [Bayes' theorem](probability-theory.md#bayes-theorem).

// Target: statistical-inference.bigb

### Match-biased reshuffling preserves uniform rank marginals

↑ **Parent:** [Rejection sampling](#rejection-sampling)

Accepting a fresh uniform deck permutation with a probability depending only on whether its endpoint ranks match preserves uniform individual rank marginals by symmetry. It changes their joint law. For four cards of each of thirteen ranks and rejection probability $p$ on a mismatch, the accepted matching probability is $1/(17-16p)$. The two accepted ranks are independent precisely at $p=1/4$; equality of marginals alone does not imply independence.

### Exponential-envelope rejection sampling for a chi-squared variable

↑ **Parent:** [Rejection sampling](#rejection-sampling)

Write $a=\nu/2$. Against an [exponential distribution](continuous-probability-distribution.md#exponential-distribution) proposal of mean $\nu$, the [chi-squared distribution](probability-distribution.md#chi-squared-distribution) density has envelope constant $M=a^ae^{1-a}/\Gamma(a)$. The density ratio divided by $M$ is $\exp((a-1)(\log(y/\nu)-y/\nu+1))$. Thus generate $Y=-\nu\log U$ and accept when $\log V\leq(a-1)(\log(Y/\nu)-Y/\nu+1)$ for independent [uniform distributions](continuous-probability-distribution.md#continuous-uniform-distribution). The inequality $\log t\leq t-1$ validates the acceptance probability. The accepted [probability density function](continuous-probability-distribution.md#probability-density-function) is the target because [rejection sampling](#rejection-sampling) weights the proposal by its target-to-envelope ratio.

### Ratio-of-uniforms method

↑ **Parent:** [Rejection sampling](#rejection-sampling)

For a nonnegative integrable function $h$ with integral $Z$, its ratio-of-uniforms region has area $Z/2$. A uniform point in the region transforms under $v=ux$ with [Jacobian determinant](multivariable-calculus.md#jacobian-determinant) $u$; integrating $2u/Z$ over $0<u\le\sqrt{h(x)}$ gives density $h(x)/Z$. A rectangle containing the region gives a practical [rejection sampling](#rejection-sampling) algorithm using only uniform random variables, with acceptance $Z/(2\operatorname{area}(B))$.

#### Laplace ratio-of-uniforms envelope

↑ **Parent:** [Ratio-of-uniforms method](#ratio-of-uniforms-method)

For the unnormalized [Laplace distribution](continuous-probability-distribution.md#laplace-distribution) [probability density function](continuous-probability-distribution.md#probability-density-function) $h(x)=e^{-|x-1|/2}$, the [ratio-of-uniforms method](#ratio-of-uniforms-method) uses $0<u\leq\sqrt{h(v/u)}$. The maximum of $h$ is one. On $x\leq0$, the maximum of $x^2h(x)$ occurs at $x=-4$ and equals $16e^{-5/2}$. On $x\geq0$, it occurs at $x=4$ and equals $16e^{-3/2}$. Thus the displayed rectangle contains the region. Its area is $4(e^{-3/4}+e^{-5/4})$, while the target region has area $\tfrac12\int h=2$. Uniform proposals in the rectangle, accepted when $u^2\leq h(v/u)$, therefore return the correct [Laplace distribution](continuous-probability-distribution.md#laplace-distribution) with acceptance [probability](probability-theory.md#probability) $[2(e^{-3/4}+e^{-5/4})]^{-1}$.

#### Normal ratio-of-uniforms envelope

↑ **Parent:** [Ratio-of-uniforms method](#ratio-of-uniforms-method)

For the unnormalized [normal density](probability-distribution.md#normal-density) $h(x)=e^{-x^2/(2\sigma^2)}$, the smallest axis-aligned envelope is $0<u<1$ and $|v|\le\sigma\sqrt{2/e}$. The boundary reaches that width at $u=e^{-1/2}$. Region area is $\sigma\sqrt{\pi/2}$, so the acceptance rate is $\sqrt{\pi e}/4$, independently of $\sigma$. Multiplying $h$ by a positive constant rescales both coordinates and their areas consistently.

#### Finite-area envelope for a ratio-of-uniforms region

↑ **Parent:** [Ratio-of-uniforms method](#ratio-of-uniforms-method)

A finite bounding rectangle exists when $\sqrt{h(x)}$ and $x\sqrt{h(x)}$ are bounded. This is not automatic for every [probability density function](continuous-probability-distribution.md#probability-density-function): tails proportional to $(1+|x|)^{-3/2}$ give an unbounded second coordinate. In principle any finite-area measurable region has an open envelope of finite area, decomposable up to null boundaries into disjoint dyadic rectangles. Select a rectangle with probability proportional to its area, then sample its two coordinates uniformly and reject outside the target region. The accepted point is uniform on the region, with acceptance equal to the ratio of their areas. Constructing an effective envelope remains a density-specific computational step.

### Normal rejection sampling with an exponential envelope

↑ **Parent:** [Rejection sampling](#rejection-sampling)

For the [half-normal distribution](probability-distribution.md#half-normal-distribution), the density ratio to $\operatorname{Exp}(\lambda)$ is maximized at $y=\lambda$. Completing the square gives the envelope constant above and acceptance [probability](probability-theory.md#probability) $e^{-(y-\lambda)^2/2}$. Its logarithmic derivative is $\lambda-1/\lambda$, so the optimal rate is $\lambda=1$. Give an accepted nonnegative value an independent fair sign to obtain the [standard normal distribution](probability-distribution.md#standard-normal-distribution). The expected number of proposals is $M$, while the [probability](probability-theory.md#probability) of rejecting one proposal is $1-1/M$; these are different quantities.

### Marsaglia polar method

↑ **Parent:** [Rejection sampling](#rejection-sampling)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Marsaglia_polar_method)

Reject pairs of independent uniform coordinates from the square until their squared radius $S$ lies in $(0,1)$. Multiply each coordinate by $\sqrt{-2\log S/S}$ to obtain two independent variables with the [standard normal distribution](probability-distribution.md#standard-normal-distribution). Squaring either gives a chi-squared variable with one degree of freedom.

### Binomial count and iid values in fixed-budget rejection sampling

↑ **Parent:** [Rejection sampling](#rejection-sampling)

For n independent proposals and an envelope constant $M$, each rejection decision succeeds with probability $1/M$. The accepted count is Bin(n,1/M). Conditional on any acceptance pattern, the accepted values have independent target density f; summing over patterns preserves that product law conditional on the count. The empty-output probability is $(1-1/M)^n$.

#### Random-count central limit theorem for accepted rejection samples

↑ **Parent:** [Binomial count and iid values in fixed-budget rejection sampling](#binomial-count-and-iid-values-in-fixed-budget-rejection-sampling)

Conditional iid accepted values have the ordinary target-sample CLT at scale $\sqrt N$. Since $N/n\to1/M$, the same estimator has asymptotic variance $M\operatorname{Var}_f\phi$ at scale $\sqrt n$. The centered count has limiting variance $(1/M)(1-1/M)$. Any fixed convention on an empty output is asymptotically negligible.

### Rejected-proposal distribution

↑ **Parent:** [Rejection sampling](#rejection-sampling)

With normalized densities $f,g$ and envelope $f\leq Mg$, $M>1$, conditioning a proposal on rejection gives density $r=(Mg-f)/(M-1)$. It can be used as an [importance sampling](#importance-sampling) proposal only if it covers the relevant target support. If $Mg=f$ on a set of positive target mass, rejected draws never visit that set.

### Adaptive rejection sampling

↑ **Parent:** [Rejection sampling](#rejection-sampling)

Adaptive rejection sampling builds a piecewise linear upper envelope for a differentiable [log-concave probability density](continuous-probability-distribution.md#log-concave-probability-density), samples from its piecewise exponential form, and accepts with the target-to-envelope ratio. Adding evaluated points improves the envelope without changing the target distribution. Initial tangent slopes must yield integrable tails. The accepted draws are exact samples, unlike a finite run of [Markov chain Monte Carlo](bayesian-statistics.md#markov-chain-monte-carlo).

## Importance sampling

↑ **Parent:** [Monte Carlo method](monte-carlo-method.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Importance_sampling)

To estimate $\mathbb E_f[g(X)]$, sample $Y_1,\ldots,Y_m$ independently from a reference density $h$ whose support covers that of $gf$, and use

$$
\frac1m\sum_{i=1}^m g(Y_i)\frac{f(Y_i)}{h(Y_i)}.
$$

The summands have expectation $\int g(x)f(x)\,dx$, and the [strong law of large numbers](convergence-of-random-variables.md#strong-law-of-large-numbers) gives almost-sure convergence under integrability.

### Importance sampling of a Cauchy tail

↑ **Parent:** [Importance sampling](#importance-sampling)

For $U$ uniform on $(0,1)$, $Y$ has density $q(y)=2y^{-2}$ on $y\ge2$. The [importance sampling](#importance-sampling) weight for the standard [Cauchy distribution](probability-distribution.md#cauchy-distribution) tail is $W=f(Y)/q(Y)$, and its expectation is the target tail [probability](probability-theory.md#probability). Writing $A=\arctan(1/2)$ gives $\mathbb EW=A/\pi$ and $\mathbb EW^2=(A+2/5)/(4\pi^2)$ by integrating $y^2/(1+y^2)^2$. The weight varies only between $2/(5\pi)$ and $1/(2\pi)$, making its [variance](variance.md) much smaller than that of a rare-event indicator. This is a comparison of sampling [variances](variance.md), not a deterministic ordering of every pair of empirical [variance](variance.md) estimates.

### Rao-Blackwell identity for a fixed-denominator rejection estimator

↑ **Parent:** [Importance sampling](#importance-sampling)

For rejection indicators with conditional acceptance $f(X_i)/(Mg(X_i))$, the conditional expectation of $(M/n)\sum_iI_i\phi(X_i)$ given all proposals is the unnormalized importance estimator. The [Rao-Blackwell theorem](probability-and-statistics.md#rao-blackwell-theorem) reduces variance relative to that fixed-denominator estimator. It gives no such automatic comparison with the accepted-sample mean, whose denominator is the random count.

### Bounded-weight importance-sampling moment bound

↑ **Parent:** [Importance sampling](#importance-sampling)

If $f\leq Mg$, the importance weight $w=f/g$ is bounded by $M$, and $\mathbb E_g[\phi^2w^2]\leq M\mathbb E_f\phi^2$. A finite target second moment therefore guarantees finite variance and the iid central limit theorem for the unnormalized importance-sampling average. Its proposal-budget variance is $\mathbb E_g[\phi^2w^2]-(\mathbb E_f\phi)^2$.

### Minimum-variance importance distribution

↑ **Parent:** [Importance sampling](#importance-sampling)

For $\mu=\int hf$ and $0<A=\int|h|f<\infty$, the proposal $q_*=|h|f/A$ minimizes the [variance](variance.md) of the ordinary unbiased [importance sampling](#importance-sampling) estimator. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $\int h^2f^2/q\geq A^2$, so the minimum [variance](variance.md) for $n$ independent samples is $(A^2-\mu^2)/n$. The proposal need only cover the nonzero integrand.

### Support condition for importance sampling

↑ **Parent:** [Importance sampling](#importance-sampling)

An [importance sampling](#importance-sampling) proposal $q$ must be positive wherever the target-weighted integrand can contribute. The usual sufficient condition is that the target probability is absolutely continuous with respect to $q$. Otherwise multiplying observed draws by $f/q$ cannot recover a missing part of the integral. A strict rejection envelope supplies this condition for the [rejected-proposal distribution](#rejected-proposal-distribution).

### Importance weight

↑ **Parent:** [Importance sampling](#importance-sampling)

For target density $f$ and proposal density $h$, the importance weight is the density ratio $w(x)=f(x)/h(x)$ wherever the target is supported.

### Self-normalized importance sampling

↑ **Parent:** [Importance sampling](#importance-sampling)

For an unnormalized target density, self-normalized importance sampling uses weights $w_i=f(Y_i)/h(Y_i)$ and estimates expectations by $\sum_iw_ig(Y_i)/\sum_iw_i$. Resampling a point $Y_i$ with probability proportional to $w_i$ produces the associated weighted empirical distribution.

### Optimal importance density for a single integral

↑ **Parent:** [Importance sampling](#importance-sampling)

For estimating $I=\int g(x)f(x)\,dx$ by the unbiased importance estimator $g(Y)f(Y)/q(Y)$, the proposal minimizing variance is

$$
q^*(x)=\frac{|g(x)|f(x)}{\int |g(u)|f(u)\,du}.
$$

This follows from the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality). Its normalizing constant and dependence on the particular integrand often make it impractical.

### Effective sample size of importance sampling

↑ **Parent:** [Importance sampling](#importance-sampling)

For normalized importance weights $w_i$, the standard effective sample size is $K_{\mathrm{eff}}=1/\sum_iw_i^2$.

## ↑ Ancestors (4)

1. [Probability and statistics](probability-and-statistics.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (5)

- [Central limit theorem](convergence-of-random-variables.md#central-limit-theorem)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2024/paper-2.md#b4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-34.md#2/h/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208.md#5/d/solution)
