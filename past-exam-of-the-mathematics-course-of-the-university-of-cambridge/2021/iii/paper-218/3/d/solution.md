<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fit the exposure-offset Poisson model

$$
N_i\sim\operatorname{Poisson}\{t_i\exp(\beta_0+\beta_1I_i+\gamma_{g_i})\}.
$$

For a new video with investment $I$ and genre $g$, put $\mu=90\exp(\beta_0+\beta_1I+\gamma_g)$, compute

$$
\mathbb P_\mu(N\leq9999),\quad
\mathbb P_\mu(10000\leq N\leq49999),\quad
\mathbb P_\mu(N\geq50000),
$$

and select the largest. For fixed genre these probabilities are nonlinear functions of investment, so this is a nonlinear classifier.

## ↑ Ancestors (11)

1. [D](../d.md)
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
