<h1 id="1/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The specified [asymptotic relative efficiency](../../../../../asymptotic-relative-efficiency.md) is

$$
\boxed{\frac{v(T_2)}{v(T_1)}
=\frac{\theta(\theta+2)}{(\theta+1)^2}
=1-\frac1{(\theta+1)^2}}.
$$

For every fixed $\theta>0$ this lies strictly between zero and one. **Prefer $T_2$ on grounds of asymptotic precision**: it has the smaller leading [asymptotic variance](../../../../../asymptotic-variance.md) and attains the inverse [Fisher information](../../../../../fisher-information-matrix.md). Both are [consistent estimators](../../../../../consistency-statistics.md), by the [law of large numbers](../../../../../law-of-large-numbers.md) and the [continuous mapping theorem](../../../../../continuous-mapping-theorem.md) applied respectively to $\bar X$ and $A/n$. The efficiency approaches zero as $\theta\downarrow0$ and one as $\theta\to\infty$.

This preference is an asymptotic comparison. In particular, it does not assert that $T_2$ is an [unbiased estimator](../../../../../unbiased-estimator.md): since $A$ has a [gamma distribution](../../../../../gamma-distribution.md) of shape $n$ and rate $\theta$, $\mathbb E T_2=n\theta/(n-1)$ for $n>1$.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
