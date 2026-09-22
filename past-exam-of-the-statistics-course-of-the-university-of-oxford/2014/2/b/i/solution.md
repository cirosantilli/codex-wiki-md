<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [sample mean](../../../../../sample-mean.md) $\overline X=T/n$ has [mean](../../../../../expected-value-split.md) $\theta$ and [variance](../../../../../variance-split.md) $\sigma(\theta)^2=\theta(1-\theta)/n$. The [central limit theorem](../../../../../central-limit-theorem.md) gives a [normal approximation](../../../../../normal-approximation.md) for interior $\theta$ when both expected binomial counts are sufficiently large. Under the [null hypothesis](../../../../../null-hypothesis.md), a level-$\alpha$ upper-tail cutoff is approximately

$$
\overline X>\theta_0+\sigma(\theta_0)z_\alpha,\qquad\Phi(z_\alpha)=1-\alpha.
$$

To obtain the [power function](../../../../../power-function-of-a-statistical-test.md), evaluate this same cutoff under the true [statistical parameter](../../../../../statistical-parameter.md) $\theta$, standardizing with $\sigma(\theta)$:

$$
\begin{aligned}
w(\theta)&\approx\Pr_\theta\!\left(\frac{\overline X-\theta}{\sigma(\theta)}>
\frac{\theta_0-\theta+\sigma(\theta_0)z_\alpha}{\sigma(\theta)}\right)\\
&=\boxed{1-\Phi\!\left(\frac{\theta_0-\theta}{\sigma(\theta)}+
\frac{\sigma(\theta_0)}{\sigma(\theta)}z_\alpha\right).}
\end{aligned}
$$

Here $\Phi$ is the [standard normal distribution](../../../../../standard-normal-distribution.md)'s [cumulative distribution function](../../../../../cumulative-distribution-function.md). The formula treats the binomial threshold as continuous; exact integer cutoffs and boundary randomization are finite-sample refinements.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
