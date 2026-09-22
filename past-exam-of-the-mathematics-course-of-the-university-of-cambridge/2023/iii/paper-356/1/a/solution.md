<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The backward generator of the drift--diffusion is $\mathcal L=\alpha\partial_y+D\partial_y^2$. The [survival probability](../../../../../../survival-probability.md) satisfies the [Kolmogorov backward equation](../../../../../../kolmogorov-backward-equation.md)

$$
\boxed{\partial_tQ=D\partial_y^2Q+\alpha\partial_yQ,
\qquad 0<y<L,}
$$

with

$$
\boxed{Q(0,t)=0,
\qquad \partial_yQ(L,t)=0,
\qquad Q(y,0)=1.}
$$

The target is absorbing, while reflection gives the Neumann boundary condition at $L$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
