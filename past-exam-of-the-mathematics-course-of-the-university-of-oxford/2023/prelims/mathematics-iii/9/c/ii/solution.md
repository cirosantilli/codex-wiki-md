<h1 id="9/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The new score columns are orthogonal, since $Z^TZ=V^TX^TXV$ is diagonal. This decouples the slope [normal equations](../../../../../../../normal-equation.md); with positive eigenvalues and the stated error [covariance](../../../../../../../covariance.md), the two estimated score coefficients are uncorrelated. It also makes variance explained and possible dimension reduction explicit.

The trade-off is interpretation: each [principal component](../../../../../../../principal-component.md) is a mixture of the original variables, so its regression coefficient is less directly connected to changing one original input. Keeping both components is an invertible reparameterization and gives **exactly the same fitted values and residual sum of squares**. It does not repair a zero [eigenvalue](../../../../../../../eigenvalue.md) or remove instability associated with a very small one. Dropping a low-variance component may improve numerical stability and reduce estimator variance, but changes the model and can discard predictive information, since [principal component analysis](../../../../../../../principal-component-analysis.md) uses predictor variance rather than the response. This is the distinction between a full rotation and [principal component regression](../../../../../../../principal-component-regression.md) with truncation.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [9](../../../9.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
