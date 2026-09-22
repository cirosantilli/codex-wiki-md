<h1 id="18j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $L_i=K(\alpha_1,\ldots,\alpha_i)$, with $L_0=K$, and let

$$
d_i=[L_i:L_{i-1}].
$$

Fix a $K$-embedding $\sigma:L_{i-1}\to\overline K$. If $m_i(t)$ is the minimal polynomial of $\alpha_i$ over $L_{i-1}$, an extension of $\sigma$ to $L_i$ is determined by the image of $\alpha_i$, which must be a root of the polynomial obtained by applying $\sigma$ to the coefficients of $m_i$. Conversely, each distinct root gives one extension. Since $\overline K$ is algebraically closed, there is at least one such root, and there are at most $d_i$ distinct roots.

Starting from the unique embedding of $K$, induction therefore gives

$$
1\leq |\operatorname{Hom}_K(L_i,\overline K)|
\leq d_1\cdots d_i=[L_i:K].
$$

If $L/K$ is separable, each $m_i$ is separable, so every transformed polynomial has exactly $d_i$ distinct roots. Every inequality is then an equality. Taking $i=n$ proves

$$
1\leq |\operatorname{Hom}_K(L,\overline K)|\leq[L:K],
$$

with equality in the separable case.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18J](../../18j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
