# Uniform-alternative binomial Bayes factor

↑ **Parent:** [Bayes factor](bayes-factor.md)

For a [binomial distribution](binomial-distribution.md) count, compare a point null $\theta=1/2$ with the uniform alternative [prior distribution](prior-probability.md) on $(0,1)$. The alternative [Bayesian model evidence](bayesian-model-evidence.md) is

$$
\binom ny\int_0^1\theta^y(1-\theta)^{n-y}\,d\theta=\frac1{n+1},
$$

so the exact [Bayes factor](bayes-factor.md) favouring the point null is $(n+1)\binom ny2^{-n}$. With standardized deviation $z=2(y-n/2)/\sqrt n$, the local [normal distribution](normal-distribution.md) approximation is $B_{01}\approx\sqrt{2n/\pi}e^{-z^2/2}$. At fixed $z$ the frequentist [p-value](p-value.md) remains approximately constant, while the factor grows like $\sqrt n$. This demonstrates the prior-width mechanism behind the [Jeffreys-Lindley paradox for a Gaussian point null](jeffreys-lindley-paradox-for-a-gaussian-point-null.md) in a discrete sampling model.

For a separate original example, change the point null to $H_0:p=1/2$ and take $H_U$ to have a [uniform prior](uniform-prior.md) $p\sim\operatorname{Beta}(1,1)$, fixed before the ten [Bernoulli trials](bernoulli-trial.md). Here $p$ is drawn once under $H_U$ and shared by all ten trials: they are [independent](independent-random-variables.md) conditional on $p$. For one particular ordered sequence with eight heads and two tails, the [Euler beta function](beta-function.md) gives

$$
m_0(D)=2^{-10},\qquad
m_U(D)=\int_0^1p^8(1-p)^2\,dp
=B(9,3)=\frac{8!\,2!}{11!}=\frac1{495}.
$$

Thus the [Bayes factor](bayes-factor.md) for the uniform alternative against the point null is

$$
\mathrm{BF}_{U0}=\frac{1024}{495}\approx2.0686869,
\qquad B_{0U}=\frac{495}{1024}\approx0.4833984.
$$

The [binomial distribution](binomial-distribution.md) count formulation gives $m_0(K=8)=45/1024$ and $m_U(K=8)=45/495=1/11$. Their ratio is again $1024/495$; these count masses must not be combined with the ordered-sequence masses above. The general $B_{01}$ formula at the start of this article puts the point null in the numerator, so it equals $B_{0U}$ here.

In contrast, [maximum likelihood estimation](maximum-likelihood-estimation-split.md) gives $\widehat p=0.8$: differentiating the [log-likelihood](log-likelihood.md) yields $8/p-2/(1-p)=0$, and the endpoints have zero [likelihood](likelihood-function.md). Its peak-to-null [likelihood ratio](likelihood-ratio.md) is

$$
\frac{L(0.8)}{L(0.5)}
=\frac{0.8^8\,0.2^2}{2^{-10}}\approx6.8719477.
$$

This peak is chosen after seeing the data, so it is not the [Bayes factor](bayes-factor.md) of the prespecified $H_U$. The [Bayesian model evidence](bayesian-model-evidence.md) for $H_U$ averages $L(p)$ over its entire [uniform prior](uniform-prior.md); it is smaller than the peak. It is also smaller than $L(0.7)=0.7^8\,0.3^2\approx0.00518832$. Against the same $p=0.5$ null, a point alternative fixed at $p=0.7$ would give a [Bayes factor](bayes-factor.md) about $5.31284$, greater than $2.06869$. An integrated alternative need not outperform a point alternative.

<a id="image-a-uniform-prior-average-of-the-likelihood-differs-from-its-maximum"></a>
![](bayes-factor-likelihood-averaging.png)

**[Figure 4](#image-a-uniform-prior-average-of-the-likelihood-differs-from-its-maximum). A uniform-prior average of the likelihood differs from its maximum**. Original calculation for a stipulated ordered sequence with eight heads and two tails. Left: the [likelihood function](likelihood-function.md) $L(p)=p^8(1-p)^2$ and its [uniform prior](uniform-prior.md) average $m_U=1/495$, with the point null at $p=0.5$ and peak at $p=0.8$. Right: the average, fixed $p=0.7$ value, and peak divided by the same null value $2^{-10}$. Only the first two comparisons use prespecified alternatives; the peak uses a [maximum-likelihood estimate](maximum-likelihood-estimator.md). These are calculated model quantities, not measured frequencies.

For a general proper [beta distribution](beta-distribution.md) [prior distribution](prior-probability.md) $\operatorname{Beta}(a,b)$ with $a,b>0$, the same ordered-sequence [marginal likelihood](bayesian-model-evidence.md) is $B(8+a,2+b)/B(a,b)$. This follows by substituting the normalized [prior density](prior-density.md) into the [integral](integral-split.md), and shows exactly where the parameter [prior distribution](prior-probability.md) changes the [Bayes factor](bayes-factor.md). Holding the parameter [prior distributions](prior-probability.md) fixed while changing model [prior odds](prior-odds.md) leaves that [Bayes factor](bayes-factor.md) unchanged.

## ↑ Ancestors (8)

1. [Bayes factor](bayes-factor.md)
2. [Bayesian model evidence](bayesian-model-evidence.md)
3. [Bayesian statistics](bayesian-statistics-split.md)
4. [Statistical inference](statistical-inference-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Bayesian model evidence](bayesian-model-evidence.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/1/d/solution.md)
