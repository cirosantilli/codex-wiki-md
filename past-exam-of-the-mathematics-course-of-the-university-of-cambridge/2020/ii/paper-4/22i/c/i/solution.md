<h1 id="22i/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Set $y_k(0)=x_0$ and let $M=\sup_{z\in\mathbb R^n}\lVert F(z)\rVert<\infty$. On the first interval, $y_k$ is the known constant $x_0$, so the [integral equation](../../../../../../../integral-equation.md) defines $x_k$. Its endpoint value then defines the constant $y_k$ on the next interval, and induction over the $k$ subintervals defines the pair on all of $[0,1]$. An integral of the bounded, piecewise constant function $F\circ y_k$ is [continuous](../../../../../../../continuous-function.md), so every $x_k$ is continuous. In fact,

$$
\lVert x_k(t)-x_k(s)\rVert\leq M|t-s|,
$$

so the approximations are uniformly [Lipschitz continuous](../../../../../../../lipschitz-continuity.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [22I](../../../22i.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
