<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Draw $n$ [independent](../../../../../../independent-random-variables.md) pairs of [independent](../../../../../../independent-random-variables.md) [uniform random variables](../../../../../../uniform-random-variable.md) on $[0,1]$. In each pair call the minimum $L$ and maximum $R$, then relabel whole pairs so $R_1<\cdots<R_n$. Merge all endpoints in $(R_{i-1},R_i]$ into [vertex](../../../../../../vertex-graph-theory.md) $i$, with $R_0=0$, and join the blocks containing the two endpoints of each pair, orienting from the right endpoint to the left. [Self-loops](../../../../../../loop-graph-theory.md) are retained. This gives the [uniform linearized chord diagram](../../../../../../uniform-linearized-chord-diagram.md) representation.

Before ordering, a pair has joint density $2$ on $0<L<R<1$. Consequently its maximum has distribution $\Pr(R\le r)=r^2$ and density $2r$; conditional on $R=r$, its minimum is uniform on $[0,r]$. Independence and relabelling give the equivalent precise description

$$
\boxed{R_1^2<\cdots<R_n^2\text{ are the order statistics of }n\text{ independent }U(0,1)\text{ variables};\quad L_i\mid(R_1,\ldots,R_n)\ \text{independently }U(0,R_i).}
$$

Every one of the $(2n)!$ relative orderings of the independently drawn labelled endpoints has the same [probability](../../../../../../probability.md). After forgetting pair labels and within-pair labels, each matching of $2n$ ordered points is produced by $2^n n!$ orderings. Thus its matching is uniform among the $(2n-1)!!$ pairings.

To prove equivalence with the recursive [graph](../../../../../../graph-split.md) law, remove the last endpoint and its mate from a uniform pairing. The remaining ordered points have a uniform $(n-1)$-pairing, and the mate's old rank is uniform among the $2n-1$ possible ranks, independently of that smaller pairing. Conversely insert the mate into a uniformly chosen one of its $2n-1$ gaps, and pair it with the new final endpoint. For each old [vertex](../../../../../../vertex-graph-theory.md) block, the number of gaps assigned to it is exactly the number of endpoints already in that block, hence its old total [vertex degree](../../../../../../degree-graph-theory.md). These are the gaps immediately before each endpoint of that block. The last gap, after the last old endpoint, makes both new endpoints belong to the new final block and produces a [self-loop](../../../../../../loop-graph-theory.md). Therefore the attachment [probabilities](../../../../../../probability.md) are $d_i/(2n-1)$ for old [vertices](../../../../../../vertex-graph-theory.md) and $1/(2n-1)$ for the new one. Induction proves **the continuous construction and the recursive LCD model have the same distribution**. Inserting a left endpoint into an old block raises exactly that [vertex](../../../../../../vertex-graph-theory.md)'s [vertex degree](../../../../../../degree-graph-theory.md) without splitting any old block.

<a id="6/a/image-a-linearized-chord-diagram-with-six-vertex-blocks-six-edges-and-loops-counted-twice-in-the-block-degrees"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-12-lcd.png)

**[Figure 1](#6/a/image-a-linearized-chord-diagram-with-six-vertex-blocks-six-edges-and-loops-counted-twice-in-the-block-degrees). A linearized chord diagram with six vertex blocks, six edges and loops counted twice in the block degrees**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
