<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $p_k=\mathbb P(X=k)$. Monotonicity gives

$$
1\geq\sum_{j=1}^kp_j\geq kp_k,
$$

so $p_k\leq1/k$ and therefore $\log_2k\leq\log_2(1/p_k)$ whenever $p_k>0$. Hence

$$
\boxed{\mathbb E[\log_2X]
=\sum_{k\geq1}p_k\log_2k
\leq\sum_{k\geq1}p_k\log_2\frac1{p_k}
=H(X)<\infty.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
