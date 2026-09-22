# Bayes factor

↑ **Parent:** [Bayesian model evidence](bayesian-model-evidence.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bayes_factor)

A [Bayes factor](bayes-factor.md) measures how data change the relative support for two specified [statistical models](statistical-model-split.md). Write $m_j(D)=p(D\mid H_j)$ for their [Bayesian model evidence](bayesian-model-evidence.md) and define the direction explicitly:

$$
\mathrm{BF}_{10}(D)=\frac{m_1(D)}{m_0(D)}.
$$

For positive finite $m_0(D),m_1(D)$, a value above one favors $H_1$ over $H_0$; a value below one favors $H_0$ over $H_1$. Reversing the comparison gives $B_{01}=\mathrm{BF}_{01}=1/\mathrm{BF}_{10}$, the opposite direction used in some formulas below.

For mutually exclusive, exhaustive $H_0,H_1$ with positive [prior probabilities](prior-probability.md), divide their two [Bayes' theorem](bayes-theorem.md) formulas. Their common data normalizer cancels, leaving

$$
\underbrace{\frac{\mathbb P(H_1\mid D)}{\mathbb P(H_0\mid D)}}_{\text{posterior odds}}
=\underbrace{\frac{m_1(D)}{m_0(D)}}_{\mathrm{BF}_{10}}
\underbrace{\frac{\mathbb P(H_1)}{\mathbb P(H_0)}}_{\text{prior odds}}.
$$

The [Bayes factor](bayes-factor.md) therefore multiplies [prior odds](prior-odds.md) into [posterior odds](posterior-odds.md). It is evidence conditional on the specified [statistical models](statistical-model-split.md) and their within-model [prior distributions](prior-probability.md); it is not $\mathbb P(H_1\mid D)$. Model [prior probabilities](prior-probability.md) supply a separate input.[Kass and Raftery, Bayes Factors (1995), section 3.1, p. 776: posterior odds, prior odds, and direction of the Bayes factor](bayes-factors-by-robert-e-kass-and-adrian-e-raftery.md)

For an original stipulated example, consider ten [independent and identically distributed](independent-and-identically-distributed-random-variables.md) [Bernoulli trials](bernoulli-trial.md), with heads as success. Compare $H_0:p=0.4$ with $H_1:p=0.7$, both fixed before seeing the data. Take $D$ to be one particular ordered sequence containing eight heads and two tails. The [likelihood function](likelihood-function.md) under either point model is $p^8(1-p)^2$, so

$$
\mathrm{BF}_{10}
=\frac{0.7^8\,0.3^2}{0.4^8\,0.6^2}
=\left(\frac{0.7}{0.4}\right)^8\left(\frac{0.3}{0.6}\right)^2
=\frac{5764801}{262144}\approx21.9909706.
$$

If $\mathbb P(H_1)=0.1$, the [prior odds](prior-odds.md) for $H_1$ against $H_0$ are $1/9$. Hence the [posterior odds](posterior-odds.md) are $21.9909706/9\approx2.4434412$, and

$$
\mathbb P(H_1\mid D)
=\frac{\mathrm{BF}_{10}}{9+\mathrm{BF}_{10}}
=\frac{5764801}{8124097}\approx0.7095928.
$$

Equal model [prior probabilities](prior-probability.md) would instead give $\mathrm{BF}_{10}/(1+\mathrm{BF}_{10})\approx0.956505$. The same [Bayes factor](bayes-factor.md) can thus accompany different [posterior probabilities](posterior-probability.md). These statements condition on the two-model comparison; they do not establish that either [statistical model](statistical-model-split.md) describes a real coin.

<a id="image-evidence-across-heads-counts-and-its-multiplication-of-prior-odds"></a>
![](bayes-factor-heads-and-odds.png)

**[Figure 3](#image-evidence-across-heads-counts-and-its-multiplication-of-prior-odds). Evidence across heads counts and its multiplication of prior odds**. Original calculated [Bernoulli trials](bernoulli-trial.md) example, with ten trials and fixed point models $H_0:p=0.4$, $H_1:p=0.7$. Left: the [Bayes factor](bayes-factor.md) for each possible heads count; the highlighted eight-head result favors $H_1$. Right: at that fixed result, the [posterior odds](posterior-odds.md) equal $21.9909706$ times the [prior odds](prior-odds.md). The marked prior $\mathbb P(H_1)=0.1$ becomes [posterior probability](posterior-probability.md) $0.7095928$. No empirical observations are plotted.

Using the heads count $K=8$ instead of the ordered sequence changes the [sample space](sample-space.md). The [binomial distribution](binomial-distribution.md) assigns it mass $\binom{10}{8}p^8(1-p)^2$. The same [binomial coefficient](binomial-coefficient-split.md) multiplies both models' [Bayesian model evidence](bayesian-model-evidence.md) and cancels in their [Bayes factor](bayes-factor.md). Mixing an ordered-sequence numerator with a count denominator would introduce an erroneous factor of $45$.

Fix the candidate [statistical models](statistical-model-split.md), their parameter [prior distributions](prior-probability.md), and model [prior probabilities](prior-probability.md) before using the current data for this update. The [Bayes factor](bayes-factor.md) is useful because it separates evidence from model [prior odds](prior-odds.md), but it still depends on the parameter [prior distributions](prior-probability.md). An [improper prior](improper-prior.md) has an arbitrary multiplicative normalization: multiplying its kernel by $c$ multiplies its formal [marginal likelihood](bayesian-model-evidence.md) by $c$, even if the within-model [posterior distribution](bayesian-posterior.md) is normalizable. Without a separately justified convention, the ordinary [Bayes factor](bayes-factor.md) is then undefined up to arbitrary constants.[Kass and Raftery, Bayes Factors (1995), sections 5.2–5.3, pp. 782–783: prior sensitivity and undefined multiplicative constants](bayes-factors-by-robert-e-kass-and-adrian-e-raftery.md)

**Table of contents**

- [Uniform-alternative binomial Bayes factor](uniform-alternative-binomial-bayes-factor.md)
- [Gaussian practical-null mixture](gaussian-practical-null-mixture.md)
- [Savage-Dickey density ratio](savage-dickey-density-ratio.md)

## ↑ Ancestors (7)

1. [Bayesian model evidence](bayesian-model-evidence.md)
2. [Bayesian statistics](bayesian-statistics-split.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (35)

- [Bayes factor](bayes-factor.md)
- [Bayesian model evidence](bayesian-model-evidence.md)
- [Deviance information criterion](deviance-information-criterion.md)
- [Gaussian practical-null mixture](gaussian-practical-null-mixture.md)
- [Odds under at-least-one-positive selection](odds-under-at-least-one-positive-selection.md)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2015/paper-1/1/solution.md)
- [Solution](past-exam-of-the-frontiers-of-observational-astrophysics-course-of-the-university-of-cambridge/2016/paper-1/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4/27i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-44/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-44/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-44/1/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-44/1/h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-44/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-36/3/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-36/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/1/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/1/h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/2/h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/4/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-29/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-34/4/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/3/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/3/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-219/4/b/solution.md)
- [Poisson mean equality model comparison](poisson-mean-equality-model-comparison.md)
- [Posterior odds](posterior-odds.md)
- [Prequential log score identity](prequential-log-score-identity.md)
- [Prior odds](prior-odds.md)
- [Robert E. Kass](robert-e-kass.md)
- [Savage-Dickey density ratio](savage-dickey-density-ratio.md)
- [Uniform-alternative binomial Bayes factor](uniform-alternative-binomial-bayes-factor.md)
