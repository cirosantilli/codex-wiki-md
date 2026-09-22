<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Generate [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) $X_1,\ldots,X_n$ with [probability density function](../../../../../probability-density-function.md) $p$, evaluate $\phi(X_i)$ for each draw, and return the [Monte Carlo estimator](../../../../../monte-carlo-estimator.md)

$$
\boxed{\widehat\theta_n^{\mathrm{MC}}=\frac1n\sum_{i=1}^n\phi(X_i).}
$$

[Linearity of expectation](../../../../../linearity-of-expectation.md) makes this an [unbiased estimator](../../../../../unbiased-estimator.md): $\mathbb E\widehat\theta_n^{\mathrm{MC}}=\theta$. Independence and the specified [variance](../../../../../variance-split.md) give $\operatorname{Var}(\widehat\theta_n^{\mathrm{MC}})=1/n$. Its [Monte Carlo standard error](../../../../../monte-carlo-standard-error.md) is therefore $n^{-1/2}$, and the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) gives convergence to $\theta$ [almost surely](../../../../../almost-sure-convergence.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
