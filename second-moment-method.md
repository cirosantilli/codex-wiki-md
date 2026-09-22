# Second moment method

↑ **Parent:** [Probability inequality](probability-inequality-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Second_moment_method)

The second moment method uses a [random variable](random-variable-split.md)'s [expected value](expected-value.md) and [second moment](second-moment.md) to establish that a counted or measured quantity is positive with substantial [probability](probability.md). It is useful when a positive average alone could be caused by extremely large values on very rare outcomes. Controlling the [variance](variance-split.md) rules out too much of that concentration in rare outcomes.

For a nonnegative [random variable](random-variable-split.md) $N$ with $m=\mathbb EN>0$ and finite [second moment](second-moment.md), the [second-moment bound for positivity](second-moment-bound-for-positivity.md) gives

$$
\boxed{\mathbb P(N>0)\geq\frac{(\mathbb EN)^2}{\mathbb E N^2}=\frac{m^2}{m^2+\operatorname{Var}(N)}.}
$$

Equivalently, $\mathbb P(N=0)\leq\operatorname{Var}(N)/(m^2+\operatorname{Var}(N))$. The method also includes the simpler [Chebyshev's inequality](chebyshev-s-inequality.md) bound $\mathbb P(N=0)\leq\operatorname{Var}(N)/m^2$. Thus a [sequence](sequence.md) of such [random variables](random-variable-split.md) with $\operatorname{Var}(N)/(\mathbb EN)^2\to0$ has $N>0$ with [probability](probability.md) tending to one. These statements require no [independence](independent-random-variables.md) assumption. The variance argument and its use for random counts are developed in Zhao's lecture notes. [Yufei Zhao, MIT 18.226, §4.1, corollaries 4.1.7–4.1.8: variance and non-existence](https://ocw.mit.edu/courses/18-226-probabilistic-methods-in-combinatorics-fall-2022/mit18_226_f22_lec06-07.pdf).

For an original toy count, let $N$ count successes in ten [independent](independent-random-variables.md) [Bernoulli trials](bernoulli-trial.md) with success [probability](probability.md) $p=1/10$. The [binomial distribution](binomial-distribution.md) gives

$$
\mathbb EN=1,\qquad \operatorname{Var}(N)=9/10,\qquad \mathbb E N^2=19/10.
$$

Consequently **$\mathbb P(N>0)\geq10/19\approx0.526316$**. The exact [probability](probability.md) is $1-(9/10)^{10}\approx0.651322$. The [first moment method](first-moment-method.md) and [union bound](boole-s-inequality.md) only give the upper bound $\mathbb P(N>0)\leq\min\{1,\mathbb EN\}=1$ here. First and second moments therefore answer complementary existence questions.

<a id="image-the-second-moment-method-certifies-a-positive-count-while-statistical-dependence-can-change-the-conclusion-despite-an-unchanged-mean"></a>
![](second-moment-count-positivity-and-dependence.png)

**[Figure 4](#image-the-second-moment-method-certifies-a-positive-count-while-statistical-dependence-can-change-the-conclusion-despite-an-unchanged-mean). The second moment method certifies a positive count, while statistical dependence can change the conclusion despite an unchanged mean**. Left: exact [binomial distribution](binomial-distribution.md) probabilities of at least one success and second-moment lower bounds for ten [independent](independent-random-variables.md) trials as the success probability varies. Right: the same ten trials with $p=1/10$ either occur independently or share one common [Bernoulli](bernoulli-distribution.md) outcome. Both counts have [mean](expected-value.md) one, but the perfectly linked count has much larger [variance](variance-split.md) and only $1/10$ probability of being positive. All data are original specified probability models.

For a [sum](sum.md) of [indicator random variables](indicator-random-variable.md), the [variance of a sum](variance-of-a-sum.md) is

$$
\operatorname{Var}\left(\sum_i I_i\right)=\sum_i\operatorname{Var}(I_i)+2\sum_{i<j}\operatorname{Cov}(I_i,I_j).
$$

[Independence](independent-random-variables.md) makes the [covariances](covariance.md) vanish, but the formula itself also covers dependent counts. For the same ten success probabilities, let every trial share a single [Bernoulli random variable](bernoulli-distribution.md) $B$: then $N=10B$, with [mean](expected-value.md) one, [variance](variance-split.md) nine, and $\mathbb P(N>0)=1/10$. The second-moment lower bound is exactly $1/10$. Ignoring the positive [covariances](covariance.md) would produce the false independent-count conclusion. Zhao's discussion of sums of indicators explains why overlapping counted structures require these pairwise terms. [Zhao, MIT 18.226, §4.1: indicator covariances and Bernoulli counts](https://ocw.mit.edu/courses/18-226-probabilistic-methods-in-combinatorics-fall-2022/mit18_226_f22_lec06-07.pdf).

**Table of contents**

- [Second-moment bound for positivity](second-moment-bound-for-positivity.md)

## ↑ Ancestors (6)

1. [Probability inequality](probability-inequality-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (18)

- [First moment method](first-moment-method.md)
- [Growing-clique overlap bound](growing-clique-overlap-bound.md)
- [Lyapunov moment inequality](lyapunov-moment-inequality.md)
- [Overlap formula for the variance of a clique count](overlap-formula-for-the-variance-of-a-clique-count.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-12/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-36/3/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2/12f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-112/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ia/paper-1/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/17h/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-2/12f/iv/solution.md)
- [Second-moment bound for positivity](second-moment-bound-for-positivity.md)
- [Second moment method](second-moment-method.md)
- [Sharp subcritical largest-component scale](sharp-subcritical-largest-component-scale.md)
- [Triangle count in a binomial random graph](triangle-count-in-a-binomial-random-graph.md)
- [Triangle-existence threshold in a binomial random graph](triangle-existence-threshold-in-a-binomial-random-graph.md)
