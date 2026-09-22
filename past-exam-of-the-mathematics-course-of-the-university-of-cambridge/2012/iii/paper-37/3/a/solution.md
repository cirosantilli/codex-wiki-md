<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Index independent experimental vials by $r$, write $N_r$ for the observed total eaten and $E_r$ for the number of other-species eggs eaten. The [grouped-binomial logistic regression](../../../../../../grouped-binomial-logistic-regression.md) uses

$$
E_r\mid N_r\sim\operatorname{Bin}(N_r,p_r),\qquad
\operatorname{logit}(p_r)=\log\frac{p_r}{1-p_r}=\beta_0+d_{D_r}+s_{S_r},
\qquad d_1=0,\quad s_A=0.
$$

Here $D_r\in\{1,2,3\}$ and $S_r\in\{A,B,C\}$ identify day and adult species, and the free effects are $\beta_0,d_2,d_3,s_B,s_C$. There is no day-species interaction. The weights in the binomial [generalized linear model](../../../../../../generalized-linear-model.md) are the denominators $N_r$, so fitting the proportions $E_r/N_r$ gives this [binomial likelihood](../../../../../../binomial-likelihood.md), not 23 Bernoulli observations. The dispersion is fixed at one. This is a model for the composition of eggs eaten conditional on the total, rather than a model for the total appetite.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
