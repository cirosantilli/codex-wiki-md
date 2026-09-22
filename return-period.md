# Return period

↑ **Parent:** [Extreme value theory](extreme-value-theory-split.md)

A [return period](return-period.md) expresses how rare a threshold exceedance is in a specified time block. Let $M_j$ be the [sample maximum](sample-maximum.md) in block $j$, fix a threshold $u$, and suppose $p=\mathbb P(M_j>u)>0$ is the same for every block. The conventional [return period](return-period.md) is $T=1/p$ blocks; blocks of duration $\Delta$ give a time of $\Delta/p$. Thus an annual exceedance [probability](probability.md) $p=0.01$ means a 100-year [return period](return-period.md). This names a frequency scale, not a schedule or a guarantee of one exceedance in each century. The annual convention and the misleading “once every 100 years” interpretation are discussed in [USGS: the 100-year flood](https://www.usgs.gov/water-science-school/science/100-year-flood).

To derive a waiting-time interpretation, assume the exceedance indicators $B_j=\mathbf1_{\{M_j>u\}}$ are [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) with the [Bernoulli distribution](bernoulli-distribution.md) of parameter $p$. Define $W=\min\{j\geq1:B_j=1\}$, counting the successful block as well as all preceding blocks. The first $k-1$ [Bernoulli trials](bernoulli-trial.md) must fail and the $k$th must succeed, so [independence](independent-random-variables.md) gives the [geometric distribution](geometric-distribution.md)

$$
\mathbb P(W=k)=(1-p)^{k-1}p,\quad k=1,2,\ldots,\qquad
\mathbb P(W>n)=(1-p)^n,\qquad \mathbb E[W]=\frac1p=T.
$$

The [expected value](expected-value-split.md) can also be read directly from the [geometric series](geometric-series.md): $\mathbb E[W]=\sum_{n=0}^{\infty}\mathbb P(W>n)=\sum_{n=0}^{\infty}(1-p)^n=1/p$. This counts blocks from the starting boundary, not the exact time of an exceedance within its block. Counting only failed blocks instead would give [expected value](expected-value-split.md) $T-1$. The waiting law and its [memorylessness of the geometric distribution](memorylessness-of-the-geometric-distribution.md) are developed in [Kyle Siegrist, Random Services: the geometric distribution](https://www.randomservices.org/random/bernoulli/Geometric.html).

For a horizon of $n$ complete years, at least one exceedance is the complement of no exceedances. Under the same [independence](independent-random-variables.md) and constant-$p$ assumptions,

$$
\mathbb P(\text{at least one exceedance in }n\text{ years})
=1-(1-p)^n=1-\left(1-\frac1T\right)^n.
$$

For the toy choice $p=0.01$, this gives $9.6\%$ in 10 years, $26.0\%$ in 30 years, $39.5\%$ in 50 years, and $63.4\%$ in 100 years. Even after 100 years there is a $36.6\%$ chance of no exceedance. These numbers are exact model calculations rounded to one decimal place, not measured frequencies. The [median](median.md) waiting count is 69 years, since $1-0.99^{68}<1/2\leq1-0.99^{69}$; the [expected value](expected-value-split.md) is 100 years. A [mean](expected-value-split.md) and a [median](median.md) answer different questions.

<a id="image-a-1-percent-annual-exceedance-probability-accumulates-across-independent-years"></a>
![](return-period-exceedance-horizons.png)

**[Figure 2](#image-a-1-percent-annual-exceedance-probability-accumulates-across-independent-years). A 1 percent annual exceedance probability accumulates across independent years**. Exact toy [probabilities](probability.md) for $p=0.01$. The rising curve uses [independent](independent-random-variables.md) annual [Bernoulli trials](bernoulli-trial.md); the flat line uses one shared [Bernoulli random variable](bernoulli-distribution.md) for every year. Both have the same annual [probability](probability.md), but different multi-year [probabilities](probability.md). No observations are plotted.

The exceedance count $N_n=\sum_{j=1}^n B_j$ has the [binomial distribution](binomial-distribution.md) under [independence](independent-random-variables.md), with [expected value](expected-value-split.md) $np$. Thus $N_{100}$ has [expected value](expected-value-split.md) one, although its [probability](probability.md) of being at least one is only $63.4\%$: some realizations contribute several exceedances. For $0<p<1$, the [memorylessness of the geometric distribution](memorylessness-of-the-geometric-distribution.md) gives $\mathbb P(W>m+n\mid W>m)=(1-p)^n$. A long quiet spell does not make the next independent year's exceedance overdue, and an exceedance this year does not force a quiet interval. Two specified consecutive years both exceed with [probability](probability.md) $p^2=0.0001$ in this toy model.

A reproducible tabletop experiment makes the assumptions tangible. Put 100 identical slips numbered 1 to 100 in a bag; after thoroughly mixing, draw one and record whether it is 100. Replace the slip and mix again before every draw. Treat each draw as one toy year, so the exceedance indicator is a [Bernoulli random variable](bernoulli-distribution.md) with $p=0.01$, provided the sampling is uniform and successive draws are [independent](independent-random-variables.md). Repeat complete 30-draw runs and record the fraction containing at least one 100; separately repeat runs stopped at the first 100 and record their waiting counts. The first fraction targets $1-0.99^{30}$; the waiting-count [histogram](histogram.md) targets $0.99^{k-1}(0.01)$. Replacement keeps $p$ fixed, mixing is intended to support [independence](independent-random-variables.md), and repeated runs expose sampling variation. This is a proposed demonstration of the toy model; no experimental results are asserted here.

[Stationarity](stationary-process.md) supports a time-invariant annual [probability distribution](probability-distribution-split.md), but does not imply [independence](independent-random-variables.md). For an extreme counterexample, draw just one [Bernoulli random variable](bernoulli-distribution.md) $B$ of parameter $0.01$ and set $B_j=B$ for every year. This is a [stationary process](stationary-process.md), yet the [probability](probability.md) of any exceedance in every finite horizon is $0.01$; from an arbitrary starting boundary the wait is infinite with [probability](probability.md) $0.99$. The reciprocal marginal frequency $T=100$ therefore need not equal that forward waiting [expected value](expected-value-split.md). With equal marginal [probabilities](probability.md) $p$ and arbitrary dependence, only the general bounds $p\leq\mathbb P(N_n\geq1)\leq\min(1,np)$ follow, the upper bound being the [union bound](boole-s-inequality.md). [Linearity of expectation](linearity-of-expectation.md) still gives $\mathbb E[N_n]=np$ without [independence](independent-random-variables.md). Mere zero [correlation](pearson-correlation-coefficient.md) does not restore the product formula; even [pairwise independence does not imply joint independence](pairwise-independence-does-not-imply-joint-independence.md). If annual [probabilities](probability.md) change to $p_j$, [independence](independent-random-variables.md) instead gives $\mathbb P(N_n\geq1)=1-\prod_{j=1}^n(1-p_j)$, and one fixed [return period](return-period.md) no longer describes all years.

**Table of contents**

- [Return level](return-level.md)
  - [Return level plot](return-level-plot.md)

## ↑ Ancestors (6)

1. [Extreme value theory](extreme-value-theory-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/4/f/solution.md)
- [Return level](return-level.md)
- [Return level plot](return-level-plot.md)
- [Return period](return-period.md)
