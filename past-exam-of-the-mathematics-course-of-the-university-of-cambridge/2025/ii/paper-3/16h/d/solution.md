<h1 id="16h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

This is [König theorem for cardinal numbers](../../../../../../konig-s-theorem-set-theory.md). Since $\kappa_i<\lambda_i$, map $(i,\alpha)$ in the disjoint union to the element $s_{i,\alpha}$ of the product defined by

$$
s_{i,\alpha}(j)=
\begin{cases}
\alpha+1,&j=i,\\
0,&j\ne i.
\end{cases}
$$

Here $\alpha<\kappa_i$ implies $\alpha+1<\lambda_i$. The unique nonzero coordinate and its value recover $(i,\alpha)$, so this is an injection

$$
\bigsqcup_{i\in I}\kappa_i\longrightarrow
\prod_{i\in I}\lambda_i.
$$

For strictness, suppose $F$ mapped the disjoint union onto the product. For each $i$, the set

$$
A_i=\{F(i,\alpha)(i):\alpha<\kappa_i\}
$$

has cardinality at most $\kappa_i$, so it cannot exhaust $\lambda_i$. Choose $b_i\in\lambda_i\setminus A_i$. Then $b=(b_i)_{i\in I}$ differs from $F(i,\alpha)$ in coordinate $i$ for every $(i,\alpha)$, contradicting surjectivity. By [Cantor-Schröder-Bernstein theorem](../../../../../../cantor-schroder-bernstein-theorem.md), an injection in the reverse direction would combine with the displayed injection to give a bijection and hence a surjection. Therefore

$$
\boxed{\sum_{i\in I}\kappa_i<\prod_{i\in I}\lambda_i.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [16H](../../16h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
