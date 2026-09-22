<h1 id="17i/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Modulo three, the quintic has no linear factor: its value is $-1$ at every element of $\mathbb F_3$. The monic irreducible quadratics over this [field](../../../../../../../field.md) are $t^2+1$, $t^2+t+2$ and $t^2+2t+2$. Division leaves respectively $-1$, $t-1$ and $t-1$, all nonzero. A reducible quintic has a factor of degree at most two, so it is irreducible modulo three and therefore over $\mathbb Q$. Its [Galois group](../../../../../../../galois-group.md) is transitive on five roots.

Modulo two its squarefree factorization is

$$
t^5-t-1\equiv(t^2+t+1)(t^3+t^2+1).
$$

Both factors are irreducible, so the [Frobenius cycle type](../../../../../../../frobenius-cycle-type.md) theorem gives an element that is a disjoint transposition times a three-cycle. Cubing it gives a transposition.

The [prime-degree transposition criterion](../../../../../../../prime-degree-transposition-criterion.md) can be proved here: a transitive subgroup of prime degree containing a transposition is the whole [symmetric group](../../../../../../../symmetric-group.md). Construct a graph on the five roots whose edges are the pairs swapped by all conjugates of this transposition. The [group](../../../../../../../group-split.md) acts transitively on vertices and permutes connected components, so all component sizes are equal and divide five. An edge rules out size one; the graph is connected. Edge transpositions of any connected graph generate the full [symmetric group](../../../../../../../symmetric-group.md), for instance by transporting swaps along a spanning tree. All belong to the [Galois group](../../../../../../../galois-group.md), proving

$$
\boxed{\operatorname{Gal}(t^5-t-1/\mathbb Q)\cong S_5}.
$$

The prime-degree condition is essential to the short transposition argument.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [17I](../../../17i.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
