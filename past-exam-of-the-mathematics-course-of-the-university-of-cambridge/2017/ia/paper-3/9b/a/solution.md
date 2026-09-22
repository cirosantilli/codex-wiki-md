<h1 id="9b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $B$ is [continuously differentiable](../../../../../../continuously-differentiable-function.md). Apply the [chain rule](../../../../../../chain-rule.md) to each component with $z_j=tx_j$:

$$
\partial_{x_j}F_i=t\partial_{z_j}B_i(tx),\qquad
\partial_tF_i=x_j\partial_{z_j}B_i(tx).
$$

Contracting the first identity with $x_j$ proves

$$
\boxed{(x\cdot\nabla)F=t\,\partial_tF.}
$$

Here $\nabla$ differentiates with respect to $x$ at fixed $t$, while the [time derivative](../../../../../../time-derivative.md) holds $x$ fixed. The equality follows directly even at $t=0$; no division by $t$ is needed. It holds componentwise for the [vector field](../../../../../../vector-field.md), so it is not restricted to [scalar](../../../../../../scalar.md) functions.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9B](../../9b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
