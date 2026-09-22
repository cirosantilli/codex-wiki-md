<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Model "lme2" replaces $b_j$ by a random intercept and random PTHK slope:

$$
\operatorname{THK}_{ij}
=x_{ij}^T\beta+b_{0j}+b_{1j}\operatorname{PTHK}_{ij}
+\varepsilon_{ij},
$$

with a fitted bivariate normal covariance matrix for $(b_{0j},b_{1j})$. This adds a random-slope variance and an intercept-slope covariance.

The likelihood-ratio statistic is

$$
2\{-2680.4-(-2684.6)\}=8.4.
$$

An ordinary chi-squared reference is unreliable because the null random-slope variance is on the boundary and its correlation is unidentified there; the reported correlation of one also signals a nearly singular fit. A valid practical test is a [parametric bootstrap](../../../../../../parametric-bootstrap.md): simulate many datasets from fitted "lme1", refit both models by maximum likelihood to each, recompute the likelihood-ratio statistic, and estimate the p-value by the fraction at least $8.4$. The AIC favors "lme2" slightly, whereas its BIC is larger, so the descriptive criteria do not agree.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
