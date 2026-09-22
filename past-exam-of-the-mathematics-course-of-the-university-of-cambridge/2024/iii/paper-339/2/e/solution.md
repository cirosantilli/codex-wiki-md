<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Set

$$
g(x)=\frac12\lVert Ax-b\rVert_2^2,
\qquad
\nabla g(x)=A^T(Ax-b).
$$

The gradient has [Lipschitz continuity](../../../../../../lipschitz-continuity.md) with constant

$$
L=\lVert A^TA\rVert_2=\lVert A\rVert_2^2,
$$

where the norm is the [spectral norm](../../../../../../matrix-2-norm.md). The [proximal gradient method](../../../../../../proximal-gradient-method.md) is therefore

$$
z_r=x_r-\alpha A^T(Ax_r-b),
\qquad
x_{r+1}=\operatorname{prox}_{\alpha\lambda h}(z_r).
$$

For $\lambda>0$, part d makes the second step explicit:

$$
x_{r+1}=z_r-\alpha\lambda
P_C\left(\frac{z_r}{\alpha\lambda}\right),
$$

where $C$ is the [capped simplex](../../../../../../capped-simplex.md); when $\lambda=0$, this proximal step is the identity.

A standard fixed choice is $0<\alpha\leq1/L$; the wider interval $0<\alpha<2/L$ also gives convergence under the usual forward-backward conditions. For a general convex objective, the function-value error is $O(1/r)$. If $A$ has full column rank, the quadratic term is [strongly convex](../../../../../../strongly-convex-function.md) and an appropriate fixed step gives a linear convergence rate.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
