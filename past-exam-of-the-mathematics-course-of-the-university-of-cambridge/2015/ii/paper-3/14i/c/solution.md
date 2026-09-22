<h1 id="14i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Add missing cross-edges to a hypothetical non-Hamiltonian balanced [bipartite graph](../../../../../../bipartite-graph.md) until it is maximal with that property. The complete bipartite graph is Hamiltonian for $n\geq2$, so a missing cross-edge $uv$ remains. Adding it creates a Hamilton cycle, and removing it gives a Hamilton path

$$
u=A_1,B_1,A_2,B_2,\ldots,A_n,B_n=v.
$$

For each $i$, consider the conditions $uB_i\in E$ and $A_iv\in E$. Since $\deg u+\deg v>n$, they hold together for some $i$. Following the path from $u$ to $A_i$, crossing to $v$, following the remaining path backwards to $B_i$, and crossing back to $u$ gives a Hamilton cycle already in the original maximal graph. This contradiction proves **the stated Hamiltonicity criterion**.

For $n=2m$, two disjoint copies of $K_{m,m}$ have $n$ vertices in each class and minimum degree $m$. For $n=2m+1$, the disjoint union $K_{m,m+1}\sqcup K_{m+1,m}$ has $n$ vertices in each class and minimum degree $m$. Both are disconnected and hence non-Hamiltonian. Thus **the sharp counterexamples have** $\boxed{\delta=\lfloor n/2\rfloor}$ for every $n\geq2$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [14I](../../14i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
