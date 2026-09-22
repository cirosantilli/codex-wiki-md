<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For response $j$ from subject $s$, model2 is the [generalized linear mixed model](../../../../../../generalized-linear-mixed-model.md)

$$
Y_{sj}\mid b_s\sim\operatorname{IG}(\mu_{sj},\lambda),
\qquad
\frac1{\mu_{sj}^2}=\beta_0+\beta_1d_{sj}+b_s,
\qquad
b_s\overset{\mathrm{iid}}\sim N(0,\tau^2),
$$

with conditional independence given the [random intercepts](../../../../../../random-intercept.md). The fitted values are $\widehat\beta_0=8.9966$, $\widehat\beta_1=-1.2317$, $\widehat\tau^2=1.7533$, and fitted residual dispersion $0.7591$.

The random intercept models persistent between-subject differences and the resulting within-subject dependence among repeated measurements. That is the main feature absent from model1.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
