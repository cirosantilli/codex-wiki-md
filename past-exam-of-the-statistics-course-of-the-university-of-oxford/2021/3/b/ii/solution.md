<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $M_0=\alpha+x_0\beta$. As a [linear combination of independent normal random variables](../../../../../linear-combination-of-independent-normal-random-variables.md) under the [posterior distribution](../../../../../bayesian-posterior.md),

$$
M_0\mid\boldsymbol y\sim N(m_0,v_0),\qquad
m_0=m_\alpha+x_0m_\beta,\qquad
v_0=v_\alpha+x_0^2v_\beta.
$$

The shortest 95% [credible interval](../../../../../credible-interval.md) is

$$
\boxed{\left[m_\alpha+x_0m_\beta
-\Phi^{-1}(0.975)\sqrt{v_\alpha+x_0^2v_\beta},\quad
m_\alpha+x_0m_\beta
+\Phi^{-1}(0.975)\sqrt{v_\alpha+x_0^2v_\beta}\right]}.
$$

Here $\Phi$ is the [standard normal distribution](../../../../../standard-normal-distribution.md) [cumulative distribution function](../../../../../cumulative-distribution-function.md). To justify shortest length, consider all intervals of a fixed length $d$. If $f$ is this [normal distribution](../../../../../normal-distribution.md) [posterior density](../../../../../posterior-density.md), the interval probability $\int_a^{a+d}f(t)\,dt$ has [derivative](../../../../../derivative.md) $f(a+d)-f(a)$ with respect to $a$. The [normal distribution](../../../../../normal-distribution.md) is symmetric and its density strictly decreases with distance from its [mean](../../../../../expected-value-split.md), so this probability is uniquely maximized when the midpoint is $m_0$. The centered interval can therefore attain 95% [posterior probability](../../../../../posterior-probability.md) with the least length. It is both an [equal-tailed credible interval](../../../../../equal-tailed-credible-interval.md) and a [highest posterior density interval](../../../../../highest-posterior-density-interval.md).

The target is the experiment's [mean](../../../../../expected-value-split.md) at $x_0$. A [posterior predictive distribution](../../../../../posterior-predictive-distribution.md) for a new noisy observation would instead have [variance](../../../../../variance-split.md) $v_0+\sigma^2$; that extra observation [variance](../../../../../variance-split.md) does not belong in the requested interval.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
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
