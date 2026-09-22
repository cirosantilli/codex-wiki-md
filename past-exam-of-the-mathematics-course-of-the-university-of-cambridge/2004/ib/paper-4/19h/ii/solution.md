<h1 id="19h/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

This relative [absolute-error loss](../../../../../../absolute-error-loss.md) weights each parameter by $1/\theta$. Its [posterior expected loss](../../../../../../posterior-expected-loss.md) is

$$
R_x(a)=b^2\int_0^\infty|\theta-a|e^{-b\theta}d\theta.
$$

The effective density for the [Bayes estimator under weighted absolute loss](../../../../../../bayes-estimator-under-weighted-absolute-loss.md) is proportional to $\pi(\theta\mid x)/\theta$, hence an [exponential distribution](../../../../../../exponential-distribution.md) of rate $b$. Its median solves $1-e^{-ba}=1/2$.

More explicitly, for $a\geq0$, differentiating the split integrals at $\theta=a$ gives $R_x'(a)=b(1-2e^{-ba})$ and $R_x''(a)=2b^2e^{-ba}>0$. For $a<0$, the loss has derivative $-b$, so its minimum cannot lie there. The unique global minimum is therefore

$$
\boxed{\widehat\theta_B(X)=\frac{\log2}{\mu+X}.}
$$

This is the [weighted posterior median](../../../../../../bayes-estimator-under-weighted-absolute-loss.md); the ordinary median of the Gamma posterior would minimize unweighted absolute loss and would give a different answer.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [19H](../../19h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
