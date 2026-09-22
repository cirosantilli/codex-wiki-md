# Beta distribution

↑ **Parent:** [Probability distribution](probability-distribution-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Beta_distribution)

The [beta distribution](beta-distribution.md) is an [absolutely continuous probability distribution](absolutely-continuous-probability-distribution.md) for a [random variable](random-variable-split.md) $X$ between zero and one. It can describe uncertainty about a [probability](probability.md), such as an unknown coin's chance of heads. For any real $\alpha,\beta>0$, its [probability density function](probability-density-function.md) is

$$
f_X(x)=\frac{x^{\alpha-1}(1-x)^{\beta-1}}{B(\alpha,\beta)},\qquad 0<x<1,
$$

and zero outside $[0,1]$. The normalizer is the [Euler beta function](beta-function.md), related to the [gamma function](gamma-function.md) by the [beta-gamma identity](beta-gamma-identity.md):

$$
B(\alpha,\beta)=\int_0^1x^{\alpha-1}(1-x)^{\beta-1}\,dx=\frac{\Gamma(\alpha)\Gamma(\beta)}{\Gamma(\alpha+\beta)}.
$$

Thus the [probability density function](probability-density-function.md) integrates to one. [NIST DLMF 5.12.1: the beta integral and gamma-function normalizer](https://dlmf.nist.gov/5.12#E1).

The endpoint behavior explains why the restrictions are exactly $\alpha,\beta>0$: near zero the [probability density function](probability-density-function.md) behaves like a constant times $x^{\alpha-1}$, and near one like a constant times $(1-x)^{\beta-1}$. These [improper integrals](improper-integral.md) converge for positive parameters, even when the [probability density function](probability-density-function.md) diverges at zero for $\alpha<1$ or at one for $\beta<1$. There is no [probability mass](probability-mass.md) at either endpoint: $\mathbb P(X=0)=\mathbb P(X=1)=0$. A [probability density function](probability-density-function.md)'s height is not a [probability](probability.md); an interval's [probability](probability.md) is the area under it.

Some useful examples of the [beta distribution](beta-distribution.md) are:

- $\operatorname{Beta}(1,1)$ is the [uniform distribution](continuous-uniform-distribution.md) on $(0,1)$, with [probability density function](probability-density-function.md) $f_X(x)=1$.
- $\operatorname{Beta}(2,2)$ has [probability density function](probability-density-function.md) $f_X(x)=6x(1-x)$: values near one half are favored, and it is a [symmetric probability distribution](symmetric-probability-distribution.md) about one half.
- $\operatorname{Beta}(2,5)$ has [probability density function](probability-density-function.md) $f_X(x)=30x(1-x)^4$. Its [mean](expected-value-split.md) is $2/7$ and its [variance](variance-split.md) is $10/(49\cdot8)=5/196\approx0.0255102$; most of its area lies toward the lower end.
- $\operatorname{Beta}(1/2,1/2)$ is the [arcsine distribution](arcsine-distribution.md), with [probability density function](probability-density-function.md) $f_X(x)=1/(\pi\sqrt{x(1-x)})$. It favors values near both endpoints despite having [mean](expected-value-split.md) $1/2$; its [variance](variance-split.md) is $1/8$.

<a id="image-beta-density-shapes-uniform-central-asymmetric-and-boundary-singular"></a>
![](beta-density-shapes.png)

**[Figure 4](#image-beta-density-shapes-uniform-central-asymmetric-and-boundary-singular). Beta density shapes: uniform, central, asymmetric, and boundary singular**.

The [arcsine distribution](arcsine-distribution.md) curve is plotted only for $0.001\leq x\leq0.999$; its finite plotted ends do not represent finite endpoint values of the [probability density function](probability-density-function.md). Using the [inverse sine](inverse-sine.md), the shaded central interval has exact [probability](probability.md) $\mathbb P(0.1<X<0.9)=1-4\arcsin(\sqrt{0.1})/\pi\approx0.5903$, calculated analytically rather than by treating the cropped curve as normalized.

To separate location from spread, write $\kappa=\alpha+\beta$ and $m=\alpha/\kappa$. The [mean](expected-value-split.md) and [variance](variance-split.md) of the [beta distribution](beta-distribution.md) are

$$
\mathbb E[X]=m=\frac{\alpha}{\kappa},\qquad
\operatorname{Var}(X)=\frac{\alpha\beta}{\kappa^2(\kappa+1)}=\frac{m(1-m)}{\kappa+1}.
$$

The [mean](expected-value-split.md) specifies the balance between the parameters; their sum $\kappa$ controls concentration about that [mean](expected-value-split.md). Multiplying both parameters by the same positive number preserves the [mean](expected-value-split.md) and changes the [variance](variance-split.md). Larger $\kappa$ puts more area near $m$ and makes the [probability density function](probability-density-function.md) taller there; the total area stays one. Small $\kappa$ allows much greater spread, sometimes favoring the endpoints rather than the [mean](expected-value-split.md) itself.

For example, keeping [mean](expected-value-split.md) $m=0.3$ and taking $\kappa=5,20,80$ gives the [beta distributions](beta-distribution.md) $\operatorname{Beta}(1.5,3.5)$, $\operatorname{Beta}(6,14)$, and $\operatorname{Beta}(24,56)$. Their [variances](variance-split.md) are $0.035$, $0.01$, and $0.21/81\approx0.00259259$, respectively. Parameters need not be integers.

<a id="image-the-same-beta-mean-with-three-concentrations-and-decreasing-variance"></a>
![](beta-mean-and-concentration.png)

**[Figure 5](#image-the-same-beta-mean-with-three-concentrations-and-decreasing-variance). The same beta mean with three concentrations and decreasing variance**.

The formulas follow from two short [moment](moment.md) calculations. Multiplying the [probability density function](probability-density-function.md) by $x$ or $x^2$ increases the first parameter of the [Euler beta function](beta-function.md):

$$
\mathbb E[X]=\frac{B(\alpha+1,\beta)}{B(\alpha,\beta)}=\frac{\alpha}{\kappa},\qquad
\mathbb E[X^2]=\frac{B(\alpha+2,\beta)}{B(\alpha,\beta)}=\frac{\alpha(\alpha+1)}{\kappa(\kappa+1)}.
$$

Apply the [Gamma function recurrence](gamma-function-recurrence.md) to the [beta-gamma identity](beta-gamma-identity.md), then subtract $(\mathbb E[X])^2$ from $\mathbb E[X^2]$ to obtain the [variance](variance-split.md).

The [beta distribution](beta-distribution.md) is especially convenient as a [prior distribution](prior-probability.md) for the unknown success [probability](probability.md) $P$ of [Bernoulli trials](bernoulli-trial.md). The [Beta-binomial conjugacy](beta-binomial-conjugacy.md) says that $h$ successes and $t$ failures update a [prior distribution](prior-probability.md) $\operatorname{Beta}(\alpha,\beta)$ to a [posterior distribution](bayesian-posterior.md) $\operatorname{Beta}(\alpha+h,\beta+t)$. For example, suppose a coin has [prior distribution](prior-probability.md) $\operatorname{Beta}(2,2)$ and we observe eight heads and two tails. Its [posterior distribution](bayesian-posterior.md) is then $\operatorname{Beta}(10,4)$, with [posterior](bayesian-posterior.md) [mean](expected-value-split.md) $5/7$. [MIT 18.05, Reading 15: beta priors and conjugate updating](https://ocw.mit.edu/courses/18-05-introduction-to-probability-and-statistics-spring-2022/mit18_05_s22_class15-prep.pdf).

**Table of contents**

- [Moment matching for a beta prior](moment-matching-for-a-beta-prior.md)
- [Beta sampling by uniform order statistics](beta-sampling-by-uniform-order-statistics.md)
- [Beta sampling by gamma ratios](beta-sampling-by-gamma-ratios.md)

## ↑ Ancestors (6)

1. [Probability distribution](probability-distribution-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (69)

- [Arcsine distribution](arcsine-distribution.md)
- [Bayesian statistics](bayesian-statistics-split.md)
- [Beta-binomial distribution](beta-binomial-distribution.md)
- [Beta-binomial exchangeable coupling](beta-binomial-exchangeable-coupling.md)
- [Beta distribution](beta-distribution.md)
- [Beta-gamma independence](beta-gamma-independence.md)
- [Beta-geometric conjugacy](beta-geometric-conjugacy.md)
- [Beta-prime distribution](beta-prime-distribution.md)
- [Beta sampling by gamma ratios](beta-sampling-by-gamma-ratios.md)
- [Beta sampling by uniform order statistics](beta-sampling-by-uniform-order-statistics.md)
- [Binomial likelihood-power annealing](binomial-likelihood-power-annealing.md)
- [Distribution of an internally studentized Gaussian residual](distribution-of-an-internally-studentized-gaussian-residual.md)
- [Equal-tailed credible interval](equal-tailed-credible-interval.md)
- [Haldane prior](haldane-prior.md)
- [Incomplete beta function](incomplete-beta-function.md)
- [Mean measure of Poisson-Dirichlet components](mean-measure-of-poisson-dirichlet-components.md)
- [Moment matching for a beta prior](moment-matching-for-a-beta-prior.md)
- [One-sided credible interval](one-sided-credible-interval.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-1/6/b/solution.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-1/6/c/solution.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-1/6/e/solution.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-1/6/f/solution.md)
- [Solution](past-exam-of-the-mathematical-and-computational-biology-course-of-the-university-of-cambridge/2025/paper-1/6/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-40/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-42/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-47/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1/18c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-43/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-44/2/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/3/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-36/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-36/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-36/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-36/4/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-36/4/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36/1/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-34/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/2/e/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/2/e/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/2/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/2/h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/2/j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-39/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/25j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2/9f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/12j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-216/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-4/19h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-210/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-2/8h/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-207/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-207/1/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-4/17h/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-1/18h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2023/paper-1/16/c/solution.md)
- [Prior elicitation](prior-elicitation.md)
- [Prior probability](prior-probability.md)
- [Probability content of a nearest neighbour ball](probability-content-of-a-nearest-neighbour-ball.md)
- [Uniform-alternative binomial Bayes factor](uniform-alternative-binomial-bayes-factor.md)
- [Uniform-envelope rejection sampling for a beta distribution](uniform-envelope-rejection-sampling-for-a-beta-distribution.md)
- [Uniform order statistic](uniform-order-statistic.md)
- [Uniform prior](uniform-prior.md)
- [Uniform-value multi-prize all-pay effort formula](uniform-value-multi-prize-all-pay-effort-formula.md)
