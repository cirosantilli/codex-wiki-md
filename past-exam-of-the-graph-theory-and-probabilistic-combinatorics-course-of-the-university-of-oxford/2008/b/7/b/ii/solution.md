<h1 id="b/7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $t=\sqrt{2k\log_e(6kr)}$ and define $A_j=\{|Y_j|\ge t\}$. The preceding estimate gives $\mathbb P(A_j)\le1/(3kr)$. An event depends only on the $k$ signs in that row. Each such column occurs in at most $r-1$ other rows, so its dependency degree is at most $d=k(r-1)$. Events on disjoint sets of signs are independent even jointly, giving the required dependency [graph](../../../../../../graph-split.md).

For positive $k,r$,

$$
e\frac{d+1}{3kr}=\frac{e\{k(r-1)+1\}}{3kr}\le\frac e3<1.
$$

The symmetric [Lovász local lemma](../../../../../../lovasz-local-lemma.md) therefore gives positive probability that no $A_j$ occurs. Such a sign vector satisfies

$$
\boxed{\max_j|(Mx)_j|<\sqrt{2k\log_e(6kr)}}.
$$

The positive-parameter assumption is implicit in the printed square-root expression. If all rows are zero, all row sums vanish and no probabilistic construction is needed.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [B](../../../../b.md)
5. [2008](../../../../../2008-split.md)
6. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../split.md)
7. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
