<h1 id="chebyshev-s-inequality">Chebyshev's inequality</h1>

↑ **Parent:** [Probability inequality](probability-inequality-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chebyshev's_inequality)

For a real [random variable](random-variable-split.md) $X$ with finite [variance](variance-split.md) $\sigma^2$, [expected value](expected-value-split.md) $\mu$, and a threshold $a>0$, [Chebyshev's inequality](chebyshev-s-inequality.md) gives

$$
\mathbb P(|X-\mu|\geq a)\leq\frac{\sigma^2}{a^2}.
$$

One can also cap this upper bound at one, since a [probability](probability.md) cannot exceed one. If $\sigma>0$, taking $a=k\sigma$ gives $\mathbb P(|X-\mu|\geq k\sigma)\leq1/k^2$. For example, at least $3/4$ of the [probability](probability.md) lies strictly within two [standard deviations](standard-deviation.md) of the [mean](expected-value-split.md). This statement needs only the finite [variance](variance-split.md) assumption. If the [variance](variance-split.md) is zero, $X=\mu$ [almost surely](almost-sure-convergence.md) and every positive deviation threshold has zero [tail probability](tail-probability.md).

Consider a [random variable](random-variable-split.md) uniformly distributed on $\{-2,-1,0,1,2\}$. Its [expected value](expected-value-split.md) is zero and its [variance](variance-split.md) is $(4+1+0+1+4)/5=2$. At $a=2$ the actual [tail probability](tail-probability.md) is $2/5$, while [Chebyshev's inequality](chebyshev-s-inequality.md) gives $2/2^2=1/2$. At $a=3$ the actual [tail probability](tail-probability.md) is zero, while the bound is $2/9$. A valid bound need not describe the exact shape or bounded support of a particular [probability distribution](probability-distribution-split.md).

<a id="image-a-general-variance-bound-can-be-loose-for-a-normal-distribution-and-exact-for-another-distribution"></a>
![](chebyshev-bound-and-sharpness.png)

**[Figure 2](#image-a-general-variance-bound-can-be-loose-for-a-normal-distribution-and-exact-for-another-distribution). A general variance bound can be loose for a normal distribution and exact for another distribution**. Left: the two-sided [tail probability](tail-probability.md) of the [standard normal distribution](standard-normal-distribution.md) is compared with the capped [Chebyshev's inequality](chebyshev-s-inequality.md) bound. Right: the three-point [probability distribution](probability-distribution-split.md) places [probabilities](probability.md) $1/8$, $3/4$, $1/8$ at $-2$, $0$, $2$, giving [variance](variance-split.md) one and [probability](probability.md) $1/4$ at a deviation of at least two. The points at the threshold are included by $\geq$.

For the [standard normal distribution](standard-normal-distribution.md), the actual [tail probabilities](tail-probability.md) beyond two and three [standard deviations](standard-deviation.md) are approximately $0.0455003$ and $0.0026998$, whereas the general bounds are $1/4$ and $1/9$. More knowledge of the [probability distribution](probability-distribution-split.md) can therefore improve the estimate. The comparison does not diminish the guarantee: the three-point example in [equality in Chebyshev's inequality](equality-in-chebyshev-s-inequality.md) attains it exactly.

The proof is a one-line use of [Markov's inequality](markov-s-inequality.md) on the nonnegative [random variable](random-variable-split.md) $Y=(X-\mu)^2$. The event $|X-\mu|\geq a$ equals $Y\geq a^2$, and $\mathbb E Y=\sigma^2$. This explains why the denominator is squared and why a finite [variance](variance-split.md) supplies the necessary information. [Scott Sheffield, MIT 18.175, lecture 8: Markov and Chebyshev bounds](https://ocw.mit.edu/courses/18-175-theory-of-probability-spring-2014/887e96172e82a615dac16fb26702d88b_MIT18_175S14_Lecture8.pdf).

One important use is control of a [sample mean](sample-mean.md). For [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) with finite [variance](variance-split.md) $\sigma^2$, the [variance of a sample mean](variance-of-a-sample-mean.md) is $\sigma^2/n$. Hence

$$
\mathbb P(|\overline X_n-\mu|\geq\varepsilon)\leq\frac{\sigma^2}{n\varepsilon^2},\qquad \varepsilon>0.
$$

For every fixed tolerance, the bound tends to zero as the [sample size](sample-size.md) grows, proving the finite-[variance](variance-split.md) case of the [weak law of large numbers](weak-law-of-large-numbers.md). For $\sigma^2=1$ and $\varepsilon=0.1$, $n=2000$ makes the bound $0.05$. This is a sufficient bound under the stated assumptions, rather than an optimal required [sample size](sample-size.md).

An early historical source is [Pafnuty Chebyshev](pafnuty-chebyshev.md)'s 1867 paper “Des valeurs moyennes”, published in French translation by N. de Khanikof. Its opening theorem bounds deviations of sums using their [expected values](expected-value-split.md) and [second moments](second-moment.md), linking averages with control of exceptional outcomes. [Chebyshev, Journal de mathématiques pures et appliquées, 2nd series 12, 177–184 (1867)](https://www.numdam.org/item/JMPA_1867_2_12__177_0.pdf).

**Table of contents**

- [Equality in Chebyshev's inequality](equality-in-chebyshev-s-inequality.md)
- [Cantelli inequality](cantelli-inequality.md)
  - [Equality in Cantelli's inequality](equality-in-cantelli-s-inequality.md)

## ↑ Ancestors (6)

1. [Probability inequality](probability-inequality-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (33)

- [Bernstein polynomial](bernstein-polynomial.md)
- [Brownian exit-skeleton clock convergence](brownian-exit-skeleton-clock-convergence.md)
- [Cantelli inequality](cantelli-inequality.md)
- [Chebyshev's inequality](chebyshev-s-inequality.md)
- [Concentration of discrete cubes at diameter scale](concentration-of-discrete-cubes-at-diameter-scale.md)
- [Efron–Stein inequality](efron-stein-inequality.md)
- [Equality in Chebyshev's inequality](equality-in-chebyshev-s-inequality.md)
- [Exponential Markov bound](exponential-markov-bound.md)
- [Markov's inequality](markov-s-inequality.md)
- [Normal scale mixture representation of Student t](normal-scale-mixture-representation-of-student-t.md)
- [Pafnuty Chebyshev](pafnuty-chebyshev.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-27/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-34/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-32/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-71/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/12f/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-33/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-58/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-14/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-31/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-69/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-11/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-2/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-112/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/11f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-339/3/a/i/solution.md)
- [Probability inequality](probability-inequality-split.md)
- [Second moment method](second-moment-method.md)
- [Typical-set concentration for a biased coin](typical-set-concentration-for-a-biased-coin.md)
- [Variance of a sample mean](variance-of-a-sample-mean.md)
- [Weak law without an absolute first moment](weak-law-without-an-absolute-first-moment.md)
