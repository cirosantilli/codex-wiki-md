<h1 id="13k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The reduced model `fit3` retains malignancy but omits both site indicators. The [analysis of deviance for nested generalized linear models](../../../../../../analysis-of-deviance-for-nested-generalized-linear-models.md) therefore tests

$$
H_0:\beta_B=\beta_C=0
$$

against the additive model with a site effect. The likelihood-ratio statistic is the reduction in deviance,

$$
7.4923-0.8505=6.6418.
$$

The full model adds two parameters, so under $H_0$ this is approximately $\chi^2_2$. Since

$$
6.6418>\chi^2_{2,0.95}=5.9915
$$

but is less than the $0.99$ quantile $9.2103$, the p-value is between $0.01$ and $0.05$; in fact, because $\chi^2_2$ has survival function $e^{-x/2}$,

$$
p=e^{-6.6418/2}\approx0.0361.
$$

We reject the no-site-effect null at the $5\%$ level and find evidence that survival differs by site after adjustment for malignancy.

## ↑ Ancestors (11)

1. [D](../d.md)
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
