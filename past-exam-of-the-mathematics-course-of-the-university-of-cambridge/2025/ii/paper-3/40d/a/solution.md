<h1 id="40d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Consider a general constant-coefficient linear difference scheme

$$
\sum_{r,j}a_{rj}u_{m+j}^{n+r}=0.
$$

A spatial Fourier mode has the form

$$
u_m^n=\widehat u^{,n}e^{im\theta}.
$$

If one time step multiplies its amplitude by $G$, then $\widehat u^{,n+r}=G^r\widehat u^{,n}$, and substitution gives the [amplification polynomial of a multilevel finite difference scheme](../../../../../../amplification-polynomial-of-a-multilevel-finite-difference-scheme.md)

$$
\boxed{\sum_{r,j}a_{rj}G^r e^{ij\theta}=0}.
$$

For a one-step method this equation directly determines

$$
G(\theta)=\frac{\widehat u^{,n+1}}{\widehat u^{,n}}.
$$

By Parseval's identity, [von Neumann stability analysis](../../../../../../von-neumann-stability-analysis.md) gives $2$-norm stability when $|G(\theta)|\leq1$ for every Fourier mode. For a multilevel method, every root must obey the corresponding root condition.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40D](../../40d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
