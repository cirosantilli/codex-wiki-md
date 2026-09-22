<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $L(\vartheta;x)$ be the [likelihood function](../../../../likelihood-function.md), with full parameter space $\Theta$ and [null hypothesis](../../../../null-hypothesis.md) $\vartheta\in\Theta_0\subseteq\Theta$. The [generalized likelihood-ratio test](../../../../generalized-likelihood-ratio-test.md) compares the best null fit to the best unrestricted fit:

$$
R(x)=\frac{\sup_{\vartheta\in\Theta_0}L(\vartheta;x)}
{\sup_{\vartheta\in\Theta}L(\vartheta;x)},
\qquad \Lambda(x)=-2\log R(x).
$$

The [likelihood ratio](../../../../likelihood-ratio.md) $R$ lies between zero and one, and small values count against the [null hypothesis](../../../../null-hypothesis.md); equivalently, large values of the [likelihood-ratio test statistic](../../../../likelihood-ratio-test-statistic.md) $\Lambda$ count against it.

Compute restricted and unrestricted [maximum-likelihood estimates](../../../../maximum-likelihood-estimator.md), evaluate their [log-likelihoods](../../../../log-likelihood.md), and form $\Lambda=2(\ell(\widehat\vartheta)-\ell(\widehat\vartheta_0))$. Under the regular conditions of [Wilks theorem](../../../../wilks-theorem.md), the null limit is

$$
\Lambda\xrightarrow{d}\chi_d^2,\qquad
d=\dim\Theta-\dim\Theta_0.
$$

These [statistical degrees of freedom](../../../../statistical-degrees-of-freedom.md) count independent parameter restrictions. The regularity includes a locally identifiable smooth model, nonsingular [Fisher information](../../../../fisher-information-matrix.md), and an interior null value; parameter-dependent support can invalidate the result.

For a chosen [significance level](../../../../significance-level.md) $\alpha$, obtain the $(1-\alpha)$ [quantile](../../../../quantile-function.md) $q_{d,1-\alpha}$ of the [chi-squared distribution](../../../../chi-squared-distribution.md) and use

$$
\boxed{\text{reject }H_0\text{ if }\Lambda_{\rm obs}>q_{d,1-\alpha}.}
$$

Equivalently, compare the asymptotic [p-value](../../../../p-value.md) $\Pr(\chi_d^2\geq\Lambda_{\rm obs})$ to $\alpha$. This is a large-sample calibration; part (c) requires direct treatment because its support depends on a parameter.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the statistics course of the University of Oxford](../../../split.md)
5. [Statistics course of the University of Oxford](../../../../statistics-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
