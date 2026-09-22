<h1 id="13j/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let

$$
\widetilde{\mathcal M}_1
=\{(\nu_1\mathbf1_m,\ldots,\nu_n\mathbf1_m):
(\nu_1,\ldots,\nu_n)\in\mathbb R^n\}
$$

be the block-saturated mean space, and let

$$
\widetilde{\mathcal M}_0
=\{(\mu_1(\beta)\mathbf1_m,\ldots,
\mu_n(\beta)\mathbf1_m):\beta\in\mathbb R^p\}
$$

be the fitted GLM mean space. Full column rank and the regularity assumptions give dimensions $n$ and $p$. The factorization in part (ii) makes the nuisance factor cancel from their likelihood ratio, while $\bar Y\overset d=Y$ gives

$$
\frac{D(Y;\widehat\mu)}{\sigma^2}
\overset d=
2\log
\frac{
\sup_{\tilde\mu\in\widetilde{\mathcal M}_1}
f(\widetilde Y;\tilde\mu,\tilde\sigma^2)}{
\sup_{\tilde\mu\in\widetilde{\mathcal M}_0}
f(\widetilde Y;\tilde\mu,\tilde\sigma^2)}.
$$

As $\sigma^2\to0$, the replicate count $m=1/\sigma^2$ tends to infinity. [Wilks theorem](../../../../../../../wilks-theorem.md) applied to these nested regular models makes twice the log-likelihood ratio converge in distribution to a chi-squared variable with the difference in dimensions:

$$
\boxed{
\frac{D(Y;\widehat\mu)}{\sigma^2}
\xrightarrow d\chi^2_{n-p}}.
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [13J](../../../13j.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
