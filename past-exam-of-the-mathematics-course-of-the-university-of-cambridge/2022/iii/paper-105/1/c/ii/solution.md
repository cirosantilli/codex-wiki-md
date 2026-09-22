<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Choose $h_j\to0$. The assumed bound and the [weak subsequence of a bounded Hilbert-space sequence](../../../../../../../weak-subsequence-of-a-bounded-hilbert-space-sequence.md) result give a subsequence for which

$$
\Delta_i^{h_j}u\rightharpoonup g_i
\quad\hbox{weakly in }L^2(V),
\qquad
\lVert g_i\rVert_2\leq C.
$$

For every [test function](../../../../../../../test-function.md) $\varphi\in C_c^\infty(V)$, a change of variables yields the difference-quotient integration-by-parts identity

$$
\int_V(\Delta_i^{h_j}u)\varphi
=-\int_Vu\,\Delta_i^{-h_j}\varphi.
$$

The right side converges to $-\int_VuD_i\varphi$, while the left side converges to $\int_Vg_i\varphi$. Thus $g_i$ is the $i$th [weak derivative](../../../../../../../weak-derivative.md) of $u$. This holds for every $i$, so

$$
\boxed{u\in H^1(V),\qquad
\lVert D_i u\rVert_{L^2(V)}\leq C.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
