<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $X_1,\ldots,X_N$ be independent with laws $p_1,\ldots,p_N$. We prove the claim by induction. Split the [law of total variance](../../../../../../law-of-total-variance.md) at the last coordinate:

$$
\operatorname{Var}(f(X))
=\mathbb E\!\left[\operatorname{Var}(f(X)\mid X_1,\ldots,X_{N-1})\right]
+\operatorname{Var}\!\left(\mathbb E[f(X)\mid X_1,\ldots,X_{N-1}]\right).
$$

The first term is at most $c_N^2\mathbb E|\partial_Nf(X)|^2$. Apply the induction hypothesis to $g(x_1,\ldots,x_{N-1})=\mathbb E_{X_N}f(x_1,\ldots,x_{N-1},X_N)$. Differentiation under the expectation and [Jensen inequality](../../../../../../jensen-s-inequality.md) give

$$
|\partial_i g|^2
=|\mathbb E_{X_N}\partial_i f|^2
\leq\mathbb E_{X_N}|\partial_i f|^2.
$$

Writing $c=\max_i c_i$ and combining the terms yields

$$
\operatorname{Var}(f(X))
\leq c^2\mathbb E\sum_{i=1}^N|\partial_i f(X)|^2
=c^2\mathbb E\lVert\nabla f(X)\rVert^2.
$$

This is the [Tensorization of a Poincaré inequality](../../../../../../tensorization-of-a-poincare-inequality.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
