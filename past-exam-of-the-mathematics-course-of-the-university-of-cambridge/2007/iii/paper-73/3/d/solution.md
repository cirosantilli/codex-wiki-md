<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A standard binary [Hopfield network](../../../../../../hopfield-network.md) contains $M$ recurrently connected units with activities $x_i\in\{-1,+1\}$. Choose symmetric weights $w_{ij}=w_{ji}$, omit self-couplings by setting $w_{ii}=0$, and use zero thresholds for the energy in the next part. To store desired binary patterns $\xi^\mu$, a simple choice is [Hebbian memory weights for a Hopfield network](../../../../../../hebbian-memory-weights-for-a-hopfield-network.md):

$$
\boxed{w_{ij}=\frac1M\sum_{\mu=1}^P\xi_i^\mu\xi_j^\mu\quad(i\ne j),\qquad w_{ii}=0.}
$$

Correlated activity strengthens connections between units agreeing across the training patterns and makes disagreement contribute negatively. This creates attraction toward the stored configurations when cross-talk is sufficiently small. For one stored pattern, its local field is $(M-1)\xi_i/M$, so every bit is stable for $M>1$. With multiple patterns, the other patterns add cross-talk; the rule does not guarantee exact retrieval for an arbitrary collection.

Start retrieval from a partial or corrupted cue and update one unit at a time using its current field

$$
h_i=\sum_{j\ne i}w_{ij}x_j,\qquad
x_i' =\begin{cases}+1,&h_i>0,\\-1,&h_i<0,\\x_i,&h_i=0.\end{cases}
$$

A cyclic or random fair asynchronous schedule lets the network relax toward a fixed point, completing a memory when the cue lies in its basin. This is content-addressable retrieval: the initial pattern selects the memory without an explicit address. Nonzero thresholds can be included in a more general model, but their corresponding linear terms must then be included in the energy.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
