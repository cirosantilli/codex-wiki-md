<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use a proper [normal distribution](../../../../../../normal-distribution.md) prior centered at zero on the [log odds ratio](../../../../../../log-odds-ratio.md). For example,

$$
\boxed{\beta\sim N(0,1)}
$$

puts approximately 95 percent of its mass between $-2$ and $2$, giving [odds ratios](../../../../../../odds-ratio.md) roughly between $e^{-2}$ and $e^2$, close to $1/8$ and $8$. Centering at zero treats reciprocal [odds ratios](../../../../../../odds-ratio.md) symmetrically. If the desired central 95 percent interval is exactly $(1/8,8)$, use [standard deviation](../../../../../../standard-deviation.md) $\log8/\Phi^{-1}(0.975)\simeq1.0610$. **A soft prior is appropriate for implausibility**, whereas a bounded [uniform prior](../../../../../../uniform-prior.md) would declare effects outside the limits impossible.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
