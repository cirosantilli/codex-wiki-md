<h1 id="james-stein-estimator">James–Stein estimator</h1>

↑ **Parent:** [Admissible estimator](admissible-estimator.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/James–Stein_estimator)

For one observation $X\sim N_p(\theta,I_p)$ with $p\geq3$, the James–Stein estimator is

$$
\delta_{\rm JS}(X)=
\left(1-\frac{p-2}{\lVert X\rVert^2}\right)X.
$$

Under [quadratic loss](squared-error-loss.md), Stein's risk identity gives

$$
R(\theta,\delta_{\rm JS})
=p-(p-2)^2\mathbb E_\theta\frac1{\lVert X\rVert^2}<p,
$$

so it dominates the usual estimator $X$.

**Table of contents**

- [James–Stein shrinkage toward the sample mean](james-stein-shrinkage-toward-the-sample-mean.md)
- [Identical worst-case risk under strict James-Stein domination](identical-worst-case-risk-under-strict-james-stein-domination.md)

## ↑ Ancestors (9)

1. [Admissible estimator](admissible-estimator.md)
2. [Admissible decision rule](admissible-decision-rule.md)
3. [Risk function](risk-function.md)
4. [Statistical modelling](statistical-modelling-split.md)
5. [Statistical model](statistical-model-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-1/28k/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1/25j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/28k/b/solution.md)
