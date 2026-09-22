<h1 id="13k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $Y_i$ be the number of survivors among the $n_i$ patients in row $i$. The fitted [grouped-binomial logistic regression](../../../../../../grouped-binomial-logistic-regression.md) is

$$
Y_i\ \mathrel{\mathop\sim^{\mathrm{ind}}}\ \operatorname{Bin}(n_i,p_i),
$$

with

$$
\log\frac{p_i}{1-p_i}
=\beta_0+\beta_B\mathbf1\{\text{site}_i=B\}
+\beta_C\mathbf1\{\text{site}_i=C\}
+\beta_M\mathbf1\{\text{malignant}_i=\text{yes}\}.
$$

Site A and nonmalignant tumours are the reference levels. There is no site-by-malignancy interaction, so the malignancy log-odds effect is assumed to be the same at all three sites. In the R call, `survive/total` supplies the observed proportions and `weights = total` supplies the binomial denominators $n_i$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [13K](../../13k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
