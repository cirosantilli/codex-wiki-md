<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define the piecewise-linear function

$$
h(s)=g(0)+g'(0)s+
\sum_{i=1}^N\bigl(g'(K_i)-g'(K_{i-1})\bigr)(s-K_i)^+.
$$

On $[K_j,K_{j+1})$, its slope is $g'(K_j)$. Since $g$ is [convex](../../../../../../convex-function.md), $g'$ is nondecreasing and hence $h'(s)\leq g'(s)$ wherever the derivatives exist. As $h(0)=g(0)$, integration gives $h(s)\leq g(s)$ for every $s\geq0$.

Positive no-arbitrage pricing, the forward identity $\mathbb E_{Q^T}[S_T\mid\mathcal F_t]=F_t^T$, and the call-price formula now give

$$
\boxed{\pi_t\geq B_t^T\bigl(g(0)+g'(0)F_t^T\bigr)
\bigl(g'(K_i)-g'(K_{i-1})\bigr)C_t^{T,K_i}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
