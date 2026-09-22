<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply the [weak maximum principle for elliptic operators](../../../../../../weak-maximum-principle-for-elliptic-operators.md) to $q=|Dw|^2$. The [product rule](../../../../../../product-rule.md) and the equation for the [harmonic function](../../../../../../harmonic-function.md) give

$$
\Delta q=2\sum_{i,j}(D_{ij}w)^2+2\sum_iD_iw\,D_i\Delta w
=2|D^2w|^2\geq0.
$$

The function $q$ is twice differentiable inside and continuous on the closure, by the prescribed regularity. Hence $\sup_\Omega q\leq\sup_{\partial\Omega}q$. Conversely, each boundary value of $q$ is a limit of values at interior points, so the reverse inequality holds for the suprema. Taking square roots proves the [gradient maximum principle for harmonic functions](../../../../../../gradient-maximum-principle-for-harmonic-functions.md):

$$
\boxed{\sup_\Omega|Dw|=\sup_{\partial\Omega}|Dw|.}
$$

This argument controls the length of the entire [gradient](../../../../../../gradient.md), without comparing its separate components.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
