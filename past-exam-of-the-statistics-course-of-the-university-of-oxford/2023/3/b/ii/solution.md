<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [posterior mean](../../../../../posterior-mean.md) is a [convex combination](../../../../../convex-combination.md) of the [prior mean](../../../../../prior-mean.md) and the usual [Poisson](../../../../../poisson-distribution.md) [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md):

$$
\boxed{\mathbb E(\theta\mid\boldsymbol x)=\frac{r+s}{\lambda+n}=\frac\lambda{\lambda+n}\frac r\lambda+\frac n{\lambda+n}\bar x}.
$$

Both weights are positive and sum to one, so the mean lies between $r/\lambda$ and $\bar x$, strictly between them unless they coincide. If all counts are zero, $\bar x=0$ is the boundary estimate in the usual nonnegative Poisson parameter space; with a strictly positive parameter restriction it represents the likelihood supremum at that boundary. The displayed posterior-mean relation is valid in either interpretation.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the statistics course of the University of Oxford](../../../../split.md)
6. [Statistics course of the University of Oxford](../../../../../statistics-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
