<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Apply [coordinate compression in a product of paths](../../../../../../coordinate-compression-in-a-product-of-paths.md) in both coordinates. Replacing every fiber by an initial interval preserves the number of edges inside that fiber; between two neighboring fibers, the compressed sets span the minimum of their sizes, at least their original intersection size. Repeating the operation therefore never decreases the number of edges spanned and eventually produces a down-set.

Write the nonzero row lengths of this down-set as

$$
a_1\geq a_2\geq\cdots\geq a_q>0,
\qquad \sum_{i=1}^q a_i=t^2.
$$

The horizontal edges number $t^2-q$, and the vertical edges number

$$
\sum_{i=2}^q a_i=t^2-a_1.
$$

Consequently

$$
e(\mathcal A)\leq2t^2-(q+a_1).
$$

Since $t^2\leq qa_1$, the [arithmetic-geometric mean inequality](../../../../../../arithmetic-geometric-mean-inequality.md) gives $q+a_1\geq2t$. Hence

$$
e(\mathcal A)\leq2t^2-2t=2t(t-1)=e([t]^2),
$$

as required.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
