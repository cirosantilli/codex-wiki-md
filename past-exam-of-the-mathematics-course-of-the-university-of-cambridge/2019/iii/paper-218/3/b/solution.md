<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For player $i$, competition $c$, and rival $r$, the fitted [Poisson generalized linear mixed model](../../../../../../poisson-generalized-linear-mixed-model.md) is

$$
Y_{icr}\mid b_i\sim\operatorname{Poisson}(\mu_{icr}),
$$



$$
\log\mu_{icr}
=0.7287-0.8899\mathbf1_{\{c=B\}}
+1.4961\mathbf1_{\{c=C\}}
+0.4385\mathbf1_{\{r=S\}}+b_i,
\qquad b_i\sim N(0,0.1168).
$$

A negative-binomial model is commonly obtained by gamma mixing of a multiplicative Poisson mean and has negative-binomial marginals. Here the Gaussian random intercept gives a Poisson-lognormal mixture and correlates observations from the same player.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
