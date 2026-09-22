<h1 id="o/o1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\ell_n(\theta)=\sum_{i=1}^n\log f(X_i;\theta)$ be the [log-likelihood](../../../../../log-likelihood.md). Under the usual regularity conditions, the expected [Fisher information](../../../../../fisher-information-matrix.md) in the whole sample is

$$
\boxed{I_n(\theta)=\mathbb E_\theta\!\left[\{\ell_n'(\theta)\}^2\right]
=-\mathbb E_\theta[\ell_n''(\theta)]=nI_1(\theta).}
$$

The equality of the two expressions uses [mean](../../../../../expected-value-split.md)-zero score and permitted differentiation of the normalization identity. Independent observations make the information additive. The [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) has [asymptotic normality](../../../../../asymptotic-normality.md):

$$
\sqrt n(\widehat\theta-\theta)\xrightarrow{d}N(0,I_1(\theta)^{-1}),
\qquad
\boxed{\widehat\theta\ \text{approximately}\ N(\theta,I_n(\theta)^{-1}).}
$$

The factor $n$ is included in $I_n$; it must not be inserted a second time into the [variance](../../../../../variance-split.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [O1](../../o1.md)
3. [O](../../../o.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options I course of the University of Oxford](../../../../split.md)
6. [Options I course of the University of Oxford](../../../../../options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
