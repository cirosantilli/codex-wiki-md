# Exponential family

↑ **Parent:** [Statistical modelling](statistical-modelling.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exponential_family)

A density $h(y)\exp\{\theta T(y)-A(\theta)\}$ has sufficient statistic $T$ and cumulant function $A$.

**Table of contents**

- [Curved exponential family](#curved-exponential-family)
  - [Conditional scale density in a curved Gaussian family](#conditional-scale-density-in-a-curved-gaussian-family)
- [Minimal exponential family](#minimal-exponential-family)
- [Natural exponential family](#natural-exponential-family)
  - [Convex support of an exponential family](#convex-support-of-an-exponential-family)
  - [Regular natural exponential family](#regular-natural-exponential-family)
  - [Full natural exponential family](#full-natural-exponential-family)
    - [Maximum likelihood existence in a full regular natural exponential family](#maximum-likelihood-existence-in-a-full-regular-natural-exponential-family)
- [Normal natural-mean parameter ratio estimator](#normal-natural-mean-parameter-ratio-estimator)
- [Log-density domination in an exponential family](#log-density-domination-in-an-exponential-family)
- [Conjugate prior](#conjugate-prior)
  - [Normal-gamma distribution](#normal-gamma-distribution)
  - [Gamma rate gamma conjugacy](#gamma-rate-gamma-conjugacy)
  - [Uniform-Pareto conjugacy](#uniform-pareto-conjugacy)
    - [Uniform-Pareto model evidence](#uniform-pareto-model-evidence)
  - [Gamma scale inverse-gamma conjugacy](#gamma-scale-inverse-gamma-conjugacy)
    - [Exact Bühlmann credibility for gamma claims](#exact-buhlmann-credibility-for-gamma-claims)
  - [Normal-inverse-gamma prior](#normal-inverse-gamma-prior)
  - [Natural conjugate prior](#natural-conjugate-prior)
    - [Natural conjugate credibility identity](#natural-conjugate-credibility-identity)
      - [Endpoint control for a Laplace-family conjugate posterior](#endpoint-control-for-a-laplace-family-conjugate-posterior)
- [Natural parameter of an exponential family](#natural-parameter-of-an-exponential-family)
  - [Natural parameter space](#natural-parameter-space)
- [Cumulant function of an exponential family](#cumulant-function-of-an-exponential-family)
  - [Exponential-family derivative identities](#exponential-family-derivative-identities)
  - [Mean parameter of an exponential family](#mean-parameter-of-an-exponential-family)
    - [Interior moment matching in a finite exponential family](#interior-moment-matching-in-a-finite-exponential-family)
- [Inverse Gaussian distribution](#inverse-gaussian-distribution)
  - [Inverse Gaussian shape estimation and nuisance orthogonality](#inverse-gaussian-shape-estimation-and-nuisance-orthogonality)
  - [Inverse Gaussian sum closure](#inverse-gaussian-sum-closure)
    - [Exact saddlepoint density of an inverse Gaussian sum](#exact-saddlepoint-density-of-an-inverse-gaussian-sum)
  - [Chi-squared transform of an inverse Gaussian variable](#chi-squared-transform-of-an-inverse-gaussian-variable)
  - [Reciprocal-root inverse Gaussian sampler](#reciprocal-root-inverse-gaussian-sampler)
    - [Stable root evaluation for inverse Gaussian sampling](#stable-root-evaluation-for-inverse-gaussian-sampling)
- [Exponential-family deviance](#exponential-family-deviance)
  - [Scaled deviance](#scaled-deviance)
- [Negative binomial exponential family](#negative-binomial-exponential-family)
- [Exponential dispersion model](#exponential-dispersion-model)
  - [Exponential dispersion family of order one](#exponential-dispersion-family-of-order-one)
  - [Dispersion parameter](#dispersion-parameter)
    - [Underdispersion](#underdispersion)
    - [Overdispersion](#overdispersion)
  - [Variance function](#variance-function)

## Curved exponential family

↑ **Parent:** [Exponential family](exponential-family.md)

A $(p,q)$ curved [exponential family](exponential-family.md), with $q<p$, restricts a $p$-parameter canonical family to a smooth rank-$q$ parameter surface, usually a nonaffine surface. For example, $N(\mu,\mu^2)$ with $\mu>0$ has sufficient statistics $(Y,Y^2)$ and natural parameters $(1/\mu,-1/(2\mu^2))$, constrained by $\eta_2=-\eta_1^2/2$. Canonical concavity in the ambient parameters need not imply concavity along the curved parameter surface.

### Conditional scale density in a curved Gaussian family

↑ **Parent:** [Curved exponential family](#curved-exponential-family)

For [independent](random-variable.md#independent-random-variables) $N(\mu,\mu^2)$ observations with $\mu>0$, the [sufficient statistics](probability-and-statistics.md#sufficient-statistic) are their sum and squared norm. Condition on $a=\sqrt n\,\|y\|/\sum_i y_i>0$ and write $v=\widehat\mu=\|y\|/(q\sqrt n)$, where $q=(\sqrt{1+4a^2}+1)/(2a)$. [Polar coordinates](calculus.md#polar-coordinates) supply radial measure $\|y\|^{n-1}d\|y\|$, while the conditional angular factor does not depend on $\mu$. This proves the displayed shape. Its normalization depends on $a,n$ but not $\mu$ after the substitution $v=\mu z$, and agrees with the normalized [P-star approximation](probability-theory.md#p-star-approximation).

## Minimal exponential family

↑ **Parent:** [Exponential family](exponential-family.md)

An order-$p$ [exponential family](exponential-family.md) is minimal if no nonzero linear combination of its $p$ canonical [sufficient statistics](probability-and-statistics.md#sufficient-statistic) is almost surely constant under the base measure. Equivalently, its sufficient-statistic support lies in no proper affine hyperplane. Its [cumulant function](#cumulant-function-of-an-exponential-family) then has positive-definite [Hessian matrix](calculus.md#hessian-matrix) on the interior natural domain, because that Hessian is a [covariance matrix](variance.md#covariance-matrix).

## Natural exponential family

↑ **Parent:** [Exponential family](exponential-family.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Natural_exponential_family)

A natural [exponential family](exponential-family.md) uses its observation vector itself as the canonical [sufficient statistic](probability-and-statistics.md#sufficient-statistic). Its [cumulant function](#cumulant-function-of-an-exponential-family) is $\kappa(\theta)=\log\int h(y)e^{\theta^Ty}\,d\nu(y)$ and its [natural parameter space](#natural-parameter-space) consists of parameters for which this integral is finite. On the interior, differentiating gives [mean parameter of an exponential family](#mean-parameter-of-an-exponential-family) $\nabla\kappa$ and [covariance matrix](variance.md#covariance-matrix) $\nabla^2\kappa$.

### Convex support of an exponential family

↑ **Parent:** [Natural exponential family](#natural-exponential-family)

The convex support is the closed [convex hull](mathematical-optimization.md#convex-hull) of the canonical sufficient-statistic support. For a [minimal exponential family](#minimal-exponential-family) it has nonempty interior. Means at finite interior natural parameters lie in that interior, because a supporting hyperplane at a boundary mean would force the sufficient statistic itself onto that hyperplane.

### Regular natural exponential family

↑ **Parent:** [Natural exponential family](#natural-exponential-family)

A [natural exponential family](#natural-exponential-family) is regular when its parameter space is open. In a full regular family, differentiation under the normalizing integral is justified locally by exponential moments in a neighbourhood. Regularity does not guarantee that every possible data set has a finite [maximum-likelihood estimator](statistical-modelling.md#maximum-likelihood-estimator).

### Full natural exponential family

↑ **Parent:** [Natural exponential family](#natural-exponential-family)

A [natural exponential family](#natural-exponential-family) is full when its parameter set is the entire [natural parameter space](#natural-parameter-space), with no restrictions on the allowable canonical parameters beyond finiteness of its normalizing integral. Fullness must not be confused with minimality or regularity.

#### Maximum likelihood existence in a full regular natural exponential family

↑ **Parent:** [Full natural exponential family](#full-natural-exponential-family)

In a full regular [minimal exponential family](#minimal-exponential-family), a finite [maximum-likelihood estimator](statistical-modelling.md#maximum-likelihood-estimator) exists precisely when the observed sufficient-statistic mean is in the interior of the [convex support of an exponential family](#convex-support-of-an-exponential-family). It is unique because the log likelihood is strictly concave. For an interior mean, positive base-measure mass near finitely many support points surrounding the mean makes $\kappa(\theta)-\theta^T\bar Y$ grow at least linearly as $\|\theta\|\to\infty$. At a finite boundary of the full open natural domain, the normalizing integral diverges. Thus the likelihood attains its maximum in the domain. On a boundary face, no finite parameter can have the required mean. A regular restriction should instead use the exact mean-image criterion. These full-family conventions are also discussed in [Geyer's exponential-family lecture notes](https://www.stat.umn.edu/geyer/5421/notes/expfam.html).

## Normal natural-mean parameter ratio estimator

↑ **Parent:** [Exponential family](exponential-family.md)

For independent $N(\mu,v)$ observations with unknown mean and variance, the first natural parameter is $\phi_1=\mu/v$. Its [maximum-likelihood estimator](statistical-modelling.md#maximum-likelihood-estimator) is $\bar X/[n^{-1}\sum_i(X_i-\bar X)^2]$. The [delta method](statistical-inference.md#delta-method) and independent asymptotic mean/variance errors give limiting variance $v^{-1}+2\mu^2v^{-2}$ for $\sqrt n(\widehat\phi_1-\phi_1)$. Knowing $v$ removes the second contribution and makes the estimator exactly normal with variance $1/(nv)$.

## Log-density domination in an exponential family

↑ **Parent:** [Exponential family](exponential-family.md)

On a bounded parameter set, $\log f_\theta(x)=\theta x-K(\theta)+\log f_0(x)$ has an [integrable envelope of a function class](convergence-of-random-variables.md#integrable-envelope-of-a-function-class) whenever $K$ is bounded and $|X|+|\log f_0(X)|$ is integrable under the sampling law. A [compact](topology.md#compact-space) subset of the interior natural-parameter domain bounds the [cumulant function of an exponential family](#cumulant-function-of-an-exponential-family) and provides moments under model sampling; log-base-density [integrability](measure-theory.md#integrability) is an additional condition.

## Conjugate prior

↑ **Parent:** [Exponential family](exponential-family.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conjugate_prior)

A conjugate prior belongs to a family whose posterior remains in that family after multiplication by the likelihood.

### Normal-gamma distribution

↑ **Parent:** [Conjugate prior](#conjugate-prior)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal-gamma_distribution)

A normal-gamma [conjugate prior](#conjugate-prior) for the mean $\mu$ and [precision parameter](statistical-modelling.md#precision-parameter) $\tau$ of a [Gaussian distribution](probability-theory.md#normal-distribution) specifies a [Gamma distribution](continuous-probability-distribution.md#gamma-distribution) $\tau\sim\operatorname{Gamma}(\alpha,\beta)$ in the shape-rate convention and a conditional [Gaussian distribution](probability-theory.md#normal-distribution) $\mu\mid\tau\sim N(\mu_0,(K\tau)^{-1})$. Its joint [probability density function](continuous-probability-distribution.md#probability-density-function) is proportional to $\tau^{\alpha-1}\sqrt\tau\exp[-\beta\tau-K\tau(\mu-\mu_0)^2/2]$, with $\alpha,\beta,K>0$. For $n$ independent observations with [Gaussian distribution](probability-theory.md#normal-distribution) $N(\mu,\tau^{-1})$, multiplication by the [likelihood](statistical-modelling.md#likelihood-function) and completing the square gives

$$
K_n=K+n,\quad\mu_n=(K\mu_0+n\bar x)/(K+n),\quad\alpha_n=\alpha+n/2,
$$

and $\beta_n=\beta+\sum_i(x_i-\bar x)^2/2+Kn(\bar x-\mu_0)^2/[2(K+n)]$. The identity behind conjugacy is $K(\mu-\mu_0)^2+\sum_i(x_i-\mu)^2=(K+n)(\mu-\mu_n)^2+\sum_i(x_i-\bar x)^2+Kn(\bar x-\mu_0)^2/(K+n)$.

### Gamma rate gamma conjugacy

↑ **Parent:** [Conjugate prior](#conjugate-prior)

Conditionally independent [gamma distributions](continuous-probability-distribution.md#gamma-distribution) with known shape $r$ and unknown rate $\Theta$ have likelihood proportional to $\Theta^{nr}e^{-\Theta\sum_i x_i}$. A [gamma distribution](continuous-probability-distribution.md#gamma-distribution) prior of shape $A$ and rate $B$ therefore updates to shape $A+nr$ and rate $B+\sum_i x_i$. When $A+nr>1$, the [posterior mean](statistical-inference.md#posterior-mean) of the conditional claim mean $r/\Theta$ is $r(B+\sum_i x_i)/(A+nr-1)$. For $A=rk+1$ and $B=k\mu$, this is a [credibility estimate](actuarial-statistics.md#credibility-estimate) with weight $n/(n+k)$. It is the reciprocal-rate version of [gamma scale inverse-gamma conjugacy](#gamma-scale-inverse-gamma-conjugacy).

### Uniform-Pareto conjugacy

↑ **Parent:** [Conjugate prior](#conjugate-prior)

A [Pareto distribution](continuous-probability-distribution.md#pareto-distribution) prior for the upper limit of independent [uniform distributions](continuous-probability-distribution.md#continuous-uniform-distribution) remains Pareto after observing data. The likelihood adds the sample size to the shape and replaces the lower bound by the larger of the prior bound and sample maximum.

#### Uniform-Pareto model evidence

↑ **Parent:** [Uniform-Pareto conjugacy](#uniform-pareto-conjugacy)

For positive observations and $m=\max(\beta,\max_jy_j)$, the [Bayesian model evidence](statistical-inference.md#bayesian-model-evidence) follows by integrating the [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) likelihood against a [Pareto distribution](continuous-probability-distribution.md#pareto-distribution) prior. For independent groups with shared fixed [hyperparameters](statistical-inference.md#hyperparameter), these evidences multiply. The resulting [hyperparameter](statistical-inference.md#hyperparameter) log likelihood is $I\log\alpha-\sum_i\log(\alpha+n_i)-\alpha\sum_i\log(m_i/\beta)$ up to a constant.

### Gamma scale inverse-gamma conjugacy

↑ **Parent:** [Conjugate prior](#conjugate-prior)

For conditionally independent [gamma distribution](continuous-probability-distribution.md#gamma-distribution) observations of known shape $\alpha$ and unknown scale $\Theta$, an [inverse-gamma distribution](continuous-probability-distribution.md#inverse-gamma-distribution) prior with shape $k$ and scale $\lambda$ gives an [inverse-gamma distribution](continuous-probability-distribution.md#inverse-gamma-distribution) posterior with shape $k+n\alpha$ and scale $\lambda+\sum_jx_j$. The [posterior mean](statistical-inference.md#posterior-mean) of the conditional claim [expected value](probability-theory.md#expected-value) $\alpha\Theta$ is $\alpha(\lambda+\sum_jx_j)/(k+n\alpha-1)$ when the denominator is positive.

<h4 id="exact-buhlmann-credibility-for-gamma-claims">Exact Bühlmann credibility for gamma claims</h4>

↑ **Parent:** [Gamma scale inverse-gamma conjugacy](#gamma-scale-inverse-gamma-conjugacy)

With the [gamma scale inverse-gamma conjugacy](#gamma-scale-inverse-gamma-conjugacy) model and prior shape $k>2$, the [Bühlmann model](actuarial-statistics.md#buhlmann-model) has $v/a=(k-1)/\alpha$. Its [Bühlmann credibility premium](actuarial-statistics.md#buhlmann-credibility-premium) equals $\alpha(\lambda+\sum_jX_j)/(k+n\alpha-1)$, exactly the [Bayes estimator under squared error loss](statistical-inference.md#bayes-estimator-under-squared-error-loss) of $\alpha\Theta$. Equality holds because the [posterior mean](statistical-inference.md#posterior-mean) is already affine in the observed [sample mean](variance.md#sample-mean).

### Normal-inverse-gamma prior

↑ **Parent:** [Conjugate prior](#conjugate-prior)

For a [normal linear model](statistical-modelling.md#normal-linear-model) with coefficient vector $\eta$ and residual [variance](variance.md) $\sigma^2$, a normal-inverse-gamma prior has $\eta\mid\sigma^2\sim N(m,\sigma^2V)$ and $\sigma^2\sim\operatorname{IG}(a,b)$, with $V$ a [positive-definite matrix](linear-algebra.md#positive-definite-matrix) and $a,b>0$. The inverse-gamma density is proportional to $(\sigma^2)^{-a-1}e^{-b/\sigma^2}$. Multiplying by the [normal linear model](statistical-modelling.md#normal-linear-model) [likelihood function](statistical-modelling.md#likelihood-function) and completing the square preserves the family, giving an analytic posterior and evidence integral.

### Natural conjugate prior

↑ **Parent:** [Conjugate prior](#conjugate-prior)

For an [exponential family](exponential-family.md) with density proportional to $\exp\{\theta^TT(x)-A(\theta)\}$, its natural conjugate prior has density proportional to $\exp\{\theta^T\lambda_1-\lambda_2A(\theta)\}$. Observations update $\lambda_1$ by adding sufficient statistics and update $\lambda_2$ by adding sample size.

#### Natural conjugate credibility identity

↑ **Parent:** [Natural conjugate prior](#natural-conjugate-prior)

For a positive-support [exponential family](exponential-family.md) $f(x\mid\theta)=p(x)e^{-\theta x}/q(\theta)$, normalization gives $m(\theta)=-q'(\theta)/q(\theta)$. The [natural conjugate prior](#natural-conjugate-prior) proportional to $q(\theta)^{-k}e^{-k\mu\theta}$ has logarithmic derivative $k(m(\theta)-\mu)$. If its endpoint density values vanish, integration gives prior [expected value](probability-theory.md#expected-value) $\mathbb E[m(\Theta)]=\mu$. Observations update $k$ to $k+n$ and $\mu$ to $(k\mu+\sum_i x_i)/(k+n)$. The [endpoint control for a Laplace-family conjugate posterior](#endpoint-control-for-a-laplace-family-conjugate-posterior) justifies the same mean identity after updating, giving an exact [credibility estimate](actuarial-statistics.md#credibility-estimate) with [credibility factor](actuarial-statistics.md#credibility-factor) $n/(n+k)$.

##### Endpoint control for a Laplace-family conjugate posterior

↑ **Parent:** [Natural conjugate credibility identity](#natural-conjugate-credibility-identity)

In the positive-support [exponential family](exponential-family.md) $q(\theta)=\int p(x)e^{-\theta x}\,dx$, a proper [natural conjugate prior](#natural-conjugate-prior) with zero endpoint density values has mean parameter strictly inside the essential convex support $(a,b)$. Updating that mean by a positive-weight average with supported observations keeps it inside $(a,b)$. At finite parameter endpoints, prior vanishing forces $q\to\infty$, so the increased posterior power $q^{-k-n}$ still vanishes. At positive infinity, positive base-measure mass below a point $d$ smaller than the updated mean bounds $q(\theta)$ below by $Ce^{-d\theta}$, giving [exponential decay](analysis.md#exponential-decay) of the posterior kernel. Mass above the updated mean gives the analogous bound at negative infinity. Thus the updated density is proper and has the boundary condition required to integrate its score.

## Natural parameter of an exponential family

↑ **Parent:** [Exponential family](exponential-family.md)

In the canonical representation

$$
f_\theta(y)=h(y)\exp\{\theta T(y)-A(\theta)\},
$$

$\theta$ is the natural parameter and $T$ is the natural statistic.

### Natural parameter space

↑ **Parent:** [Natural parameter of an exponential family](#natural-parameter-of-an-exponential-family)

The natural parameter space is the set of $\theta$ for which the normalizing integral $\int h(y)e^{\theta^TT(y)}\,dy$ is finite. Interior points permit the usual [exponential-family derivative identities](#exponential-family-derivative-identities) when differentiation and integration can be interchanged.

## Cumulant function of an exponential family

↑ **Parent:** [Exponential family](exponential-family.md)

The cumulant function, or log-partition function, is the normalizing term

$$
A(\theta)=\log\int h(y)e^{\theta T(y)}\,dy,
$$

with a sum in the discrete case.

### Exponential-family derivative identities

↑ **Parent:** [Cumulant function of an exponential family](#cumulant-function-of-an-exponential-family)

Differentiating the normalization identity gives

$$
A'(\theta)=\mathbb E_\theta T,
\qquad
A''(\theta)=\operatorname{var}_\theta T.
$$

### Mean parameter of an exponential family

↑ **Parent:** [Cumulant function of an exponential family](#cumulant-function-of-an-exponential-family)

The mean parameter corresponding to the natural parameter $\theta$ is

$$
\mu(\theta)=\mathbb E_\theta[T(Y)]=A'(\theta).
$$

#### Interior moment matching in a finite exponential family

↑ **Parent:** [Mean parameter of an exponential family](#mean-parameter-of-an-exponential-family)

For a finite support whose [convex hull](mathematical-optimization.md#convex-hull) has full dimension, every interior target mean is realized by a unique natural parameter. Minimize the [coercive function](real-analysis.md#coercive-function) $\log\sum_ne^{\theta\cdot n}-\theta\cdot\mu$; its [gradient](calculus.md#gradient) is the mean discrepancy and its [Hessian matrix](calculus.md#hessian-matrix) is the positive-definite [covariance matrix](variance.md#covariance-matrix) of the support.

## Inverse Gaussian distribution

↑ **Parent:** [Exponential family](exponential-family.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inverse_Gaussian_distribution)

For an [expected value](probability-theory.md#expected-value) parameter $\mu>0$ and a [shape parameter](statistical-modelling.md#shape-parameter) $\lambda>0$, the inverse Gaussian distribution has [probability density function](continuous-probability-distribution.md#probability-density-function)

$$
f(x;\mu,\lambda)
=\left(\frac{\lambda}{2\pi x^3}\right)^{1/2}
\exp\left(-\frac{\lambda(x-\mu)^2}{2\mu^2x}\right),
\qquad x>0.
$$

Its mean is $\mu$ and its variance is $\mu^3/\lambda$.

### Inverse Gaussian shape estimation and nuisance orthogonality

↑ **Parent:** [Inverse Gaussian distribution](#inverse-gaussian-distribution)

For the [Inverse Gaussian distribution](#inverse-gaussian-distribution) parametrized by shape $\psi$ and mean $\lambda$, the joint [maximum-likelihood estimators](statistical-modelling.md#maximum-likelihood-estimator) are $\widehat\lambda=\bar Y$ and $\widehat\psi=(\overline{Y^{-1}}-1/\bar Y)^{-1}$. With known $\lambda$, the shape estimator is instead $(\overline{Y^{-1}}-2/\lambda+\bar Y/\lambda^2)^{-1}$. [Parameter orthogonality](statistical-modelling.md#orthogonal-statistical-parameters) gives the same [Wald test](statistical-modelling.md#wald-test) formula $n(\widehat\psi-\psi_0)^2/(2\widehat\psi^2)$ in both fits. The two estimators differ by $O_p(n^{-1})$ under regular model sampling, so the test statistics agree to first order under the null; they need not be numerically equal in finite samples.

### Inverse Gaussian sum closure

↑ **Parent:** [Inverse Gaussian distribution](#inverse-gaussian-distribution)

In the parametrization with density proportional to $y^{-3/2}\exp[-(\lambda/y+\phi y)/2]$, the [Inverse Gaussian distribution](#inverse-gaussian-distribution) has [cumulant-generating function](probability-theory.md#cumulant-generating-function) $K(t)=\sqrt{\lambda\phi}-\sqrt{\lambda(\phi-2t)}$. For $n$ independent copies, the average has this same family with parameters $(n\phi,n\lambda)$, while the sum has parameters $(\phi,n^2\lambda)$. These assertions follow by multiplying [moment-generating functions](probability-theory.md#moment-generating-function) and scaling the density. The more usual mean parameter is $\mu=\sqrt{\lambda/\phi}$, so the sum has mean $n\mu$ and shape $n^2\lambda$.

#### Exact saddlepoint density of an inverse Gaussian sum

↑ **Parent:** [Inverse Gaussian sum closure](#inverse-gaussian-sum-closure)

For the [inverse Gaussian sum closure](#inverse-gaussian-sum-closure), take $x=s/n>0$. The saddle solves $\widehat t=(\phi-\lambda/x^2)/2$, and $K''(\widehat t)=x^3/\lambda$. Substitution in the [saddlepoint density approximation](probability-theory.md#saddlepoint-density-approximation) gives

$$
\widehat f_{S_n}(s)=\frac{n\sqrt\lambda}{\sqrt{2\pi}s^{3/2}}\exp\left[n\sqrt{\lambda\phi}-\frac12\left(\frac{n^2\lambda}{s}+\phi s\right)\right].
$$

This is the exact sum density, so its leading saddlepoint expression needs no correction or renormalization.

### Chi-squared transform of an inverse Gaussian variable

↑ **Parent:** [Inverse Gaussian distribution](#inverse-gaussian-distribution)

For $X\sim IG(\mu,\lambda)$, $h(X)=\lambda(X-\mu)^2/(\mu^2X)$ has the chi-squared-one law. Its two inverse branches contribute weights $\mu/(\mu+x_-)$ and $\mu/(\mu+x_+)$ to the transformed density, and reciprocal roots make those weights sum to one.

### Reciprocal-root inverse Gaussian sampler

↑ **Parent:** [Inverse Gaussian distribution](#inverse-gaussian-distribution)

For a chi-squared-one variable $Y$, the positive inverse branches of $h(x)=\lambda(x-\mu)^2/(\mu^2x)$ have product $\mu^2$. Weight a branch value $x$ by $\mu/(\mu+x)$; the two weights sum to one. Multiplying the chi-squared density by this weight and the branch Jacobian gives the inverse Gaussian density on both sides of $\mu$.

#### Stable root evaluation for inverse Gaussian sampling

↑ **Parent:** [Reciprocal-root inverse Gaussian sampler](#reciprocal-root-inverse-gaussian-sampler)

With $t=\mu Y/(2\lambda)$, the lower root is $\mu/(1+t+\sqrt{t(t+2)})$ and the upper root is $\mu^2/x_-$. Rationalizing the lower-root formula avoids subtracting nearly equal large numbers when $Y$ is large.

## Exponential-family deviance

↑ **Parent:** [Exponential family](exponential-family.md)

The deviance from $\theta_1$ to $\theta_2$ is twice the [Kullback-Leibler divergence](probability-and-statistics.md#kullback-leibler-divergence):

$$
D(\theta_1,\theta_2)
=2\mathbb E_{\theta_1}\!\left[
\log\frac{f_{\theta_1}(Y)}{f_{\theta_2}(Y)}
\right].
$$

### Scaled deviance

↑ **Parent:** [Exponential-family deviance](#exponential-family-deviance)

For an [exponential dispersion family](#exponential-dispersion-model) with a common [dispersion parameter](#dispersion-parameter) $\phi$, scaled deviance compares a fitted model with the [saturated statistical model](statistical-modelling.md#saturated-statistical-model) at the same dispersion:

$$
D^*=2\{\ell(\widetilde\theta;\phi)-\ell(\widehat\theta;\phi)\}=\frac D\phi,
\qquad
D=2\sum_i\{y_i(\widetilde\theta_i-\widehat\theta_i)-b(\widetilde\theta_i)+b(\widehat\theta_i)\}.
$$

For a [normal distribution](probability-theory.md#normal-distribution) with variance $\sigma^2$, unscaled [deviance](#exponential-family-deviance) is the [residual sum of squares](linear-regression.md#residual-sum-of-squares) and scaled deviance is that sum divided by $\sigma^2$. For the [binomial distribution](discrete-probability-distribution.md#binomial-distribution), $\phi=1$ and the two coincide. Unknown Gaussian dispersion requires variance estimation; raw deviance differences should not be treated as chi-squared statistics without the scale.

## Negative binomial exponential family

↑ **Parent:** [Exponential family](exponential-family.md)

For fixed positive integer $r$, the failures-before-the-$r$th-success distribution is a one-parameter exponential family with

$$
\theta=\log(1-p)<0,
\quad
T(x)=x,
\quad
A(\theta)=-r\log(1-e^\theta),
$$

and carrier $h(x)=\binom{x+r-1}{x}$.

## Exponential dispersion model

↑ **Parent:** [Exponential family](exponential-family.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exponential_dispersion_model)

With dispersion $\phi$ and known weight $w$, an exponential dispersion density has exponent

$$
\frac w\phi\{y\theta-b(\theta)\}+c(y,\phi/w).
$$

Its mean is $b'(\theta)$ and its variance is $(\phi/w)b''(\theta)$.

### Exponential dispersion family of order one

↑ **Parent:** [Exponential dispersion model](#exponential-dispersion-model)

An order-one [exponential dispersion family](#exponential-dispersion-model) has a scalar [natural parameter](#natural-parameter-of-an-exponential-family) and canonical sufficient statistic $y$; its density or mass function has the displayed form on parameter-independent support. Differentiating its normalization gives $\mathbb E Y=b'(\theta)$ and $\operatorname{Var}(Y)=\phi b''(\theta)$. Known observation weights $w$ replace $\phi$ by $\phi/w$. Its [variance function](#variance-function) is $V(\mu)=b''((b')^{-1}(\mu))$, and its [canonical link function](statistical-modelling.md#canonical-link-function) is $(b')^{-1}$.

### Dispersion parameter

↑ **Parent:** [Exponential dispersion model](#exponential-dispersion-model)

The dispersion parameter scales the variance of an [exponential dispersion family](#exponential-dispersion-model) while leaving its mean function unchanged.

#### Underdispersion

↑ **Parent:** [Dispersion parameter](#dispersion-parameter)

Underdispersion means less variation than prescribed by a reference statistical model, corresponding to a working [dispersion parameter](#dispersion-parameter) below one. It is not, by itself, evidence that the reference mean function is improved.

#### Overdispersion

↑ **Parent:** [Dispersion parameter](#dispersion-parameter)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Overdispersion)

Overdispersion occurs when observed conditional variation exceeds that prescribed by a statistical model. For count data it commonly means variance greater than the mean assumed by a Poisson model.

### Variance function

↑ **Parent:** [Exponential dispersion model](#exponential-dispersion-model)

The variance function writes an exponential dispersion family's variance as $\operatorname{Var}(Y)=\phi V(\mu)/w$.

## ↑ Ancestors (6)

1. [Statistical modelling](statistical-modelling.md)
2. [Statistical model](statistical-model.md)
3. [Probability and statistics](probability-and-statistics.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (40)

- [Complete sufficient statistic](probability-and-statistics.md#complete-sufficient-statistic)
- [Curved exponential family](#curved-exponential-family)
- [Efficient unbiased estimator implies exponential family](statistical-inference.md#efficient-unbiased-estimator-implies-exponential-family)
- [Endpoint control for a Laplace-family conjugate posterior](#endpoint-control-for-a-laplace-family-conjugate-posterior)
- [Fixed-size negative binomial generalized linear model](statistical-modelling.md#fixed-size-negative-binomial-generalized-linear-model)
- [Minimal exponential family](#minimal-exponential-family)
- [Natural conjugate credibility identity](#natural-conjugate-credibility-identity)
- [Natural conjugate prior](#natural-conjugate-prior)
- [Natural exponential family](#natural-exponential-family)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32.md#6/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-32.md#6/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1.md#5i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3.md#5i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-41.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-42.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-42.md#4/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-4.md#27i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3.md#26i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1.md#28j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-37.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3.md#27k/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-39.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-32.md#3/b/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-213.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-2.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2.md#5j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-224.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#5j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-216.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-224.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1.md#13k/a/solution)
- [Saddlepoint conditional likelihood adjustment](statistical-modelling.md#saddlepoint-conditional-likelihood-adjustment)
