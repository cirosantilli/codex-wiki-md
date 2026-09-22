<h1 id="markov-s-inequality">Markov's inequality</h1>

↑ **Parent:** [Probability inequality](probability-inequality-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Markov's_inequality)

For a nonnegative [random variable](random-variable-split.md) $Y$ and threshold $a>0$, [Markov's inequality](markov-s-inequality.md) gives

$$
\mathbb P(Y\geq a)\leq\frac{\mathbb E Y}{a}.
$$

The useful case has finite [expected value](expected-value-split.md); an infinite right side gives no finite information. The bound also holds if $Y$ is nonnegative [almost surely](almost-sure-convergence.md). Combining it with the elementary bound one gives $\mathbb P(Y\geq a)\leq\min\{1,\mathbb E Y/a\}$. Nonnegativity is essential: negative values could otherwise cancel the contribution of large positive values to the [expected value](expected-value-split.md).

The idea is an average budget. Every outcome where $Y\geq a$ contributes at least $a$ times its [probability](probability.md) to $\mathbb E Y$, and the other outcomes contribute nonnegative amounts. Formally, the [indicator function](indicator-function.md) gives $Y\geq a\mathbf1_{\{Y\geq a\}}$; taking the [expected value](expected-value-split.md) proves the bound. [Sheffield, MIT 18.175, lecture 8: the expectation argument](https://ocw.mit.edu/courses/18-175-theory-of-probability-spring-2014/887e96172e82a615dac16fb26702d88b_MIT18_175S14_Lecture8.pdf).

For example, let $Y$ take $0$, $1$, $2$, $5$ with respective [probabilities](probability.md) $0.5$, $0.2$, $0.2$, $0.1$. Its [expected value](expected-value-split.md) is $1.1$. At $a=2$, the [tail probability](tail-probability.md) is $0.3$, while the bound is $1.1/2=0.55$. At $a=5$, the [tail probability](tail-probability.md) is $0.1$, while the bound is $0.22$. A different [probability distribution](probability-distribution-split.md) with the same [expected value](expected-value-split.md), putting masses $0.78$ and $0.22$ at $0$ and $5$, attains the bound $0.22$ exactly at $a=5$.

<a id="image-an-average-bounds-how-much-probability-can-lie-beyond-a-positive-threshold"></a>
![](markov-average-and-tail.png)

**[Figure 5](#image-an-average-bounds-how-much-probability-can-lie-beyond-a-positive-threshold). An average bounds how much probability can lie beyond a positive threshold**. Left: the stipulated four-point [probability distribution](probability-distribution-split.md) has [expected value](expected-value-split.md) $1.1$. Right: its exact [tail probability](tail-probability.md) $\mathbb P(Y\geq a)$ and the capped [Markov's inequality](markov-s-inequality.md) bound. Filled markers include an atom at the threshold; open markers show the smaller value immediately after it. The highlighted threshold $a=2$ has actual [probability](probability.md) $0.3$ and bound $0.55$.

[Markov's inequality](markov-s-inequality.md) is useful when a [moment](moment.md) is easy to compute but a full [probability distribution](probability-distribution-split.md) is difficult to determine. A nonnegative count with [expected value](expected-value-split.md) less than one must have some positive [probability](probability.md) of being zero, giving the [first moment method](first-moment-method.md). Applying the same bound to a squared centered [random variable](random-variable-split.md) gives [Chebyshev's inequality](chebyshev-s-inequality.md). Applying it to an [exponential function](exponential-function.md) of a [random variable](random-variable-split.md) gives an [exponential Markov bound](exponential-markov-bound.md), which can exploit more than a single [moment](moment.md).

**Table of contents**

- [Equality in Markov's inequality](equality-in-markov-s-inequality.md)
- [Exponential Markov bound](exponential-markov-bound.md)

## ↑ Ancestors (6)

1. [Probability inequality](probability-inequality-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (30)

- [Cantelli inequality](cantelli-inequality.md)
- [Chebyshev's inequality](chebyshev-s-inequality.md)
- [Equality in Cantelli's inequality](equality-in-cantelli-s-inequality.md)
- [Equality in Markov's inequality](equality-in-markov-s-inequality.md)
- [Exponential Markov bound](exponential-markov-bound.md)
- [First moment method](first-moment-method.md)
- [Hoeffding inequality](hoeffding-inequality.md)
- [Markov's inequality](markov-s-inequality.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-24/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-24/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-41/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2/25j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-15/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-31/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-2/10f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-2/10f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-32/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-12/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-12/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-2/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-67/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-67/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-112/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2/10f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-2/3f/solution.md)
- [Probability inequality](probability-inequality-split.md)
- [QMA error reduction](qma-error-reduction.md)
