<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**Yes.** Write $D_S=D(Q_{X_S}\Vert P_{X_S})$ and $D=D_{\{1,\ldots,n\}}$. The bounds from b and d are respectively

$$
B_{\mathrm{old}}=nD-\sum_iD_{X^{(i)}},
\qquad
B_{\mathrm{new}}=\frac{nD-\sum_iD_{\{i\}}}{n-1}.
$$

The [Strong form of Han's entropy inequality](../../../../../../strong-form-of-han-s-entropy-inequality.md), obtained by repeated [entropy submodularity](../../../../../../entropy-submodularity.md), states

$$
(n-1)\sum_iH(X^{(i)})
\geq n(n-2)H(X_{1:n})+\sum_iH(X_i).
$$

After replacing entropies by divergences from the product reference, whose cross-entropy terms cancel, this is exactly $B_{\mathrm{new}}\leq B_{\mathrm{old}}$. Equality holds for product $Q$ and when $n=2$; dependence can make the new bound strictly smaller.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
