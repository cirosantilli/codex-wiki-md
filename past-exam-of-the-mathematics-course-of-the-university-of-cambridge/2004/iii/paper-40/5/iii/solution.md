<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

An exact [Gibbs sampler](../../../../../../gibbs-sampler.md) update is available despite the non-Gaussian intercept: draw $\theta'$ from the conditional [gamma distribution](../../../../../../gamma-distribution.md) law in part (ii), then set

$$
\boxed{\mu'=\log\theta'.}
$$

Together with conditional updates of the two remaining effects, this targets the required joint posterior in the log-intercept coordinates. The [log-gamma prior for a Poisson log-intercept](../../../../../../log-gamma-prior-for-a-poisson-log-intercept.md) includes the change-of-variable factor: with $d\theta/d\mu=e^\mu$,

$$
\pi(\mu\mid a_2,b_2,\mathbf x)
\propto\exp\{(a+T)\mu-(b+E)e^\mu\}.
$$

Using $(a+T-1)\mu$ instead would omit the Jacobian and give the wrong conditional law for $\mu$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
