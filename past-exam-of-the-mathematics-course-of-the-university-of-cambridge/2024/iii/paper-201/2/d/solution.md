<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $g:M'\to\mathbb R$ be bounded and continuous. The composition $h=g\circ f$ is bounded and measurable, and every discontinuity point of $h$ is a discontinuity point of $f$. Thus

$$
\mathbb P(X\in D_h)\leq\mathbb P(X\in D_f)=0.
$$

The [Portmanteau theorem](../../../../../../portmanteau-theorem.md) includes the null-discontinuity criterion: if $X_n\xrightarrow dX$ and a bounded measurable function is continuous at $X$ almost surely, then its expectations converge. Hence

$$
\mathbb E[g(f(X_n))]\longrightarrow\mathbb E[g(f(X))].
$$

Since this holds for every bounded continuous $g$, it proves the [continuous mapping theorem](../../../../../../continuous-mapping-theorem.md) conclusion $f(X_n)\xrightarrow d f(X)$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
