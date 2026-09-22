<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $J(A)$ for the partition supremum. Empty cells are permitted, so $J\geq\mu_i$ for each $i$, and $J(A)\leq\sum_i\mu_i(A)$ is finite. Also $J(\varnothing)=0$.

Let $A=\bigsqcup_{j\geq1}B_j$. Any measurable partition $A=\bigsqcup_iA_i$ yields

$$
\sum_i\mu_i(A_i)=\sum_j\sum_i\mu_i(A_i\cap B_j)\leq\sum_jJ(B_j).
$$

Taking its supremum gives one inequality. Conversely, for any $\varepsilon>0$ choose for each $j$ a partition $B_j=\bigsqcup_iB_{ji}$ whose sum exceeds $J(B_j)-\varepsilon2^{-j}$. The sets $A_i=\bigsqcup_jB_{ji}$ partition $A$, and [countable additivity](../../../../countable-additivity.md) of each $\mu_i$ gives $J(A)\geq\sum_jJ(B_j)-\varepsilon$. Let $\varepsilon\downarrow0$. Thus **$J$ is a [finite measure](../../../../finite-measure.md)**.

If another [measure](../../../../measure-split.md) $\nu$ dominates every $\mu_i$, then for every such partition $\sum_i\mu_i(A_i)\leq\sum_i\nu(A_i)=\nu(A)$. Consequently $J\leq\nu$. Hence **$J=\bigvee_i\mu_i$ is the least dominating [measure](../../../../measure-split.md)**, the [finite supremum of positive measures](../../../../finite-supremum-of-positive-measures.md). It generally differs from the pointwise maximum of the numbers $\mu_i(A)$: the maximizing index may differ between pieces of $A$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the real and harmonic analysis course of the University of Oxford](../../../split.md)
5. [Real and harmonic analysis course of the University of Oxford](../../../../real-and-harmonic-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
