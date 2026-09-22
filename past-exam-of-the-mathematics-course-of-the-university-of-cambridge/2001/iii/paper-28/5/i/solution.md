<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the index order in the probability specification: influence $i$, accommodation type $j$, contact $k$ and satisfaction $l$. Put $N_{ijk}=n_{ijk+}$, which is conditioned on. The independent [multinomial likelihood](../../../../../../multinomial-likelihood.md) is

$$
L(p;n)=\prod_{ijk}\frac{N_{ijk}!}{\prod_ln_{ijkl}!}\prod_lp_{ijkl}^{n_{ijkl}},\qquad\sum_lp_{ijkl}=1.
$$

Thus the relevant sample is a collection of conditional satisfaction distributions for fixed covariate strata; it is not a model for the marginal distribution of the three covariates. In the published dataset there are three influence, four accommodation, two contact and three satisfaction levels, giving 24 strata and 72 cells; these dimensions are documented in [https://stat.ethz.ch/R-manual/R-devel/library/MASS/html/housing.html](https://stat.ethz.ch/R-manual/R-devel/library/MASS/html/housing.html) .

The missing output does not identify its two actual formulas. Two standard canonical models can nevertheless be derived explicitly, and the following general result identifies the sufficient statistics for any specified baseline-logit model. The first standard model has no response/covariate association: $p_{ijkl}=q_l$ for every stratum. Its likelihood factors as

$$
L(q;n)=h(n)\prod_lq_l^{n_{+++l}}.
$$

Therefore **the pooled satisfaction totals $n_{+++l}$ are sufficient**, with only two independent totals because the grand total is fixed. The [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is $\widehat q_l=n_{+++l}/1681$, and fitted counts are $N_{ijk}\widehat q_l$. A Poisson surrogate formula with all covariate-stratum interactions and only a satisfaction main effect produces this same conditional model. It has two conditional parameters and 46 residual degrees of freedom when all 24 strata are present.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
