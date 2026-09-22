<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the shape-rate convention $R_k\sim\operatorname{Gamma}(\alpha_0,\beta_0)$. The factors involving $R_k$ in the [posterior density](../../../../../../../posterior-density.md) are

$$
R_k^{I_k}e^{-s_kR_k}R_k^{\alpha_0-1}e^{-\beta_0R_k}
=R_k^{I_k+\alpha_0-1}e^{-(s_k+\beta_0)R_k}.
$$

By [Poisson-gamma conjugacy](../../../../../../../poisson-gamma-conjugacy.md),

$$
R_k\mid I_k,s_k\sim\operatorname{Gamma}(I_k+\alpha_0,s_k+\beta_0),
$$

so its [posterior mean](../../../../../../../posterior-mean.md) is $(I_k+\alpha_0)/(s_k+\beta_0)$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
