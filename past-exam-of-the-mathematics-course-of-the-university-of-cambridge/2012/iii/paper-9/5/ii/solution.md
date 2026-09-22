<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [persistence of unsampled graph components](../../../../../../persistence-of-unsampled-graph-components.md) prevents the mass from each size band from disappearing entirely before $t_c$. More precisely, a band $[k,Dk)$ containing at least $\delta n/4$ [vertices](../../../../../../vertex-graph-theory.md) retains at least $\beta n$ [vertices](../../../../../../vertex-graph-theory.md) in that same band after at most $n/k$ steps, [with high probability](../../../../../../with-high-probability.md), for a fixed $\beta>0$ depending only on $\delta,D$. To see why, each initial [graph component](../../../../../../component-graph-theory.md) in that band has a fixed positive [probability](../../../../../../probability.md) that none of the offered [edge](../../../../../../edge-of-a-graph.md) endpoints touches it during the interval. Such a [graph component](../../../../../../component-graph-theory.md) remains unchanged regardless of the selection rule. The [McDiarmid inequality](../../../../../../mcdiarmid-s-inequality.md) concentrates the total mass of these untouched [graph components](../../../../../../component-graph-theory.md). The reusable lemma supplies the full uniform-in-starting-time argument, including the version that samples absent [edges](../../../../../../edge-of-a-graph.md).

Choose finitely many disjoint bands $[D^j,D^{j+1})$, $j=0,\ldots,J$, with $(J+1)\beta>1$. Part (i) provides at least $\delta n/4$ [vertices](../../../../../../vertex-graph-theory.md) in band $j$ at its time $t_{D^j}$. Each interval from that time to $t_c$ has length at most $n/D^j$, so persistence leaves at least $\beta n$ [vertices](../../../../../../vertex-graph-theory.md) in every one of these disjoint bands at the common time $t_c$. A [union bound](../../../../../../boole-s-inequality.md) over this fixed finite number of bands makes all the conclusions simultaneous. Their total exceeds $n$, a contradiction. **No fixed two-choice Achlioptas rule satisfies the explosive percolation hypothesis.**

This [continuity of fixed-choice percolation](../../../../../../continuity-of-fixed-choice-percolation.md) is the fixed-choice obstruction proved by Riordan and Warnke; their [original research paper](https://arxiv.org/abs/1102.5306) also treats a broader class of rules. The argument here does not apply when the number of offered choices grows with $n$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
