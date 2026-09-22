<h1 id="13j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $y_{i+}=\sum_jy_{ij}$ and $\mu_{i+}=\sum_j\mu_{ij}$. Under the model in part (a),

$$
\mu_{i+}=e^{\alpha_i}\sum_je^{\beta_j},
\qquad
p_j:=\frac{\mu_{ij}}{\mu_{i+}}
=\frac{e^{\beta_j}}{\sum_ke^{\beta_k}},
$$

and $p_j$ is independent of the price category $i$. The [Poisson-multinomial conditioning](../../../../../../poisson-multinomial-conditioning.md) identity gives

$$
(Y_{i1},Y_{i2},Y_{i3})\mid Y_{i+}=y_{i+}
\sim\operatorname{Multinomial}(y_{i+};p_1,p_2,p_3).
$$

More explicitly, the [likelihood function](../../../../../../likelihood-function.md) for row $i$ factors as

$$
\prod_j\frac{e^{-\mu_{ij}}\mu_{ij}^{y_{ij}}}{y_{ij}!}
=
\frac{e^{-\mu_{i+}}\mu_{i+}^{y_{i+}}}{y_{i+}!}
\frac{y_{i+}!}{\prod_jy_{ij}!}\prod_jp_j^{y_{ij}}.
$$

The first factor is the likelihood of the row total and the second is the conditional [multinomial likelihood](../../../../../../multinomial-likelihood.md). The free price effect $\alpha_i$ makes the first factor maximal at $\widehat\mu_{i+}=y_{i+}$, while maximizing the remaining factors gives

$$
\widehat p_j=\frac{y_{+j}}{y_{++}}.
$$

Consequently both fits have the same [maximum-likelihood fitted value](../../../../../../maximum-likelihood-fitted-value.md)

$$
\boxed{\widehat\mu_{ij}=y_{i+}\widehat p_j
=\frac{y_{i+}y_{+j}}{y_{++}}}.
$$

Here every row total is $30$, the column totals are $31,28,31$, and $y_{++}=90$, so every fitted row is

$$
\boxed{(31/3,\ 28/3,\ 31/3)}.
$$

This factorization is the [Poisson trick](../../../../../../poisson-trick.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [13J](../../13j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
