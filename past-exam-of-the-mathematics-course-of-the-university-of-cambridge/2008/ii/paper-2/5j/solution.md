<h1 id="5j/solution">Solution</h1>

↑ **Parent:** [5J](../5j.md)

Under independent [normal distributions](../../../../../normal-distribution.md), [maximum likelihood estimation](../../../../../maximum-likelihood-estimation.md) minimizes $(y_A-\alpha)^2+(y_B-\beta)^2+(y_C-\gamma)^2$ subject to $\alpha+\beta+\gamma=\pi$. A [Lagrange multiplier](../../../../../lagrange-multiplier.md) gives the same correction at every corner. Writing $s=y_A+y_B+y_C$, the interior estimates are

$$
\boxed{\widehat\alpha=y_A+\frac{\pi-s}{3},\quad\widehat\beta=y_B+\frac{\pi-s}{3},\quad\widehat\gamma=y_C+\frac{\pi-s}{3}.}
$$

The result is unchanged if the common [variance](../../../../../variance-split.md) is unknown, since profiling it still minimizes the residual sum of squares. If physical positivity of the three angles is imposed and this projection gives a negative component, the constrained estimate over the closed simplex is instead $\widehat\theta_i=\max(y_i-\lambda,0)$, with $\lambda$ chosen to make the components sum to $\pi$. If only strictly nondegenerate triangles are admitted, a boundary optimum is merely an unattained likelihood supremum.

The normal-error model is a useful small-error approximation, but its unbounded tails assign positive probability to impossible measured angles. Periodicity or a measurement convention may matter for large errors, and equal [variance](../../../../../variance-split.md) and independence require experimental justification. The exact sum constraint on the true angles does not itself invalidate independence of three raw measurement errors. After imposing that constraint, however, the fitted-angle errors are correlated: the covariance of the interior estimator is $\sigma^2(I-\boldsymbol1\boldsymbol1^T/3)$.

## ↑ Ancestors (10)

1. [5J](../5j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
