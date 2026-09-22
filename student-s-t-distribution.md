<h1 id="student-s-t-distribution">Student's t-distribution</h1>

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Student's_t-distribution)

The [Student's t-distribution](student-s-t-distribution.md) describes a [standard normal random variable](standard-normal-random-variable.md) divided by an [independent](independent-random-variables.md) estimate of its scale. For any real $\nu>0$, let $Z\sim N(0,1)$ have the [standard normal distribution](standard-normal-distribution.md) and let $V\sim\chi^2_\nu$ have the [chi-squared distribution](chi-squared-distribution.md), with $Z$ and $V$ [independent](independent-random-variables.md). Then

$$
T=\frac{Z}{\sqrt{V/\nu}}\sim t_\nu.
$$

The parameter $\nu$ is called the number of [statistical degrees of freedom](statistical-degrees-of-freedom.md). It need not be an integer: the [chi-squared distribution](chi-squared-distribution.md) is a [gamma distribution](gamma-distribution.md) with shape $\nu/2$ and rate $1/2$. The [independence](independent-random-variables.md) assumption is essential; specifying only the two [marginal distributions](marginal-distribution.md) does not determine the [probability distribution](probability-distribution-split.md) of their ratio.

Its [probability density function](probability-density-function.md) on the whole [real line](real-line.md) is

$$
f_\nu(t)=\frac{\Gamma((\nu+1)/2)}{\sqrt{\nu\pi}\,\Gamma(\nu/2)}\left(1+\frac{t^2}{\nu}\right)^{-(\nu+1)/2},\qquad -\infty<t<\infty,
$$

where $\Gamma$ is the [gamma function](gamma-function.md). Every member is a [symmetric distribution](symmetric-distribution.md) about zero. At $\nu=1$ it is the [Standard Cauchy distribution](standard-cauchy-distribution.md); as $\nu\to\infty$ it approaches the [standard normal distribution](standard-normal-distribution.md). The essential shape change is the tail: at any fixed finite $\nu$, $f_\nu(t)$ decays like a constant times $|t|^{-(\nu+1)}$, much more slowly than the [standard normal density](standard-normal-density.md)'s exponential decay. Thus it is a [heavy-tailed distribution](heavy-tailed-distribution.md). [NIST and SEMATECH e-Handbook of Statistical Methods; NIST/SEMATECH e-Handbook, Section 1.3.6.6.4: density, Cauchy special case and normal limit; the ratio derivation here also permits noninteger degrees of freedom](nist-and-sematech-e-handbook-of-statistical-methods/1-3-6-6-4-t-distribution.md)

<a id="image-student-t-densities-with-1-3-and-10-degrees-of-freedom-compared-with-the-standard-normal-density"></a>
![](student-t-density-families.png)

**[Figure 7](#image-student-t-densities-with-1-3-and-10-degrees-of-freedom-compared-with-the-standard-normal-density). Student t densities with 1, 3 and 10 degrees of freedom compared with the standard normal density**.

The left panel shows the centers; the right panel uses a [logarithmic scale](logarithmic-scale.md) to reveal the tails that a linear plot hides. All four curves have location zero and scale one. They do not have the same [variance](variance-split.md): the $t_1$ curve has no finite [mean](expected-value-split.md) or [variance](variance-split.md), whereas $t_3$ has [variance](variance-split.md) 3 and $t_{10}$ has [variance](variance-split.md) $10/8$.

More generally, the absolute [moment](moment.md) $\mathbb E|T|^p$ for $p>0$ is finite exactly when $p<\nu$, as follows by comparing the tail integrand with $t^{p-\nu-1}$. Consequently

$$
\mathbb E[T]=0\quad(\nu>1),\qquad \operatorname{Var}(T)=\frac{\nu}{\nu-2}\quad(\nu>2).
$$

For $0<\nu\leq1$ there is no finite [mean](expected-value-split.md); symmetry alone cannot supply one. For $1<\nu\leq2$ the [mean](expected-value-split.md) exists but the [variance](variance-split.md) is infinite. For $0<\nu\leq1$ even the centered definition of [variance](variance-split.md) is unavailable because the [mean](expected-value-split.md) does not exist.

A shifted and scaled version $Y=m+bT$, $b>0$, has [probability density function](probability-density-function.md) $b^{-1}f_\nu((y-m)/b)$. The scale $b$ is not its [standard deviation](standard-deviation.md): for $\nu>2$,

$$
\operatorname{SD}(Y)=b\sqrt{\frac{\nu}{\nu-2}}.
$$

For example, $\nu=3$ and scale $b=2$ give [standard deviation](standard-deviation.md) $2\sqrt3$, rather than 2. The distinction matters when using a [Student's t-distribution](student-s-t-distribution.md) to model data with occasional extreme values, as well as when interpreting a [Student t confidence interval](student-t-confidence-interval.md).

**Table of contents**

- [Normal scale mixture representation of Student t](normal-scale-mixture-representation-of-student-t.md)
- [Noncentral t-distribution](noncentral-t-distribution.md)
- [Studentized normal sample mean](studentized-normal-sample-mean.md)
  - [Small normal sample mean confidence interval](small-normal-sample-mean-confidence-interval.md)
- [History of Student's t-distribution](history-of-student-s-t-distribution.md)

## ↑ Ancestors (7)

1. [Continuous probability distribution](continuous-probability-distribution-split.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (30)

- [Distribution of an internally studentized Gaussian residual](distribution-of-an-internally-studentized-gaussian-residual.md)
- [Noncentral t-distribution](noncentral-t-distribution.md)
- [Normal prediction interval with maximum-likelihood variance](normal-prediction-interval-with-maximum-likelihood-variance.md)
- [Pareto distribution](pareto-distribution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-4/12d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-4/3d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-2/12h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-42/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-1/10h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-3/8d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-3/5j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1/13j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35/4/h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-4/10j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/19h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-206/2/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/5j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-3/20h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-3/20h/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/5j/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2015/paper-1/section-d/d12/solution.md)
- [Residual estimate of slope uncertainty through the origin](residual-estimate-of-slope-uncertainty-through-the-origin.md)
- [Small normal sample mean confidence interval](small-normal-sample-mean-confidence-interval.md)
- [Student's t-distribution](student-s-t-distribution.md)
- [Student's t-test](student-s-t-test.md)
- [Student t random-effect model](student-t-random-effect-model.md)
- [Student t test for regression through the origin](student-t-test-for-regression-through-the-origin.md)
- [Studentized normal sample mean](studentized-normal-sample-mean.md)
