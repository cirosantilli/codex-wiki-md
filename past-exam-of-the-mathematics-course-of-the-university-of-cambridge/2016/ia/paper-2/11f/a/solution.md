<h1 id="11f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\mu=\mathbb E[X]$ and $A=\{X>\theta\mu\}$. The finite [second moment](../../../../../../second-moment.md) implies a finite first [moment](../../../../../../moment.md), and nonnegativity with $\mathbb E[X^2]>0$ implies $\mu>0$. On $A^c$, one has $0\leq X\leq\theta\mu$. Therefore

$$
\mathbb E[X\mathbf1_{A^c}]\leq\theta\mu\,\mathbb P(A^c)\leq\theta\mu.
$$

Subtract this from $\mathbb E[X]=\mu$ to obtain the [truncated first moment bound](../../../../../../truncated-first-moment-bound.md):

$$
\boxed{\mathbb E[X\mathbf1_A]\geq(1-\theta)\mathbb E[X].}
$$

The [indicator function](../../../../../../indicator-function.md) uses the strict event specified in the question; any mass at the threshold belongs to $A^c$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
