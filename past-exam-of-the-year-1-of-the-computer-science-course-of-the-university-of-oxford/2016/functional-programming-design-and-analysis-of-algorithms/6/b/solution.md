<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [subset dynamic programming for a Hamiltonian path](../../../../../subset-dynamic-programming-for-a-hamiltonian-path.md), with a Boolean [dynamic programming state](../../../../../dynamic-programming-state.md) $D[S,v]$ for each nonempty [subset](../../../../../subset.md) $S\subseteq V$ and $v\in S$. It is true exactly when there is a [graph path](../../../../../path-in-a-graph.md) using every [vertex](../../../../../vertex-graph-theory.md) of $S$ once, using no other [vertices](../../../../../vertex-graph-theory.md), and ending at $v$. The base and transition are

$$
D[\{v\},v]=\mathrm{true},\qquad
D[S,v]=\bigvee_{u\in S\setminus\{v\}}
\bigl(D[S\setminus\{v\},u]\land A[u,v]\bigr)
\quad(|S|\geq2),
$$

where $A$ is the [adjacency matrix of a directed graph](../../../../../adjacency-matrix-of-a-directed-graph.md).
```
HamiltonianExists(A):
    initialize every D[S,v] to false
    for v in V:
        D[{v},v] = true
    for k = 2,...,n:
        for S subset of V with |S| = k:
            for v in S:
                D[S,v] = any(D[S-{v},u] and A[u,v]
                             for u in S-{v})
    return any(D[V,v] for v in V)
```
For correctness, a valid path ending at $v$ has some penultimate [vertex](../../../../../vertex-graph-theory.md) $u$; removing $v$ yields exactly a path recorded by the corresponding predecessor state. Conversely, extending any true predecessor state by the edge $(u,v)$ produces a path visiting precisely $S$ once. [Mathematical induction](../../../../../mathematical-induction.md) on $|S|$ proves the meaning of every state. Therefore **the final disjunction is true exactly when a [Hamiltonian path](../../../../../hamiltonian-path.md) exists**.

There are $n2^{n-1}$ possible states and at most $n-1$ predecessor checks per state. More exactly, the full set of ordered predecessor checks has size $n(n-1)2^{n-2}$ for $n\geq2$. With constant-time [adjacency matrix](../../../../../adjacency-matrix.md) access and ordinary subset-indexed table access,

$$
\boxed{\text{time }O(n^2 2^n),\qquad\text{space }O(n2^n)}.
$$

The graph is normally assumed nonempty here. If the empty graph is admitted, return the chosen convention for its empty [Hamiltonian path](../../../../../hamiltonian-path.md) separately; it does not affect the bound.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
