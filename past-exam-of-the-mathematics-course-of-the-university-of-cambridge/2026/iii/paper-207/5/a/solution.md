<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Cox proportional-hazards model](../../../../../../cox-proportional-hazards-model.md) is

$$
h_i(t)=h_0(t)e^{\beta z_i},
$$

where $h_0$ is an unspecified baseline hazard and $z_i$ indicates treatment. With no tied events, the [Cox partial likelihood](../../../../../../cox-partial-likelihood.md) is

$$
L(\beta)=\prod_{i:\,v_i=1}
\frac{e^{\beta z_i}}{\sum_{j\in R(x_i)}e^{\beta z_j}}.
$$

Equality of the two hazard functions is $H_0:\beta=0$, testable with a likelihood-ratio, score, or Wald test from this likelihood.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
