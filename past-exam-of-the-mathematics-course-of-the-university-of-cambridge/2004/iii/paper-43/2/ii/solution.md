<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $n=\sum_{\nu=1}^gn_\nu$, $\bar x_\nu=n_\nu^{-1}\sum_jx_j^{(\nu)}$ and $\bar x=n^{-1}\sum_\nu n_\nu\bar x_\nu$. Define the within-group and between-group scatter [matrices](../../../../../../matrix.md) by

$$
\boxed{W=\sum_{\nu=1}^g\sum_{j=1}^{n_\nu}(x_j^{(\nu)}-\bar x_\nu)(x_j^{(\nu)}-\bar x_\nu)^T,\qquad B=\sum_{\nu=1}^gn_\nu(\bar x_\nu-\bar x)(\bar x_\nu-\bar x)^T.}
$$

The [within-group and between-group scatter decomposition](../../../../../../within-group-and-between-group-scatter-decomposition.md) gives total scatter $T=W+B$: in each group the residuals about $\bar x_\nu$ sum to zero, so all cross terms vanish. Under unrestricted group [means](../../../../../../expected-value.md), the [maximum-likelihood estimators](../../../../../../maximum-likelihood-estimator.md) are $\widehat\mu_\nu=\bar x_\nu$ and $\widehat V=W/n$. Under the common-mean [null hypothesis](../../../../../../null-hypothesis.md), they are $\widehat\mu=\bar x$ and $\widehat V_0=(W+B)/n$.

For either fitted scatter [matrix](../../../../../../matrix.md) $A$, substitution into the [log-likelihood](../../../../../../log-likelihood.md) gives

$$
\ell_{\max}(A)=-\frac{np}{2}\log(2\pi)-\frac n2\log|A/n|-\frac{np}{2},
$$

since $\operatorname{tr}[(A/n)^{-1}A]=np$. Thus the maximized [likelihood ratio](../../../../../../likelihood-ratio.md) is

$$
\Lambda_{\mathrm{LR}}=\frac{\sup_{H_0}L}{\sup_{H_1}L}=\left(\frac{|W|}{|W+B|}\right)^{n/2}.
$$

A [generalized likelihood-ratio test](../../../../../../generalized-likelihood-ratio-test.md) rejects for small $\Lambda_{\mathrm{LR}}$, equivalently

$$
\boxed{\log\frac{|W+B|}{|W|}>c.}
$$

The cutoff $c$ is chosen for the desired significance level. The determinant ratio $|W|/|W+B|$ itself is the [Wilks lambda statistic](../../../../../../wilks-lambda-statistic.md). The derivation assumes $W$ is [positive-definite](../../../../../../positive-definite-bilinear-form.md), which for continuous normal samples requires enough within-group degrees of freedom, $n-g\geq p$; singular $W$ does not support this ordinary determinant-based test without a modified model.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
