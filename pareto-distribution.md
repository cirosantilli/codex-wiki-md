# Pareto distribution

↑ **Parent:** [Continuous probability distribution](continuous-probability-distribution-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pareto_distribution)

The [Pareto distribution](pareto-distribution.md) describes a positive [random variable](random-variable-split.md) whose [tail probability](tail-probability.md) falls as a [power law](power-law.md). In the shape–minimum convention used here, $X\sim\operatorname{Pareto}(\alpha,\beta)$ has [shape parameter](shape-parameter.md) $\alpha>0$ and minimum $\beta>0$, with [probability support](support-of-a-probability-distribution.md) $[\beta,\infty)$. Its [probability density function](probability-density-function.md) is

$$
f(x)=\begin{cases}\alpha\beta^\alpha x^{-\alpha-1},&x\geq\beta,\\0,&x<\beta.\end{cases}
$$

The minimum $\beta$ has the same units as $X$; the [shape parameter](shape-parameter.md) $\alpha$ is dimensionless. At fixed $\alpha$, changing $\beta$ gives a [scale family](scale-family.md), since $X/\beta\sim\operatorname{Pareto}(\alpha,1)$. This convention is also used in [uniform-Pareto conjugacy](uniform-pareto-conjugacy.md).[NIST Dataplot Reference Manual; Description: standard Pareto density and lower bound; source gamma,a correspond to alpha,beta here](nist-dataplot-reference-manual/pareto-probability-density-function.md)

The [survival function](survival-function.md) and [cumulative distribution function](cumulative-distribution-function.md) are

$$
\overline F(x)=\mathbb P(X>x)=\begin{cases}1,&x<\beta,\\(\beta/x)^\alpha,&x\geq\beta,\end{cases}
\qquad F(x)=1-\overline F(x).
$$

For $0<p<1$, solving $F(x)=p$ gives the [quantile function](quantile-function.md)

$$
Q(p)=\beta(1-p)^{-1/\alpha}.
$$

Its right-hand limit at $p=0$ is $\beta$; it tends to infinity as $p\uparrow1$.[Random: Probability, Mathematical Statistics, Stochastic Processes by Kyle Siegrist; The General Pareto Distribution, Distribution Functions: density, CDF and quantiles; source a,b correspond to alpha,beta here](random-probability-mathematical-statistics-stochastic-processes-by-kyle-siegrist/the-pareto-distribution.md) There is no [probability mass](probability-mass.md) at $\beta$: changing a [probability density function](probability-density-function.md)'s value at that single point changes no [probabilities](probability.md).

Choose $\alpha=2$ and $\beta=10$ as an original theoretical example. Then $\mathbb P(X>20)=1/4$, $\mathbb P(X>100)=1/100$, the [median](median.md) is $10\sqrt2\simeq14.142$, and the 0.99 [quantile](quantile-function.md) is $Q(0.99)=100$. These chosen values and all figures below describe mathematical [probability distributions](probability-distribution-split.md), not actual wealth observations.

<a id="image-pareto-survival-curves-smaller-alpha-gives-a-slower-power-law-tail"></a>
![](pareto-survival-loglog.png)

**[Figure 3](#image-pareto-survival-curves-smaller-alpha-gives-a-slower-power-law-tail). Pareto survival curves: smaller alpha gives a slower power-law tail**.

On this [log-log plot](log-log-plot.md), write $r=x/\beta$ to obtain $\log\overline F(\beta r)=-\alpha\log r$. The [slope](slope.md) is $-\alpha$, whereas the [probability density function](probability-density-function.md) has power exponent $\alpha+1$. Multiplying a threshold by ten divides its [tail probability](tail-probability.md) by $10^\alpha$. A larger $\alpha$ therefore concentrates the [Pareto distribution](pareto-distribution.md) nearer $\beta$; a smaller $\alpha$ makes extreme values more plausible. This exact scaling is useful when modelling large positive losses or sizes over several orders of magnitude.

The [Pareto distribution](pareto-distribution.md) is a [heavy-tailed distribution](heavy-tailed-distribution.md): for every $t>0$, the [exponential moment](exponential-moment.md) $\mathbb E[e^{tX}]$ diverges because $e^{tx}x^{-\alpha-1}$ eventually grows without bound. In contrast, the [Laplace distribution](laplace-distribution.md) has exponentially decreasing tails and some finite positive [exponential moments](exponential-moment.md). The [Student's t-distribution](student-s-t-distribution.md) also has power tails, but on both sides of the [real line](real-line.md), with a smooth central region rather than a positive minimum.

**Table of contents**

- [One-big-jump polynomial lower bound](one-big-jump-polynomial-lower-bound.md)
- [Pareto moment threshold](pareto-moment-threshold.md)
- [Pareto tail conditional scaling](pareto-tail-conditional-scaling.md)
- [Pareto top shares and the 80/20 rule](pareto-top-shares-and-the-80-20-rule.md)

## ↑ Ancestors (7)

1. [Continuous probability distribution](continuous-probability-distribution-split.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (30)

- [Call-price decay and moment threshold](call-price-decay-and-moment-threshold.md)
- [Central limit theorem](central-limit-theorem.md)
- [One-big-jump polynomial lower bound](one-big-jump-polynomial-lower-bound.md)
- [Pareto distribution](pareto-distribution.md)
- [Pareto moment threshold](pareto-moment-threshold.md)
- [Pareto tail conditional scaling](pareto-tail-conditional-scaling.md)
- [Pareto top shares and the 80/20 rule](pareto-top-shares-and-the-80-20-rule.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-35/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/1/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/1/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-41/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-32/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-32/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-33/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-34/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-34/1/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-39/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2/11/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/10/a/solution.md)
- [Power law](power-law.md)
- [Power-law distribution](power-law-distribution.md)
- [Power laws, Pareto distributions and Zipf's law by Mark Newman](power-laws-pareto-distributions-and-zipf-s-law-by-mark-newman.md)
- [Regular variation](regular-variation.md)
- [Tail probability](tail-probability.md)
- [Truncated gamma rejection sampling with a Pareto envelope](truncated-gamma-rejection-sampling-with-a-pareto-envelope.md)
- [Uniform-Pareto conjugacy](uniform-pareto-conjugacy.md)
- [Uniform-Pareto model evidence](uniform-pareto-model-evidence.md)
- [Variance-minimizing retention for shape-three Pareto claims](variance-minimizing-retention-for-shape-three-pareto-claims.md)
- [Weak law of large numbers](weak-law-of-large-numbers.md)
