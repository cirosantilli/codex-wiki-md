<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Part b places $\delta=\widehat\beta-\beta^0$ in the [Lasso cone condition](../../../../../../lasso-cone-condition.md). Keeping the prediction-error term in the same argument gives

$$
\frac1n\lVert X\delta\rVert_2^2
\leq\frac{3\lambda}{2}\lVert\delta_S\rVert_1
\leq\frac{3\lambda\sqrt{|S|}}2\lVert\delta\rVert_2,
$$

where the second step is the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). The [restricted eigenvalue condition](../../../../../../restricted-eigenvalue-condition.md) gives

$$
\frac1n\lVert X\delta\rVert_2^2>\gamma\lVert\delta\rVert_2^2
$$

for nonzero $\delta$ in this cone. Division by $\lVert\delta\rVert_2$ proves

$$
\lVert\widehat\beta-\beta^0\rVert_2
\leq\frac{3\lambda\sqrt{|S|}}{2\gamma}.
$$

The result is immediate when $\delta=0$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
