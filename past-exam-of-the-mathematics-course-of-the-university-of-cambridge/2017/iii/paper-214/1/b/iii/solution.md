<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For each integer $j$, consider the cut of horizontal [edges](../../../../../../../edge-of-a-graph.md) joining column $j$ to column $j+1$ inside the strip. It contains exactly $2k+1$ [edges](../../../../../../../edge-of-a-graph.md). Its being completely closed has [probability](../../../../../../../probability.md)

$$
r_k=(1-p)^{2k+1}>0.
$$

Different cuts use disjoint [edge](../../../../../../../edge-of-a-graph.md) sets, so these closed-cut events are independent. Any [graph path](../../../../../../../path-in-a-graph.md) from column zero to column $n>0$, even one that wanders to other columns first, must cross each cut with $j=0,\ldots,n-1$. None of those $n$ cuts may therefore be completely closed. This gives the [closed-cut bound for percolation in a strip](../../../../../../../closed-cut-bound-for-percolation-in-a-strip.md):

$$
q_k(n)\leq(1-r_k)^n.
$$

Taking negative logarithms, dividing by $n$ and taking the established [limit of a sequence](../../../../../../../limit-of-a-sequence.md) yields

$$
\boxed{f_k(p)\geq-\log\bigl(1-(1-p)^{2k+1}\bigr)>0.}
$$

The strict inequality uses both finite width and $p<1$. It is consistent with $f_k(p)\leq-\log p$, since $1-(1-p)^{2k+1}\geq p$. At $p=1$ all strip connections occur and the decay rate is zero, so that excluded endpoint would invalidate strict positivity. The mechanism is a positive [probability](../../../../../../../probability.md) of an impermeable finite cut, rather than any assumption that the unrestricted lattice is subcritical.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 214](../../../../paper-214-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
