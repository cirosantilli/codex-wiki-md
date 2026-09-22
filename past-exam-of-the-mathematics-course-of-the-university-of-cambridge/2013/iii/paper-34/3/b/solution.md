<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $\eta_{ik}=\beta_k^T\mathbf x_i$, so $\eta_{i1}=0$. The [multinomial logistic regression](../../../../../../multinomial-logistic-regression.md) implies $p_{ik}=e^{\eta_{ik}}p_{i1}$. Normalizing gives

$$
p_{ik}=\frac{e^{\eta_{ik}}}{S_i},\qquad
S_i=\sum_{j=1}^Ke^{\eta_{ij}}
=1+\sum_{j=2}^Ke^{\eta_{ij}}.
$$

Multiply the [multinomial likelihoods](../../../../../../multinomial-likelihood.md) for conditionally independent groups. The multinomial coefficients are constant in $\beta$, leaving

$$
\boxed{L(\beta)\propto\prod_{i=1}^I
\frac{\exp\{\sum_{k=1}^K y_{ik}\beta_k^T\mathbf x_i\}}
{\{\sum_{k=1}^K\exp(\beta_k^T\mathbf x_i)\}^{n_i}}.}
$$

The reference constraint $\beta_1=0$ identifies the coefficients: a common shift of every category coefficient otherwise leaves all probabilities unchanged. The PDF places the full sum inside the numerator exponent; the TeX breaks that expression.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
