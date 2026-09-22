<h1 id="a/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First the [graph](../../../../../graph-split.md) is [connected](../../../../../connected-space.md): every component has at least $\delta(G)+1>n/2$ vertices, so two components cannot fit. Take a [longest path](../../../../../longest-path.md) $v_1,\ldots,v_k$. Every neighbour of either endpoint lies on that path. In the index set $\{1,\ldots,k-1\}$ define

$$
I=\{i:v_1v_{i+1}\in E\},\qquad J=\{i:v_iv_k\in E\}.
$$

Their sizes sum to $d(v_1)+d(v_k)\ge n>k-1$, so they share an index $i$. The edges at that index give the cycle

$$
v_1,v_2,\ldots,v_i,v_k,v_{k-1},\ldots,v_{i+1},v_1,
$$

containing every vertex of the path. The minimum-[degree](../../../../../degree-of-a-polynomial.md) assumption and $n\ge3$ ensure the resulting cycle is nondegenerate. If it omitted any [graph](../../../../../graph-split.md) vertex, [connectedness](../../../../../connected-space.md) would supply an edge from outside it to the cycle. Starting with that outside vertex and then following the cycle without closing it gives a path with $k+1$ vertices, contradicting maximality. Thus **the cycle is [Hamiltonian](../../../../../hamiltonian.md)**. This proves [Dirac's theorem](../../../../../dirac-s-theorem.md) in the required case.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
