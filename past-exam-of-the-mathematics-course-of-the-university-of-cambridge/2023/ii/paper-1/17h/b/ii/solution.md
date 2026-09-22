<h1 id="17h/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $Y$ count unordered pairs of distinct $K_4$ copies that have a common vertex. Classifying such a pair by whether it shares one, two, or three vertices gives

$$
\mathbb EY
=O(n^7p^{12})+O(n^6p^{11})+O(n^5p^9)
=o(1).
$$

Indeed, after substituting $p=n^{-2/3}\log n$, these terms are respectively

$$
O(n^{-1}(\log n)^{12}),\qquad
O(n^{-4/3}(\log n)^{11}),\qquad
O(n^{-1}(\log n)^9).
$$

The [first moment method](../../../../../../../first-moment-method.md) gives $\mathbb P(Y>0)\leq\mathbb EY\to0$. Part (i) says that $X\geq100$ with probability tending to one, so the [union bound](../../../../../../../boole-s-inequality.md) shows that, with probability tending to one, both $X\geq100$ and $Y=0$. On that event any one hundred of the $K_4$ copies are pairwise vertex-disjoint, proving [vertex-disjoint sparse clique copies](../../../../../../../vertex-disjoint-sparse-clique-copies.md) in this case.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [17H](../../../17h.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
