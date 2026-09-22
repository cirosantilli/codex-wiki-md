<h1 id="18c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Define the [cardinal polynomials](../../../../../../lagrange-polynomial.md)

$$
\ell_k(x)=\prod_{\substack{0\le j\le n\\j\ne k}}
\frac{x-x_j}{x_k-x_j}.
$$

They satisfy $\ell_k(x_i)=\delta_{ik}$. Hence evaluating the proposed [polynomial interpolation](../../../../../../polynomial-interpolation.md) formula at $x_i$ gives $p_n(x_i)=a_i$, so the required coefficients are

$$
\boxed{a_k=f_k}.
$$

The polynomial $\sum_kf_k\ell_k$ has degree at most $n$ and takes every prescribed value. Its uniqueness follows because the difference of two such polynomials would have $n+1$ distinct roots while having degree at most $n$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18C](../../18c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
