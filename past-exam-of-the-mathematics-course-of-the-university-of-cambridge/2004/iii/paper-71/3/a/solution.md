<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a real continuous $2\pi$-periodic function $f$, the [trigonometric Chebyshev alternation theorem](../../../../../../trigonometric-chebyshev-alternation-theorem.md) says that $t^*\in\mathcal T_n$ is its [best uniform approximation](../../../../../../best-uniform-approximation.md) if and only if there are $2n+2$ distinct cyclically ordered points in one period,

$$
x_0<x_1<\cdots<x_{2n+1}<x_0+2\pi,
$$

and a sign $\varepsilon\in\{1,-1\}$ such that

$$
\boxed{f(x_j)-t^*(x_j)=\varepsilon(-1)^j\|f-t^*\|_\infty
\quad(0\le j\le2n+1).}
$$

The best approximant exists and is unique. Alternation is cyclic: the last and first displayed extrema also have opposite signs across the closing interval. If the error is zero, $f=t^*$ and the characterization holds trivially.

The sufficiency can be seen from zero counting. A strictly improving [trigonometric polynomial](../../../../../../trigonometric-polynomial.md) would have a difference from $t^*$ with the alternating nonzero signs at these points, forcing at least $2n+2$ zeros on the circle. A nonzero member of $\mathcal T_n$ has at most $2n$ zeros: multiplying its Laurent expression by $e^{inx}$ gives an ordinary [polynomial](../../../../../../polynomial-split.md) of degree at most $2n$ in $e^{ix}$. This contradiction is the alternation mechanism used in the next part.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
