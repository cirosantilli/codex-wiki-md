<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For

$$
J(x)=\frac12\lVert Ax-y\rVert^2,
$$

the [Fréchet derivative](../../../../../../frechet-derivative.md) in direction $h$ is

$$
J'(x)h
=\operatorname{Re}
\langle Ax-y,Ah\rangle_Y
=\operatorname{Re}
\langle A^*(Ax-y),h\rangle_X.
$$

Thus the Hilbert-space [gradient](../../../../../../gradient.md) is

$$
\boxed{\nabla J(x)=A^*(Ax-y)}.
$$

The [gradient descent](../../../../../../gradient-descent.md) update with step size $\gamma$ is consequently

$$
x_{n+1}=x_n-\gamma\nabla J(x_n)
=x_n+\gamma A^*(y-Ax_n),
$$

which is exactly [Landweber iteration](../../../../../../landweber-iteration.md). Its stationary points solve the normal equation and minimize the convex quadratic functional $J$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
