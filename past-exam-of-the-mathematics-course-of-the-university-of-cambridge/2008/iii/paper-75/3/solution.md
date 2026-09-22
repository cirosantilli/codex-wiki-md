<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a real [continuous function](../../../../../continuous-function.md) on $[-1,1]$, the [Chebyshev alternation theorem](../../../../../equioscillation-theorem.md) gives a unique [best uniform approximation](../../../../../best-uniform-approximation.md) $p_n^*$ from the space of [polynomials](../../../../../polynomial-split.md) of degree at most $n$. If $f$ is not already in that space, a candidate $p$ is best if and only if there exist ordered points $x_0<\cdots<x_{n+1}$ and a sign $\sigma\in\{1,-1\}$ with

$$
 f(x_j)-p(x_j)=\sigma(-1)^j\|f-p\|_\infty,
 \qquad 0\le j\le n+1.
$$

Thus a nonzero best error has **at least $n+2$ alternating extrema of equal magnitude**. If $f$ is already a [polynomial](../../../../../polynomial-split.md) of degree at most $n$, the unique best approximant is $f$ itself with zero error.

Existence does not require assuming that the infimum is attained: a minimizing sequence has uniformly bounded [polynomial](../../../../../polynomial-split.md) [norms](../../../../../norm.md), and evaluation at $n+1$ fixed distinct nodes bounds its coefficients through an invertible interpolation [matrix](../../../../../matrix.md). A convergent coefficient subsequence then attains the infimum. The alternation criterion characterizes that minimum and gives uniqueness. In the following parts, $n\ge1$ whenever $E_{n-1}$ occurs.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 75](../../paper-75-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
