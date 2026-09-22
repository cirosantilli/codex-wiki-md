<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Time is exposure: doubling the public duration should double the expected count without changing the viewing rate. Modeling the rate is therefore preferable to treating time as an additive linear predictor. In a [Poisson regression](../../../../../../poisson-regression.md) the exact implementation should be

$$
\log\mathbb E(N_i)=\log t_i+\beta_0+\beta_1I_i,
$$

using $\log t_i$ as an offset; directly supplying noninteger $N_i/t_i$ without exposure weights is not generally likelihood-equivalent.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
