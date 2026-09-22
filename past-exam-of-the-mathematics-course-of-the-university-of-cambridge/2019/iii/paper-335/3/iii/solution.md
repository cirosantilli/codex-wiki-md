<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Minimize the data-misfit functional $J(x)=\tfrac12\|Ax-y\|^2$. For a perturbation $h$, $DJ(x)[h]=\operatorname{Re}\langle A^*(Ax-y),h\rangle$, so its [gradient](../../../../../../gradient.md) is $A^*(Ax-y)$. [Gradient descent](../../../../../../gradient-descent.md) gives [Landweber iteration](../../../../../../landweber-iteration.md):

$$
\boxed{x_{n+1}=x_n+\tau A^*(y-Ax_n),\qquad x_0=0,\qquad 0<\tau<\frac2{\|A\|^2}.}
$$

On a singular component, the iteration error is multiplied by $1-\tau\sigma_j^2$, whose modulus is less than one. Starting from zero preserves orthogonality to $\ker A$ and makes the exact-data iterates converge to $x^\dagger$.

For the unit-step formulas and noise bound used below, rescale so that $\tau=1$ and $\|A\|\leq1$. Finite iteration count bounds amplification of small singular-value components; the stopping count provides the regularization parameter.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
