<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [generalized linear mixed model](../../../../../../generalized-linear-mixed-model.md) tries to explain overdispersion by replacing the fixed minority coefficient with a Gaussian [random intercept](../../../../../../random-intercept.md). Conditional on the group effect $b_m$,

$$
Y_i\sim\operatorname{Poisson}(\mu_i),
\qquad
\log\mu_i=\beta_0+\beta_1g_i+b_{m_i},
\qquad b_0,b_1\sim N(0,\tau^2).
$$

This is a poor use of a random effect because minority has only two levels. Two realized intercepts contain almost no information about a random-effects distribution or its variance, and the two levels are substantively fixed categories rather than a sample from a population of groups. The model also has worse [Akaike information criterion](../../../../../../akaike-information-criterion.md) than model 1, $1132.8>1122.3$, and its fit does not establish that the original overdispersion has disappeared.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
