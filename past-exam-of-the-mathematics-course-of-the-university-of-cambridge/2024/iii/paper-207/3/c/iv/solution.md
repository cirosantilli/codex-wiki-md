<h1 id="3/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

A [Dirichlet process mixture model](../../../../../../../dirichlet-process-mixture-model.md) avoids fixing the number of occupied functions. Let $G_0=N_n(0,K)$ be the finite-dimensional [Gaussian process](../../../../../../../gaussian-process.md) law on the common input grid and specify

$$
G\sim\operatorname{DP}(\alpha,G_0),
\qquad
f_i\mid G\overset{\mathrm{iid}}\sim G,
\qquad
y_i\mid f_i\sim N_n(f_i,\sigma^2I_n).
$$

A draw from a [Dirichlet process](../../../../../../../dirichlet-process.md) is almost surely discrete, so several $f_i$ coincide and thereby form clusters. The number of occupied clusters is random and can grow with the data.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
