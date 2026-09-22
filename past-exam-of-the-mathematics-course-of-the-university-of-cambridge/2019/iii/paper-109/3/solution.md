<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $N[A]$ for the [closed graph neighbourhood](../../../../../closed-graph-neighbourhood.md) of $A$. Since $|N[A]|=|A|+|\partial_vA|$, minimizing the [external vertex boundary](../../../../../external-vertex-boundary.md) at fixed cardinality is equivalent to minimizing the closed neighbourhood. The [vertex-isoperimetric inequality in a grid](../../../../../vertex-isoperimetric-inequality-in-a-grid.md) says that, among all $t$-vertex subsets of $[k]^n$, the first $t$ vertices in the [simplicial order on a grid](../../../../../simplicial-order-on-a-grid.md) minimize this quantity.

We prove the theorem by [mathematical induction](../../../../../mathematical-induction.md) on $n$, using the allowed two-dimensional case. Fix a coordinate $i$ and write $A_j\subseteq[k]^{n-1}$ for the section in which that coordinate equals $j$. Replace each $A_j$ by the equally large initial simplicial segment $B_j$. By induction, $|N[B_j]|\leq|N[A_j]|$. The [section formula for a grid neighbourhood](../../../../../section-formula-for-a-grid-neighbourhood.md) gives

$$
N[A]_j=N[A_j]\cup A_{j-1}\cup A_{j+1},
\qquad A_0=A_{k+1}=\varnothing.
$$

For the compressed family, $N[B_j],B_{j-1},B_{j+1}$ are nested initial segments, so the size of their union is the maximum of their sizes. That maximum is no larger than the size of the corresponding uncompressed union. Summing over $j$ proves that [coordinate compression in a product of paths](../../../../../coordinate-compression-in-a-product-of-paths.md) does not enlarge the boundary.

Apply these compressions in every coordinate, choosing among boundary-minimizing outcomes one with least coordinate-sum weight. If the result were not an initial simplicial segment, it would contain a later vertex while omitting an earlier one. After cancelling coordinates in which they agree, this gives an inversion in a two-coordinate face. Replacing the occupied portion of that face by the equal-size initial segment in $[k]^2$ does not increase its neighbourhood by the assumed two-dimensional theorem, while it strictly lowers the weight. This contradiction is the [local-to-global lemma for simplicial grid order](../../../../../local-to-global-lemma-for-simplicial-grid-order.md), and completes the induction.

For the second assertion, list the vertices of $Q_2$ in the [Gray code](../../../../../gray-code.md) order

$$
00,\ 01,\ 11,\ 10.
$$

The three consecutive edges form a copy of the four-vertex path $P_4$. Pairing the $2n$ binary coordinates and applying this identification in each pair realizes

$$
[4]^n=P_4^n
$$

as a [spanning subgraph](../../../../../spanning-subgraph.md) of the [hypercube graph](../../../../../hypercube-graph.md) $Q_{2n}$. For any fixed vertex set, adding graph edges can only enlarge its [external vertex boundary](../../../../../external-vertex-boundary.md). Hence a $t$-set in $Q_{2n}$ has boundary at least that of the same $t$ vertices in $[4]^n$, which by hypothesis is at least $s$. Therefore

$$
\boxed{|\partial_{Q_{2n}}A|\geq s\quad\text{whenever }|A|=t.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 109](../../paper-109-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
