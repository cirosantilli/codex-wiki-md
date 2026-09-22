<h1 id="5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Set $X=Du/\sqrt{1+|Du|^2}$. Since $u\in C^2(\mathbb R^n)$, the field is $C^1$, and $|X|\leq1$ everywhere, even when the [gradient](../../../../../../gradient.md) of $u$ is unbounded. The [divergence theorem](../../../../../../divergence-theorem.md) on $B_R(0)$ gives

$$
\kappa|B_R|=\int_{\partial B_R}X\cdot\nu\,dS,\qquad |\kappa|\leq\frac{|\partial B_R|}{|B_R|}=\frac nR.
$$

Letting $R\to\infty$ proves $\kappa=0$. This is the fact that [an entire bounded vector field cannot have nonzero constant divergence](../../../../../../an-entire-bounded-vector-field-cannot-have-nonzero-constant-divergence.md); it holds in every dimension.

The equation is now exactly the [minimal surface equation for a graph](../../../../../../minimal-surface-equation-for-a-graph.md). Apply the supplied [Bernstein theorem for minimal graphs](../../../../../../bernstein-theorem-for-minimal-graphs.md) in dimensions $1\leq n\leq7$ to conclude

$$
\boxed{\kappa=0,\qquad u(x)=a\cdot x+b\quad(a\in\mathbb R^n,\ b\in\mathbb R).}
$$

Thus no nonzero constant right-hand side is possible for an entire graph, and in the stated dimensions every possible graph is an affine plane.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
