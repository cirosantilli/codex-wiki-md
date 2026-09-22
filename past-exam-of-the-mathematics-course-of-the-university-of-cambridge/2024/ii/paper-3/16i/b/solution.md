<h1 id="16i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Godel completeness theorem](../../../../../../godel-s-completeness-theorem.md) says that a first-order sentence follows semantically from a theory exactly when it is formally derivable from it. The [compactness theorem](../../../../../../compactness-theorem.md) says that a theory has a model exactly when every finite subset has a model.

Fix $i$. For each $j\ne i$, the theory $T_i\cup T_j$ has no model because the model classes form a partition. By compactness, some finite $\Delta_{ij}\subseteq T_i$ is already inconsistent with $T_j$. Let

$$
\Delta_i=\bigcup_{j\ne i}\Delta_{ij},
$$

a finite subset of $T_i$. Every model of $T_i$ models $\Delta_i$. Conversely, a model of $\Delta_i$ belongs to exactly one class $T_j$; if $j\ne i$, it would model both $T_j$ and $\Delta_{ij}$, a contradiction. Hence it belongs to $T_i$, and $\Delta_i$ finitely axiomatizes $T_i$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [16I](../../16i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
