<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [residual deviance](../../../../../../residual-deviance.md) is $290.93$ on $98$ [residual degrees of freedom](../../../../../../residual-degrees-of-freedom.md). Under a suitable Poisson [deviance goodness-of-fit test](../../../../../../deviance-goodness-of-fit-test.md) approximation it is compared with $\chi^2_{98}$, whose supplied 95th percentile is $122.1$. Since $290.93$ is much larger, **the chosen Poisson model does not provide a satisfactory absolute fit**, despite being preferred among the three candidates.

The ratio $290.93/98\approx2.97$ suggests substantial [overdispersion](../../../../../../overdispersion.md) or mean-model misspecification. It is a deviance ratio, not the exact [Pearson dispersion estimator](../../../../../../pearson-dispersion-estimator.md), which cannot be computed from the excerpt. Check residual patterns, nonlinear effects, unusual rivers and dependence. A [Quasi-Poisson regression](../../../../../../quasi-poisson-regression.md) could adjust uncertainty under an estimated dispersion, and a [negative binomial regression](../../../../../../negative-binomial-regression.md) could model extra count variation; a more adequate mean model may also be needed. The nominal Poisson tests in part (a) should be interpreted in light of this failure, rather than treated as a validated final analysis.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
