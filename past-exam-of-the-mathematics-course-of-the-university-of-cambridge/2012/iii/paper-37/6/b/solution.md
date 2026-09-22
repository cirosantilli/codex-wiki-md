<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the moment approach, write $m_i=\mathbb E Y_i$ and let $V_i$ be a positive-definite working [covariance](../../../../../../covariance.md) constructed from the proposed moment formulas. For identifiable mean coefficients $\theta$, let $D_i=\partial m_i/\partial\theta^T$. [Generalized estimating equations](../../../../../../generalized-estimating-equation.md) take the form

$$
\sum_{i=1}^m D_i^TV_i^{-1}(Y_i-m_i)=0.
$$

Across independent students, correct mean specification and standard regularity conditions give consistent identifiable mean coefficients even if the working [covariance](../../../../../../covariance.md) is wrong. [Sandwich covariance matrix](../../../../../../sandwich-covariance-matrix.md) [standard errors](../../../../../../standard-error.md) use

$$
A=\sum_iD_i^TV_i^{-1}D_i,\quad
B=\sum_iD_i^TV_i^{-1}(Y_i-m_i)(Y_i-m_i)^TV_i^{-1}D_i,\quad
\widehat{\operatorname{Cov}}(\widehat\theta)=A^{-1}BA^{-1}.
$$

Residual second-moment estimating equations can estimate identifiable dispersion and association parameters. The marginal mean only identifies $\gamma_0=\beta_0+\log(1-\pi)$, not $\beta_0$ and $\pi$ separately. Moment restrictions beyond the mean would be needed to separate them; as shown below, the printed restrictions do not generally recover the intended latent parameters.

For the hierarchical approach, maximize the [observed-data likelihood](../../../../../../observed-data-likelihood.md) after integrating out the [random effect](../../../../../../random-effect.md). Set $\mu_{ij}=e^{\beta_0+\beta^Tx_i+\alpha_j}$, $r=1/\tau$, $M_i=\sum_j\mu_{ij}$ and $s_i=\sum_jy_{ij}$. The joint likelihood contribution is

$$
L_i=\pi\mathbf1_{\{s_i=0\}}+(1-\pi)
\frac{\Gamma(r+s_i)}{\Gamma(r)}
\frac{r^r}{(r+M_i)^{r+s_i}}
\prod_{j=1}^3\frac{\mu_{ij}^{y_{ij}}}{y_{ij}!}.
$$

The integral comes from multiplying three conditional Poisson mass functions by the Gamma density and integrating $b_i^{r+s_i-1}e^{-(r+M_i)b_i}$ over $b_i>0$. Independent students give $\ell=\sum_i\log L_i$. Direct numerical maximum likelihood or an [expectation-maximization algorithm](../../../../../../expectation-maximization-algorithm.md) can be used; in an EM algorithm an all-zero profile has an uncertain latent component membership. Information-based likelihood [standard errors](../../../../../../standard-error.md) apply under regular interior conditions, with special care for parameter boundaries.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
