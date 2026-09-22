<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Since $U\subset\mathbb R^3$ is bounded and smooth, the [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) gives continuous embeddings $H^1(U)\hookrightarrow L^4(U)$ and $H^1(U)\hookrightarrow L^6(U)$. Because $|\sin s|\leq1$,

$$
\|w(t)^2\sin w(t)\|_{L^2(U)}
\leq\|w(t)\|_{L^4(U)}^2
\leq C\|w(t)\|_{H^1(U)}^2.
$$

Taking the $L^2$ norm in time gives

$$
\boxed{\|w^2\sin w\|_{L^2(U_T)}
\leq\beta T^{1/2}\|w\|_{L_t^\infty H_x^1}^2}.
$$

For $F(s)=s^2\sin s$, the [mean value theorem](../../../../../../mean-value-theorem.md) and $|F'(s)|\leq2|s|+s^2$ imply

$$
|F(r)-F(s)|
\leq C|r-s|\bigl(|r|+|s|+|r|^2+|s|^2\bigr).
$$

Apply the [Generalized Holder inequality](../../../../../../generalized-holder-inequality.md) in space, using $L^4$ for the quadratic products and $L^6\cdot L^3$ for the cubic products, and then use the two Sobolev embeddings. Pointwise in time this yields

$$
\|F(w)-F(\widetilde w)\|_2
\leq C\|w-\widetilde w\|_{H^1}
\left(\|w\|_{H^1}+\|w\|_{H^1}^2
+\|\widetilde w\|_{H^1}+\|\widetilde w\|_{H^1}^2\right).
$$

Taking the $L^2$ norm in time proves the required estimate with the factor $\gamma T^{1/2}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
