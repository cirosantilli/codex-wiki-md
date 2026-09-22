<h1 id="14b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For distinct [interpolation nodes](../../../../../../interpolation-node.md) $x_0,\ldots,x_n$, let $p_n$ be the unique [polynomial](../../../../../../polynomial-split.md) of degree at most $n$ satisfying $p_n(x_i)=f(x_i)$. Existence follows from the [Lagrange polynomial](../../../../../../lagrange-polynomial.md) expression

$$
p_n(x)=\sum_{i=0}^nf(x_i)\prod_{j\ne i}\frac{x-x_j}{x_i-x_j};
$$

uniqueness follows because the difference of two interpolants has $n+1$ distinct zeros but degree at most $n$.

Define the [divided difference](../../../../../../divided-difference.md) $f[x_0,\ldots,x_n]$ to be the coefficient of $x^n$ in $p_n$, even when that coefficient is zero. For $n=0$ this gives $f[x_0]=f(x_0)$. Permuting the nodes does not change the interpolation conditions, so it does not change their unique interpolant or this coefficient. **The divided difference is symmetric in all the nodes.** Equivalently its symmetric expression is

$$
f[x_0,\ldots,x_n]=\sum_{i=0}^n\frac{f(x_i)}{\prod_{j\ne i}(x_i-x_j)}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
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
