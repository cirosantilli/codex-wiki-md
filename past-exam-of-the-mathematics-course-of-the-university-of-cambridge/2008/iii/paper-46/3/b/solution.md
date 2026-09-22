<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under [independent censoring](../../../../../../independent-censoring.md) conditional on the modelled [covariates](../../../../../../covariate.md), an observed event contributes $f_i(x_i)=h_i(x_i)e^{-H_i(x_i)}$, and a right-censored observation contributes $S_i(x_i)=e^{-H_i(x_i)}$. Factors from the censoring distribution may be omitted when they contain no survival-model parameters. The [survival likelihood](../../../../../../survival-likelihood.md) and [log-likelihood](../../../../../../log-likelihood.md) are therefore

$$
\boxed{L=\prod_i h_i(x_i)^{v_i}e^{-H_i(x_i)},\qquad
\ell=\sum_i v_i\log h_i(x_i)-\sum_iH_i(x_i).}
$$

Censored individuals still contribute their observed exposure through $H_i(x_i)$; they are not deleted from the analysis.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
