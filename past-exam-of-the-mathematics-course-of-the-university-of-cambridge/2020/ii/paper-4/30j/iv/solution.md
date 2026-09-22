<h1 id="30j/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

With varying positive step sizes, the same one-step inequality is

$$
2\eta_s\,\mathbb E[f(\beta_s)-f(\widehat\beta)]
\leq\mathbb E\lVert\beta_s-\widehat\beta\rVert_2^2
-\mathbb E\lVert\beta_{s+1}-\widehat\beta\rVert_2^2
+\eta_s^2\frac{M^2}{\{\log2\}^2}.
$$

Sum from $s=1$ to $k$, use $\lVert\beta_1-\widehat\beta\rVert_2\leq2R$, and divide by $2A_1$. The [Jensen inequality](../../../../../../jensen-s-inequality.md) for the weighted average $\widetilde\beta=A_1^{-1}\sum_s\eta_s\beta_s$ gives

$$
\boxed{
\mathbb E f(\widetilde\beta)-f(\widehat\beta)
\leq\frac{A_2M^2}{2A_1\{\log(2)\}^2}+\frac{2R^2}{A_1}},
$$

where $A_1=\sum_s\eta_s$ and $A_2=\sum_s\eta_s^2$.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [30J](../../30j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
