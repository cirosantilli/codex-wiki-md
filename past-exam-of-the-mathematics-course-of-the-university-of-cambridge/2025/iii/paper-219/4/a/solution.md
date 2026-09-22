<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

One simple algorithm is [importance sampling](../../../../../../importance-sampling.md) from the prior. Draw $(\theta_j,\boldsymbol\alpha_j)$ independently from $\pi(\theta)\pi(\boldsymbol\alpha)$ and assign weight $w_j=L_A(\theta_j,\boldsymbol\alpha_j)$. Then

$$
\widehat{\mathcal Z}_A=\frac1J\sum_{j=1}^Jw_j
$$

estimates the [Bayesian model evidence](../../../../../../bayesian-model-evidence.md), and the normalized weights $w_j/\sum_kw_k$ represent the posterior. A weighted histogram or [kernel density estimation](../../../../../../kernel-density-estimation.md) of the $\theta_j$ estimates the marginal $\mathcal P_A(\theta)$; discarding $\boldsymbol\alpha_j$ performs the marginalization.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
