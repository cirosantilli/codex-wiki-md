<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose the uniform distribution on shortest paths equivariantly under graph automorphisms. Automorphisms preserve distances and send uniform shortest paths to uniform shortest paths, so vertex transitivity makes

$$
\widetilde f(x)=\sum_{y\sim x}f(x,y)
$$

constant in $x$. Summing this constant over vertices counts each path-edge incidence at most twice:

$$
n\widetilde f(x)
=\sum_x\widetilde f(x)
\leq2\sum_{u,v\in V}\mathbb E_{\nu_{uv}}|\Gamma_{uv}|
\leq2n^2\Delta.
$$

Thus $\widetilde f(x)\leq2n\Delta$, and each nonnegative summand satisfies

$$
\boxed{f(e)\leq2n\Delta}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 215](../../../../paper-215-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
