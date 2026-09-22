<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We prove the [reverse-inclusion well-quasi-ordering of monomial ideals](../../../../../../reverse-inclusion-well-quasi-ordering-of-monomial-ideals.md), equivalently of all upward-closed subsets of $\mathbb N^r$, by induction on $r$. For $r=1$ the sets are tails $[a,\infty)$ and the empty set; reverse inclusion orders their endpoints as $0<1<\cdots<\infty$, a [well-order](../../../../../../well-order.md). The case $r=0$, if needed for the induction, is just a finite family.

For an upset $U\subseteq\mathbb N^{r+1}$, let $U_k=\{\alpha:(\alpha,k)\in U\}$. These are upsets of $\mathbb N^r$ and satisfy $U_0\subseteq U_1\subseteq\cdots$. They stabilize. Indeed the union $U_\infty$ has a finite minimal basis by [Dickson's lemma](../../../../../../dickson-s-lemma.md): an infinite set of minimal elements would be an [antichain](../../../../../../antichain.md) in the componentwise [well-quasi-ordering](../../../../../../well-quasi-ordering.md) of $\mathbb N^r$. Each basis element appears in some slice, and after the largest of these finitely many indices the slice contains the entire upset $U_\infty$.

Choose a stabilization index $m$, and encode $U$ by the finite [word](../../../../../../string.md) $(U_0,\ldots,U_{m-1})$ and the final slice $U_\infty$. The induction hypothesis makes slices a [well-quasi-ordering](../../../../../../well-quasi-ordering.md) by reverse inclusion. [Higman's lemma](../../../../../../higman-s-lemma.md), proved in Question 3 below, makes their finite [words](../../../../../../string.md) a [well-quasi-ordering](../../../../../../well-quasi-ordering.md); [finite product closure of well-quasi-orderings](../../../../../../finite-product-closure-of-well-quasi-orderings.md) also compares the final slices. Thus in every infinite sequence of upsets there are earlier $U$ and later $V$ with a strictly increasing matching $h$ of the earlier pre-stabilization slices into the later ones, such that

$$
U_k\supseteq V_{h(k)}\quad(k<m_U),\qquad U_\infty\supseteq V_\infty.
$$

Since $h(k)\ge k$ and the $V$-slices increase, $U_k\supseteq V_{h(k)}\supseteq V_k$ for $k<m_U$. For $k\ge m_U$, $U_k=U_\infty\supseteq V_\infty\supseteq V_k$. Therefore $U\supseteq V$, completing the induction.

Now choose one finite support $A_n$ for each term of an arbitrary infinite [sequence](../../../../../../sequence.md) $(f_n)$ in the finitely generated [incline](../../../../../../incline.md). The result supplies $i<j$ with $U_{A_i}\supseteq U_{A_j}$, and the preceding absorption calculation gives $f_i\preceq f_j$. Hence **every finitely generated incline is well-quasi-ordered by the specified reverse absorption order**. The proof allows all additional algebraic identifications among the generators.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
