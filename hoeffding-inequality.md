# Hoeffding inequality

↑ **Parent:** [Concentration inequality](concentration-inequality.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hoeffding's_inequality)

The [Hoeffding inequality](hoeffding-inequality.md) turns finite [interval](interval-mathematics.md) bounds and [independence](independent-random-variables.md) into exponentially small [tail probabilities](tail-probability.md) for a [sum](sum.md). It requires neither a [normal distribution](normal-distribution.md) nor identical [probability distributions](probability-distribution-split.md). Let $X_1,\ldots,X_n$ be [independent](independent-random-variables.md) [essentially bounded](essentially-bounded-function.md) real [random variables](random-variable-split.md), with deterministic finite bounds $a_i\leq X_i\leq b_i$ [almost surely](almost-sure-convergence.md). Define the centered [sum](sum.md) and its squared-width budget by

$$
S_n=\sum_{i=1}^n(X_i-\mathbb EX_i),\qquad V=\sum_{i=1}^n(b_i-a_i)^2.
$$

For $V>0$ and $t>0$,

$$
\boxed{\mathbb P(S_n\geq t)\leq e^{-2t^2/V},\qquad \mathbb P(S_n\leq-t)\leq e^{-2t^2/V}.}
$$

The [union bound](boole-s-inequality.md) therefore gives $\mathbb P(|S_n|\geq t)\leq\min\{1,2e^{-2t^2/V}\}$. If $V=0$, every $X_i$ is constant [almost surely](almost-sure-convergence.md), so $S_n=0$ and both positive-threshold [tail probabilities](tail-probability.md) vanish. The equal-width version is stated in the authored Stanford notes.[§3, p. 6, theorem 4: independent bounded variables and both tails](cs229-supplemental-lecture-notes/hoeffding%E2%80%99s-inequality.md)

The quantity $V$ is a sum of squared [interval](interval-mathematics.md) widths, **not the [variance](variance-split.md) of $S_n$**. Centering changes the endpoints to $a_i-\mathbb EX_i$ and $b_i-\mathbb EX_i$, leaving each width unchanged. For example, [independent](independent-random-variables.md) [random variables](random-variable-split.md) in $[-2,1]$ and $[4,5]$ have $V=3^2+1^2=10$, whatever their [expected values](expected-value-split.md) or [probability distributions](probability-distribution-split.md). A deviation at least three above their total [expected value](expected-value-split.md) has [probability](probability.md) at most $e^{-18/10}\approx0.165299$. If all widths equal $b-a>0$, the [sample mean](sample-mean.md) $\overline X_n=n^{-1}\sum_iX_i$ satisfies

$$
\mathbb P\left(|\overline X_n-\mathbb E\overline X_n|\geq\varepsilon\right)\leq\min\{1,2\exp(-2n\varepsilon^2/(b-a)^2)\},\qquad\varepsilon>0.
$$

[Independence](independent-random-variables.md) is essential to this general guarantee. Take one [Bernoulli random variable](bernoulli-distribution.md) $B$ with success [probability](probability.md) $1/2$ and set every $X_i=B$. Each lies in $[0,1]$, but for every $n$ the [sample mean](sample-mean.md) is either zero or one. Thus $\mathbb P(|\overline X_n-1/2|\geq1/4)=1$, whereas incorrectly inserting these dependent observations into the formula would give $2e^{-n/8}$, less than one for $n\geq6$. Some special dependent models have their own valid [concentration inequalities](concentration-inequality.md); arbitrary [statistical dependence](statistical-dependence.md) cannot be ignored.

For the short proof, apply [Markov's inequality](markov-s-inequality.md) to $e^{\lambda S_n}$ with $\lambda>0$, factor the [expectation](expected-value-split.md) using [independence](independent-random-variables.md), and apply the [Hoeffding lemma](hoeffding-lemma.md) to each factor:

$$
\mathbb P(S_n\geq t)\leq e^{-\lambda t}\prod_i\mathbb E e^{\lambda(X_i-\mathbb EX_i)}\leq\exp(-\lambda t+\lambda^2V/8).
$$

Minimizing this [quadratic polynomial](quadratic-polynomial.md) at $\lambda=4t/V$ gives the upper [tail probability](tail-probability.md); applying it to $-S_n$ gives the lower one. This is the [Chernoff bound](chernoff-bound.md) method. The original 1963 article is [Probability Inequalities for Sums of Bounded Random Variables by Wassily Hoeffding](probability-inequalities-for-sums-of-bounded-random-variables-by-wassily-hoeffding.md); its publisher record identifies the article, but its full text was unavailable during this source check. The argument above is a direct derivation rather than a claim to have inspected that article's proof.

**Table of contents**

- [Hoeffding sample size for Bernoulli frequencies](hoeffding-sample-size-for-bernoulli-frequencies.md)
- [Hoeffding confidence interval](hoeffding-confidence-interval.md)
- [Hoeffding lemma](hoeffding-lemma.md)

## ↑ Ancestors (7)

1. [Concentration inequality](concentration-inequality.md)
2. [Probability inequality](probability-inequality-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (20)

- [Annealing ratios for a matching generating function](annealing-ratios-for-a-matching-generating-function.md)
- [Bennett bounds for sparse binomial fluctuations](bennett-bounds-for-sparse-binomial-fluctuations.md)
- [BQP error reduction](bqp-error-reduction.md)
- [Hoeffding confidence interval](hoeffding-confidence-interval.md)
- [Hoeffding inequality](hoeffding-inequality.md)
- [Hoeffding lemma](hoeffding-lemma.md)
- [Hoeffding lower-tail bound for Hamming balls](hoeffding-lower-tail-bound-for-hamming-balls.md)
- [Hoeffding sample size for Bernoulli frequencies](hoeffding-sample-size-for-bernoulli-frequencies.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-13/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-10/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-63/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-36/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-67/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-209/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-210/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-210/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-223/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-205/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-208/1/c/solution.md)
