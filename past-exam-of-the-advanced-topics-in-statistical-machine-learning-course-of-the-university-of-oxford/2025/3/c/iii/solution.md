<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**Additional observations weakly decrease the [posterior variance](../../../../../posterior-variance.md) at every fixed prediction input.** Apply part (ii) repeatedly to add observations one at a time. An observation whose remaining [conditional covariance](../../../../../conditional-covariance.md) with $f_*$ is nonzero strictly decreases that [posterior variance](../../../../../posterior-variance.md); one with zero remaining [conditional covariance](../../../../../conditional-covariance.md) leaves it unchanged. Large observation noise reduces the information gained through the denominator $v_{n-1}(x_n)+\sigma^2$.

For fixed [Gaussian process](../../../../../gaussian-process-split.md) hyperparameters and a [Gaussian likelihood](../../../../../gaussian-likelihood.md), the [posterior variance](../../../../../posterior-variance.md) depends on the observation locations and noise level, but not on the observed numerical outputs. Hence the reduction holds for each possible new output, rather than only on average. The [predictive variance](../../../../../predictive-variance.md) of a future noisy observation also decreases by the same amount because its extra independent noise [variance](../../../../../variance-split.md) is fixed. Refitting the hyperparameters after adding data can change the [covariance function](../../../../../covariance-function.md); the monotonicity statement compares conditioning under one fixed model.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the advanced topics in statistical machine learning course of the University of Oxford](../../../../split.md)
6. [Advanced topics in statistical machine learning course of the University of Oxford](../../../../../advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics and statistics course of the University of Oxford](../../../../../year-4-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
