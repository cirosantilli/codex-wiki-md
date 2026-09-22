<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $S_i$ be singleton deliveries among $C_i$ treatment cycles. Under a common-probability [binomial distribution](../../../../../../binomial-distribution.md) model, $S_i\sim\operatorname{Bin}(C_i,p)$ independently across years. The pooled [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is

$$
\widehat p=\frac{\sum_iS_i}{\sum_iC_i}=\frac{40429}{323362}=0.1250271.
$$

The [Pearson chi-squared test of homogeneity](../../../../../../pearson-chi-squared-test-of-homogeneity.md) compares singleton and non-singleton counts across all fourteen years, using

$$
X^2=\sum_{i=1}^{14}\left[\frac{(S_i-C_i\widehat p)^2}{C_i\widehat p}
+\frac{((C_i-S_i)-C_i(1-\widehat p))^2}{C_i(1-\widehat p)}\right]
=\sum_{i=1}^{14}\frac{(S_i-C_i\widehat p)^2}{C_i\widehat p(1-\widehat p)}.
$$

All expected cells are large. One probability has been estimated, so the reference [chi-squared distribution](../../../../../../chi-squared-distribution.md) has 13 degrees of freedom. Numerically,

$$
\boxed{X^2=1188.812,\quad \mathrm{df}=13,\quad p\simeq4.52\times10^{-246}.}
$$

**The constant singleton-per-cycle probability is decisively rejected under the independent-binomial model.** The observed proportion rises from $1712/18201=0.0941$ to $3626/23794=0.1524$. Dependence between repeated treatments or patient heterogeneity can invalidate literal binomial precision, but they should be addressed by an explicit variance model rather than ignored.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
