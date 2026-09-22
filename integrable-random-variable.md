# Integrable random variable

↑ **Parent:** [Expected value](expected-value.md)

A real or complex [random variable](random-variable-split.md) $X$ is integrable when $\mathbb E|X|<\infty$. This is [integrability](integrability.md) with respect to its [probability measure](probability-measure.md), and ensures that its [expected value](expected-value.md) is finite. A bounded [random variable](random-variable-split.md) is always an [integrable random variable](integrable-random-variable.md); so is the example taking $-1,2,8$, for which $\mathbb E|X|=2.7$.

For a real [random variable](random-variable-split.md), put $X_+=\max(X,0)$ and $X_-=\max(-X,0)$, its [positive part](positive-part-of-a-real-valued-function.md) and [negative part](negative-part-of-a-real-valued-function.md). Each has a nonnegative [Lebesgue integral](lebesgue-integral.md), possibly infinite. The expression $\mathbb E[X]=\mathbb E[X_+]-\mathbb E[X_-]$ is defined when at least one of these two [expected values](expected-value.md) is finite; if both are infinite, the [expected value](expected-value.md) is undefined. [Integrability](integrability.md) makes both finite. A nonnegative [random variable](random-variable-split.md) can have [expected value](expected-value.md) $+\infty$, even though it is not an [integrable random variable](integrable-random-variable.md).

The standard [Cauchy distribution](cauchy-distribution.md) is a useful warning. With its [probability density function](probability-density-function.md) $f(x)=1/[\pi(1+x^2)]$, the positive contribution is $\int_0^Rxf(x)\,dx=\log(1+R^2)/(2\pi)$, which tends to infinity; the negative contribution has the same magnitude. Integrating symmetrically over $[-R,R]$ gives zero for each $R$, but this cancellation does not define an [expected value](expected-value.md). The [Cauchy sample mean has an unchanged distribution](cauchy-sample-mean-has-an-unchanged-distribution.md), showing why the [integrability](integrability.md) hypothesis in the [strong law of large numbers](strong-law-of-large-numbers.md) matters.

For an [integrable random variable](integrable-random-variable.md), [conditional expectation](conditional-expectation.md) preserves [integrability](integrability.md), and [linearity of expectation](linearity-of-expectation.md) can safely combine finite averages without forming $\infty-\infty$.

## ↑ Ancestors (6)

1. [Expected value](expected-value.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (42)

- [Almost sure submartingale convergence theorem](almost-sure-submartingale-convergence-theorem.md)
- [Bounded-increment optional stopping with integrable time](bounded-increment-optional-stopping-with-integrable-time.md)
- [Bounded stopping time](bounded-stopping-time.md)
- [Conditional expectation](conditional-expectation.md)
- [Conditional expectation of a summand given future partial sums](conditional-expectation-of-a-summand-given-future-partial-sums.md)
- [Conditional expectation preserving a distribution](conditional-expectation-preserving-a-distribution.md)
- [Count-weighted Laplace functional of a Poisson random measure](count-weighted-laplace-functional-of-a-poisson-random-measure.md)
- [Expected value](expected-value.md)
- [Integrable random variable](integrable-random-variable.md)
- [Jensen's inequality](jensen-s-inequality.md)
- [L1 contraction of conditional expectation](l1-contraction-of-conditional-expectation.md)
- [L1 convergence implies uniform integrability](l1-convergence-implies-uniform-integrability.md)
- [Law of the unconscious statistician](law-of-the-unconscious-statistician.md)
- [Law of total expectation](law-of-total-expectation.md)
- [Linearity of expectation](linearity-of-expectation.md)
- [Mean under one-sided exponential tilting](mean-under-one-sided-exponential-tilting.md)
- [Nested conditioning keeps the coarser information](nested-conditioning-keeps-the-coarser-information.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-27/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-29/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-32/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-29/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-29/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/24j/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/30k/a/solution.md)
- [Strong law for adjacent products](strong-law-for-adjacent-products.md)
- [Tail probability](tail-probability.md)
- [Uniform integrability of conditional expectations](uniform-integrability-of-conditional-expectations.md)
- [Uniformly integrable martingale convergence theorem](uniformly-integrable-martingale-convergence-theorem.md)
- [Wald's equation](wald-s-equation.md)
