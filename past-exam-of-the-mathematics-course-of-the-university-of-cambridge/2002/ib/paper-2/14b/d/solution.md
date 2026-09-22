<h1 id="14b/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Continue with $D,D_i$ from part (c). Comparing omission of $x_i$ and $x_n$ gives

$$
D_i=D_n+(x_n-x_i)D.
$$

Comparing omission of $x_0$ and $x_n$ gives $D_0=D_n+(x_n-x_0)D$. Eliminating $D$ proves

$$
\boxed{D_i=\gamma D_n+(1-\gamma)D_0,\qquad \gamma=\frac{x_i-x_0}{x_n-x_0}}.
$$

Here $D_n=f[x_0,\ldots,x_{n-1}]$ and $D_0=f[x_1,\ldots,x_n]$, so this is exactly the required [omitted-node identities for divided differences](../../../../../../omitted-node-identities-for-divided-differences.md). The original nodes need not be ordered, and the formula remains valid even if $\gamma$ lies outside $[0,1]$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [14B](../../14b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
