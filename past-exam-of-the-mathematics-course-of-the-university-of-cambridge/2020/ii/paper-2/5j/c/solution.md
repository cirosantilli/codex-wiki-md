<h1 id="5j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\varepsilon_i$ be independent standard [logistic random variables](../../../../../../logistic-distribution.md) and define the [latent variable](../../../../../../latent-variable.md)

$$
Z_i=-4.50161+0.02521\,\mathrm{height}_i
+0.02313\,\mathrm{cigs}_i+\varepsilon_i.
$$

Set $Y_i=1$ exactly when $Z_i>0$. If $F$ is the logistic [cumulative distribution function](../../../../../../cumulative-distribution-function.md), its symmetry and the identity $F^{-1}(p)=\operatorname{logit}(p)$ give

$$
\mathbb P(Y_i=1)=F(-4.50161+0.02521\,\mathrm{height}_i+0.02313\,\mathrm{cigs}_i),
$$

which is precisely the fitted [logistic regression](../../../../../../logistic-regression.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5J](../../5j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
