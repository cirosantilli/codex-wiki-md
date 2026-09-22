<h1 id="16b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $A=D+L+U$, with $D$ diagonal, and use only old iterates on the right side. The [Jacobi method](../../../../../../jacobi-method.md) is

$$
\boxed{x_i^{k+1}=\frac1{a_{ii}}\left(b_i-\sum_{j\ne i}a_{ij}x_j^k\right),\qquad
x^{k+1}=-D^{-1}(L+U)x^k+D^{-1}b}.
$$

Strict row diagonal dominance ensures every $a_{ii}\ne0$. The exact solution satisfies the same coordinate relation. For $e^k=x^k-x^*$, subtraction gives

$$
|e_i^{k+1}|\le\frac{\sum_{j\ne i}|a_{ij}|}{|a_{ii}|}\|e^k\|_\infty
\le\gamma\|e^k\|_\infty.
$$

Taking the maximum and iterating proves

$$
\boxed{\|x^k-x^*\|_\infty\le\gamma^k\|x^0-x^*\|_\infty\longrightarrow0}.
$$

This direct contraction proof requires no eigenvector assumption and applies to every strictly diagonally dominant [matrix](../../../../../../matrix.md) with the stated uniform $\gamma<1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [16B](../../16b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
