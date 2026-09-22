# Survival function

↑ **Parent:** [Survival analysis](survival-analysis-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Survival_function)

For a nonnegative [survival time](survival-time.md) $T$, the [survival function](survival-function.md) is

$$
S(t)=\mathbb P(T>t)=1-F(t),\qquad F(t)=\mathbb P(T\leq t),
$$

where $F$ is the [cumulative distribution function](cumulative-distribution-function.md). Thus $S(t)$ is the [probability](probability.md) that the chosen occurrence is still in the future at time $t$. We consistently use the strict inequality $T>t$: a [probability mass](probability-mass.md) at $t$ has already left the [survival function](survival-function.md) at $t$ itself. With this convention $S$ is a [right-continuous function](right-continuous-function.md) and a [nonincreasing function](nonincreasing-function.md) taking values in $[0,1]$. If $\mathbb P(T=0)=0$, then $S(0)=1$; if $T$ is finite with [probability](probability.md) one, then $S(t)\to0$ as $t\to\infty$.

For $S(a)>0$ and $b>a$, [conditional probability](conditional-probability.md) gives

$$
\mathbb P(T>b\mid T>a)=\frac{S(b)}{S(a)},\qquad
\mathbb P(a<T\leq b\mid T>a)=1-\frac{S(b)}{S(a)}.
$$

For example, $S(2)=0.8$ and $S(5)=0.6$ mean that $0.6/0.8=0.75$ of those still event-free at year two remain event-free through year five. Their intervening event [probability](probability.md) is $0.25$, whereas the original population's [probability](probability.md) of an occurrence in $(2,5]$ is $0.8-0.6=0.2$. Conditioning changes the denominator.

The area under the [survival function](survival-function.md) up to a horizon gives the [restricted mean survival time](restricted-mean-survival-time.md). A positive terminal plateau in a plotted [Kaplan–Meier estimator](kaplan-meier-estimator.md) does not establish that the occurrence will never happen: [terminal censoring and survival-mean identifiability](terminal-censoring-and-survival-mean-identifiability.md) explains why the unobserved tail remains undetermined.

**Table of contents**

- [Mean residual life](mean-residual-life.md)
- [Restricted mean survival time](restricted-mean-survival-time.md)
- [Hazard function](hazard-function.md)
  - [Poisson record counts in cumulative hazard coordinates](poisson-record-counts-in-cumulative-hazard-coordinates.md)
  - [Discrete hazard](discrete-hazard.md)
  - [Population hazard of a survival mixture](population-hazard-of-a-survival-mixture.md)
    - [Decreasing population hazard under constant individual hazards](decreasing-population-hazard-under-constant-individual-hazards.md)
    - [Survival selection in a heterogeneous population](survival-selection-in-a-heterogeneous-population.md)
    - [Hazard derivative for a mixture of exponential distributions](hazard-derivative-for-a-mixture-of-exponential-distributions.md)
  - [Cumulative hazard function](cumulative-hazard-function.md)
    - [Mean accumulated hazard under independent censoring](mean-accumulated-hazard-under-independent-censoring.md)
    - [Mean accumulated hazard before fixed censoring](mean-accumulated-hazard-before-fixed-censoring.md)
    - [Cumulative hazard probability transformation](cumulative-hazard-probability-transformation.md)
  - [Hazard ratio](hazard-ratio.md)

## ↑ Ancestors (5)

1. [Survival analysis](survival-analysis-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (52)

- [Cumulative hazard function](cumulative-hazard-function.md)
- [Discrete hazard](discrete-hazard.md)
- [Exponential survival risk over an interval](exponential-survival-risk-over-an-interval.md)
- [Extreme value theory](extreme-value-theory.md)
- [Finite Erlang-mixture tail for a negative-binomial exponential aggregate](finite-erlang-mixture-tail-for-a-negative-binomial-exponential-aggregate.md)
- [First-passage-time density](first-passage-time-density.md)
- [Fréchet distribution](frechet-distribution.md)
- [Gumbel limit for gamma maxima](gumbel-limit-for-gamma-maxima.md)
- [Hazard function](hazard-function.md)
- [Independent censoring](independent-censoring.md)
- [Kaplan–Meier estimator](kaplan-meier-estimator.md)
- [Kaplan–Meier estimator with delayed entry](kaplan-meier-estimator-with-delayed-entry.md)
- [Mean accumulated hazard before fixed censoring](mean-accumulated-hazard-before-fixed-censoring.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/1/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/1/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/2/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/2/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/2/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-29/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-2/10f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-2/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-41/5/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-42/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-101/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-37/5/b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-37/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-32/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32/7/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32/7/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-34/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-59/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/5/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-33/5/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-34/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2/10f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1/13j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207/4/c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-210/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/14b/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-207/5/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-207/6/solution.md)
- [Right censoring](right-censoring.md)
- [Right endpoint of a distribution](right-endpoint-of-a-distribution.md)
- [Survival analysis](survival-analysis-split.md)
- [Survival function](survival-function.md)
- [Survival time](survival-time.md)
- [Tail probability](tail-probability.md)
- [Von Mises conditions for extreme values](von-mises-conditions-for-extreme-values.md)
