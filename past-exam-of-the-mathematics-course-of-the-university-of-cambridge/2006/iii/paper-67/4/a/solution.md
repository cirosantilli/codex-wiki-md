<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For real-valued $f\in C[-1,1]$, there is a unique [best uniform approximation](../../../../../../best-uniform-approximation.md) $p_*\in\mathcal P_n$, where $\mathcal P_n$ means degree at most $n$. If $E=\|f-p_*\|_\infty>0$, the [Chebyshev alternation theorem](../../../../../../equioscillation-theorem.md) characterizes it by the existence of $n+2$ ordered points

$$
-1\leq x_0<x_1<\cdots<x_{n+1}\leq1
$$

and a sign $\varepsilon\in\{-1,1\}$ such that

$$
\boxed{f(x_j)-p_*(x_j)=\varepsilon(-1)^jE,\qquad j=0,\ldots,n+1.}
$$

Conversely, a [polynomial](../../../../../../polynomial-split.md) in $\mathcal P_n$ whose error has this alternation is the best one. If the best error is zero, $f$ itself is the exact [polynomial](../../../../../../polynomial-split.md) approximant. The real-valued qualification matters: this sign-alternation formulation is not the corresponding criterion for arbitrary complex-valued approximation.

The obstruction to a strict improvement is concrete. If $q$ had smaller error at every alternation point, $q-p_*$ would have alternating strict signs there. The intermediate value theorem would give at least $n+1$ distinct zeros, impossible for a nonzero [polynomial](../../../../../../polynomial-split.md) of degree at most $n$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
