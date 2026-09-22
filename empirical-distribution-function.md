# Empirical distribution function

↑ **Parent:** [Cumulative distribution function](cumulative-distribution-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Empirical_distribution_function)

The [empirical distribution function](empirical-distribution-function.md) counts the fraction of observations at or below a threshold. For a [statistical sample](statistical-sample.md) of $n\geq1$ real observations $X_1,\ldots,X_n$, define

$$
F_n(x)=\frac{\#\{i:X_i\leq x\}}n=\frac1n\sum_{i=1}^n\mathbf1_{\{X_i\leq x\}}.
$$

Each [indicator function](indicator-function.md) contributes one exactly when its observation is counted. Equivalently, $F_n(x)=P_n((-\infty,x])$, where the [empirical measure](empirical-measure.md) $P_n=n^{-1}\sum_i\delta_{X_i}$ assigns [probability mass](probability-mass.md) $1/n$ to each observation, including repeated observations.[§2.1, printed p. 13, Definition 2.1 and equation (2.2); §2.4, printed p. 21, equation (2.37)](all-of-nonparametric-statistics-by-larry-wasserman.md)

Choose the illustrative [statistical sample](statistical-sample.md) $[1,1,2,4,6]$. Its [empirical distribution function](empirical-distribution-function.md) is

$$
F_5(x)=\begin{cases}
0&x<1,\\
2/5&1\leq x<2,\\
3/5&2\leq x<4,\\
4/5&4\leq x<6,\\
1&6\leq x.
\end{cases}
$$

For example, $F_5(1)=2/5$ counts both observations equal to $1$, $F_5(3)=3/5$, and $F_5(4)=4/5$. There is no observation at $3$, so there is no jump there. The five observations produce only four distinct jump locations.

<a id="image-building-an-empirical-distribution-function-by-counting-observations"></a>
![](empirical-distribution-step-construction.png)

**[Figure 6](#image-building-an-empirical-distribution-function-by-counting-observations). Building an empirical distribution function by counting observations**. The chosen [statistical sample](statistical-sample.md) is $[1,1,2,4,6]$. Stacked marks retain the two observations at $1$. Open circles show excluded heights and filled circles show the value at each jump of the [right-continuous](right-continuous-function.md) [step function](step-function.md). The right axis gives the cumulative count, five times the [empirical distribution function](empirical-distribution-function.md).

The convention $X_i\leq x$ makes the [empirical distribution function](empirical-distribution-function.md) [right-continuous](right-continuous-function.md): once a threshold reaches an observation, that observation remains counted immediately to its right. For a finite [statistical sample](statistical-sample.md), the count is constant from any $x$ up to the next larger observed value, proving [right continuity](right-continuous-function.md). Its left-hand [limit](limit-of-a-function.md) $F_n(x^-)$ counts observations strictly below $x$, so

$$
F_n(x)-F_n(x^-)=\frac{\#\{i:X_i=x\}}n.
$$

A value occurring $m$ times causes one jump of size $m/n$. At $1$ the jump is $2/5$; at $2$, $4$, and $6$ each jump is $1/5$. All jumps sum to one. Thus the [empirical distribution function](empirical-distribution-function.md) is a [nondecreasing](nondecreasing-function.md) [step function](step-function.md) with limits zero and one, and is itself a valid [cumulative distribution function](cumulative-distribution-function.md).

This turns many questions about data into simple [cumulative distribution function](cumulative-distribution-function.md) operations. The observed fraction in $(a,b]$ is $F_n(b)-F_n(a)$: for $(1,4]$ it is $4/5-2/5=2/5$, counting $2$ and $4$ but excluding both $1$s. Including the left endpoint gives $F_n(4)-F_n(1^-)=4/5$. A [sample quantile](sample-quantile.md) reads the same staircase in reverse: the smallest threshold reaching $1/2$ is $2$. Unlike a [histogram](histogram.md), this representation requires no choice of bins; its jumps retain every observation and its multiplicity.

The exact description of a finite [statistical sample](statistical-sample.md) must be distinguished from a [statistical model](statistical-model-split.md) for how it was obtained. The [empirical distribution function](empirical-distribution-function.md) is defined for any finite list, with no [independence](independent-random-variables.md) assumption. Once the list is observed, its counts are fixed. For [statistical inference](statistical-inference-split.md), one often models $X_1,\ldots,X_n$ as [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) with an unknown population [cumulative distribution function](cumulative-distribution-function.md) $F(x)=\mathbb P(X_i\leq x)$. Then $F$ describes the sampling law, while $F_n$ varies across repeated [statistical samples](statistical-sample.md). The value $F_5(1)=0.4$ is an observed fraction and an estimate of $F(1)$; it does not establish that the population [probability](probability.md) is $0.4$. Even when $F$ is continuous, every finite $F_n$ is discrete.

For any threshold $x$ fixed before sampling, the [indicator functions](indicator-function.md) are [independent](independent-random-variables.md) [Bernoulli random variables](bernoulli-distribution.md) with success [probability](probability.md) $F(x)$. Therefore the count has a [binomial distribution](binomial-distribution.md) and

$$
nF_n(x)\sim\operatorname{Binomial}(n,F(x)),\qquad
\mathbb E[F_n(x)]=F(x),\qquad
\operatorname{Var}(F_n(x))=\frac{F(x)(1-F(x))}{n}.
$$

The [expected value](expected-value-split.md) follows by adding the [expected values](expected-value-split.md) of the [indicator functions](indicator-function.md); the [variance](variance-split.md) follows by adding their [variances](variance-split.md) using [independence](independent-random-variables.md) and dividing by $n^2$. Thus $F_n(x)$ is an [unbiased estimator](unbiased-estimator.md) of $F(x)$ at a fixed threshold. Controlling the error at every threshold at once requires more than a fixed-threshold calculation: the [DKW inequality](dvoretzky-kiefer-wolfowitz-inequality.md) supplies such control, and the [Glivenko-Cantelli theorem](glivenko-cantelli-theorem.md) describes its [uniform convergence](uniform-convergence.md) [almost surely](almost-sure-convergence.md) as $n$ grows.

Comparing $F_n$ with a proposed [cumulative distribution function](cumulative-distribution-function.md) also motivates [goodness-of-fit tests](goodness-of-fit-test.md), including the [Kolmogorov-Smirnov test](kolmogorov-smirnov-test.md), the [Anderson–Darling test](anderson-darling-test.md), and the [Cramér–von Mises criterion](cramer-von-mises-criterion.md). A standard [Kolmogorov-Smirnov test](kolmogorov-smirnov-test.md) calibration assumes a fully specified continuous population law; fitting its [statistical parameters](statistical-parameter.md) from the same [statistical sample](statistical-sample.md) changes that calibration.[NIST and SEMATECH e-Handbook of Statistical Methods; Characteristics and Limitations, items 1 and 3; Definition, test statistic and fully specified distribution requirement](nist-and-sematech-e-handbook-of-statistical-methods/1-3-5-16-kolmogorov-smirnov-goodness-of-fit-test.md)

**Table of contents**

- [Dvoretzky-Kiefer-Wolfowitz inequality](dvoretzky-kiefer-wolfowitz-inequality.md)
- [Simultaneous empirical distribution confidence band](simultaneous-empirical-distribution-confidence-band.md)
- [Anderson–Darling test](anderson-darling-test.md)
- [Cramér–von Mises criterion](cramer-von-mises-criterion.md)
- [Empirical distribution process](empirical-distribution-process.md)
  - [Donsker theorem for empirical distribution functions](donsker-theorem-for-empirical-distribution-functions.md)
  - [Finite-dimensional Brownian bridge limit of an empirical distribution process](finite-dimensional-brownian-bridge-limit-of-an-empirical-distribution-process.md)

## ↑ Ancestors (7)

1. [Cumulative distribution function](cumulative-distribution-function.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (25)

- [Cramér–von Mises criterion](cramer-von-mises-criterion.md)
- [Empirical distribution function](empirical-distribution-function.md)
- [Empirical distribution process](empirical-distribution-process.md)
- [Hill estimator](hill-estimator.md)
- [Kaplan–Meier estimator](kaplan-meier-estimator.md)
- [Kolmogorov-Smirnov statistic](kolmogorov-smirnov-statistic.md)
- [Kolmogorov-Smirnov test](kolmogorov-smirnov-test.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-43/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-42/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-42/6/vii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-42/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-33/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28/2/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28/2/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-34/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-210/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-210/1/solution.md)
- [Quantile proof of the Glivenko-Cantelli theorem](quantile-proof-of-the-glivenko-cantelli-theorem.md)
- [Sample median](sample-median.md)
- [Sample quantile](sample-quantile.md)
- [Simultaneous empirical distribution confidence band](simultaneous-empirical-distribution-confidence-band.md)
- [Two-sample Kolmogorov-Smirnov test](two-sample-kolmogorov-smirnov-test.md)
