<h1 id="12h/solution">Solution</h1>

↑ **Parent:** [12H](../12h.md)

Model the two samples as independent multinomial counts with fixed row totals $N_A=N_B=500$ and three category probabilities. The null hypothesis is $p_{Aj}=p_{Bj}=p_j$ for every category $j$. Up to combinatorial factors the [likelihood](../../../../../likelihood-function.md) is $\prod_{ij}p_{ij}^{O_{ij}}$. Without the null restriction its maximizers are $O_{ij}/N_i$; under the null, maximizing $\sum_j(O_{Aj}+O_{Bj})\log p_j$ subject to $\sum_jp_j=1$ gives

$$
\widehat p_j=\frac{O_{Aj}+O_{Bj}}{1000},\qquad
E_{ij}=N_i\widehat p_j.
$$

The observed column totals are $243,281,476$, giving fitted expected counts **$(121.5,140.5,238)$ in each row**.

To derive the null distribution, put $D=O_A-O_B$. Under the null its mean is zero and covariance is $1000(\operatorname{diag}p-pp^T)$. The multivariate [central limit theorem](../../../../../central-limit-theorem.md) gives, asymptotically, the standardized contrast $Z_j=D_j/\sqrt{1000p_j}$ a centered [normal distribution](../../../../../normal-distribution.md) with covariance

$$
I-uu^T,\qquad u=(\sqrt{p_1},\sqrt{p_2},\sqrt{p_3})^T,\quad u^Tu=1.
$$

This is the [orthogonal projection](../../../../../orthogonal-projection.md) onto a two-dimensional plane. In an orthonormal [basis](../../../../../basis.md) of that plane, the two nonzero coordinates are independent standard normal variables, so $\sum_jZ_j^2$ tends to $\chi_2^2$. The pooled estimates are consistent; substituting them for $p_j$ leaves this limit unchanged by [Slutsky's theorem](../../../../../slutsky-theorem.md). Since $O_{Aj}-E_{Aj}=D_j/2$ and $O_{Bj}-E_{Bj}=-D_j/2$, the resulting statistic is precisely the [Pearson chi-squared test of homogeneity](../../../../../pearson-chi-squared-test-of-homogeneity.md) statistic

$$
X^2=\sum_{i,j}\frac{(O_{ij}-E_{ij})^2}{E_{ij}}
=\sum_j\frac{D_j^2}{1000\widehat p_j},\qquad X^2\xrightarrow{d}\chi_2^2.
$$

This supplies the two degrees of freedom rather than treating all six cells as independent. Every fitted expected count is large, supporting the approximation.

For these data,

$$
\boxed{X^2=2\left(\frac{18.5^2}{121.5}+\frac{4.5^2}{140.5}
+\frac{14^2}{238}\right)=7.56906.}
$$

It exceeds the two-degree-of-freedom 95th percentile $5.99$, but not the 99th percentile $9.21$. Hence **reject equal score distributions at the 5% level, but not at the 1% level**. The asymptotic p-value is $\Pr(\chi_2^2\ge7.56906)=e^{-7.56906/2}\simeq0.02272$.

## ↑ Ancestors (10)

1. [12H](../12h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
