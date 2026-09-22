<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In the [Bühlmann model](../../../../../buhlmann-model.md), one policy has a random risk parameter $\Theta$. Conditional on $\Theta$, its annual observations $X_i$ are [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md), with mean $m(\Theta)$ and variance $v(\Theta)$. Put $m_0=\mathbb E[m(\Theta)]$, let $v=\mathbb E[v(\Theta)]$ be the [expected process variance](../../../../../expected-process-variance.md), and let $a=\operatorname{Var}(m(\Theta))$ be the [variance of hypothetical means](../../../../../variance-of-hypothetical-means.md). Assume the required second moments are finite.

The [Bühlmann credibility premium](../../../../../buhlmann-credibility-premium.md) is the best affine estimate of $m(\Theta)$ under [mean squared error](../../../../../mean-squared-error.md). After choosing the intercept to make the estimate unbiased, write it as $m_0+\sum_{i=1}^n b_i(X_i-m_0)$. If $B=\sum_i b_i$, the [law of total variance](../../../../../law-of-total-variance.md) and conditional independence give its error

$$
\mathbb E\left[\left(m(\Theta)-m_0-\sum_i b_i(X_i-m_0)\right)^2\right]
=a(1-B)^2+v\sum_i b_i^2.
$$

For fixed $B$, the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) minimizes the last sum at $b_i=B/n$. Differentiating $a(1-B)^2+vB^2/n$ gives $B=na/(na+v)$. Thus the [credibility factor](../../../../../credibility-factor.md) and [credibility premium](../../../../../credibility-estimate.md) are

$$
\boxed{Z=\frac{na}{na+v}=\frac{n}{n+v/a},\qquad \widehat m=Z\overline X+(1-Z)m_0.}
$$

The ratio form assumes $a>0$; when $a=0$ and $v>0$, the conditional mean is constant and $Z=0$. Predicting $X_{n+1}$ rather than its conditional mean adds the constant $v$ to the error and leaves the optimal affine estimate unchanged.

Here the latent intensity has a [Pareto distribution](../../../../../pareto-distribution.md) with shape three and lower bound one. For $r<3$, its moments are $\mathbb E[\Theta^r]=3\int_1^\infty\theta^{r-4}\,d\theta=3/(3-r)$. Consequently

$$
m_0=\mathbb E\Theta=\frac32,\qquad v=\mathbb E\Theta=\frac32,\qquad a=\operatorname{Var}\Theta=3-\frac94=\frac34.
$$

The equality for $v$ uses the [Poisson distribution](../../../../../poisson-distribution.md) conditional variance $v(\Theta)=\Theta$. There are two years of experience, so $Z=1/2$ and the observed [sample mean](../../../../../sample-mean.md) is $k/2$. The [Poisson credibility with a shape-three Pareto intensity](../../../../../poisson-credibility-with-a-shape-three-pareto-intensity.md) is therefore

$$
\boxed{\widehat m_{\mathrm{cred}}=\frac12\frac{k}{2}+\frac12\frac32=\frac{k+3}{4}.}
$$

In particular it equals $2$ when $k=5$.

For the exact [Bayesian credibility](../../../../../bayesian-credibility.md) estimate, the total count conditional on $\Theta=\theta$ has [Poisson distribution](../../../../../poisson-distribution.md) of mean $2\theta$. Multiplication of its [likelihood](../../../../../likelihood-function.md) by the [prior distribution](../../../../../prior-probability.md) density gives a [Bayesian posterior](../../../../../bayesian-posterior.md) density proportional to $\theta^{k-4}e^{-2\theta}$ on $\theta>1$. At $k=5$, its normalizing integral and first-moment integral are

$$
\int_1^\infty\theta e^{-2\theta}\,d\theta=\frac34e^{-2},\qquad
\int_1^\infty\theta^2e^{-2\theta}\,d\theta=\frac54e^{-2}.
$$

Hence the next-year predictive [expected value](../../../../../expected-value.md) is

$$
\boxed{\mathbb E[N_3\mid N_1+N_2=5]=\mathbb E[\Theta\mid N_1+N_2=5]=\frac53\ne2.}
$$

The [Bühlmann credibility premium](../../../../../buhlmann-credibility-premium.md) optimizes over affine estimates, whereas the [Bayesian posterior](../../../../../bayesian-posterior.md) mean optimizes over all square-integrable estimates. This explains why the two [credibility estimates](../../../../../credibility-estimate.md) need not agree for this nonconjugate prior.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 35](../../paper-35-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
