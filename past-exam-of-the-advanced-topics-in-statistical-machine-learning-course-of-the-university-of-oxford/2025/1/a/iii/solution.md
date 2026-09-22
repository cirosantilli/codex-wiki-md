<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Evaluate [Bayes' theorem](../../../../../bayes-theorem.md) at the [posterior mode](../../../../../maximum-a-posteriori-estimate.md) $\mu$:

$$
p(\mathcal D)=\frac{p(\mathcal D\mid\mu)p(\mu)}{p(\mu\mid\mathcal D)}.
$$

The [multivariate normal density](../../../../../multivariate-normal-density.md) in the [Laplace approximation](../../../../../laplace-approximation.md) has height $(2\pi)^{-d/2}|\Sigma|^{-1/2}$ at its [mean](../../../../../expected-value-split.md). Therefore

$$
\boxed{p(\mathcal D)\simeq p(\mathcal D\mid\mu)p(\mu)(2\pi)^{d/2}|\Sigma|^{1/2}}.
$$

Equivalently, the approximate log [marginal likelihood](../../../../../bayesian-model-evidence.md) is

$$
\boxed{\log p(\mathcal D)\simeq\log p(\mathcal D\mid\mu)+\log p(\mu)+\frac d2\log(2\pi)+\frac12\log|\Sigma|}.
$$

The [determinant](../../../../../determinant.md) factor accounts for the volume of the locally plausible parameter region, which the peak [likelihood](../../../../../likelihood-function.md) alone does not measure.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
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
