<h1 id="23h/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose a minimizing sequence $(u_n)$ with

$$
\lVert u_n\rVert_2=1,
\qquad
E(u_n)\longrightarrow\lambda.
$$

Since

$$
E(u_n)\geq\lVert Du_n\rVert_2^2-\lVert V\rVert_\infty,
$$

the sequence is bounded in $H_0^1(\Omega)$. Passing to a subsequence, weak compactness gives

$$
u_n\rightharpoonup w
$$

in $H_0^1(\Omega)$. Rellich compactness gives $u_n\to w$ strongly in $L^2$, and hence

$$
\lVert w\rVert_2=1.
$$

Part (i) now yields

$$
E(w)\leq\liminf_nE(u_n)=\lambda.
$$

The definition of $\lambda$ gives the reverse inequality because $w$ is admissible. Therefore

$$
\boxed{E(w)=\lambda,\qquad\lVert w\rVert_2=1}.
$$

This is the [constrained ground-state minimizer on a bounded domain](../../../../../../../constrained-ground-state-minimizer-on-a-bounded-domain.md) obtained by the direct method.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [23H](../../../23h.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
