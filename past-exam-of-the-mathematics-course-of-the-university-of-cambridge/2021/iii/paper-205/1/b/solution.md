<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The scalar [logistic loss](../../../../../../logistic-loss.md) $u\mapsto-u+\log(1+e^u)$ is strictly convex because its second derivative is $e^u/(1+e^u)^2>0$. If $\widehat\beta$ and $\widetilde\beta$ are minimizers but $X\widehat\beta\ne X\widetilde\beta$, strict convexity of the loss as a function of the fitted vector and convexity of the [L1 norm](../../../../../../l1-norm.md) make the objective at their midpoint strictly smaller than the common minimum. This contradiction proves that

$$
\boxed{X\widehat\beta=X\widetilde\beta}
$$

for every pair of solutions.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
