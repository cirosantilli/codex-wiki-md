<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [three-colourability problem](../../../../../../three-colourability-problem.md) belongs to [NP](../../../../../../np-complexity.md): a colour assignment is a polynomial-length [complexity certificate](../../../../../../certificate-complexity.md), and all edges can be checked in $O(|V|+|E|)$ time.

For [NP-hardness](../../../../../../np-hardness.md), reduce [3-SAT](../../../../../../3-sat.md) to the [three-colourability problem](../../../../../../three-colourability-problem.md). Start with a palette [graph triangle](../../../../../../triangle-in-a-graph.md) with vertices $T,F,B$. Its colours are necessarily distinct, and name them by these vertices. For each [Boolean variable](../../../../../../boolean-variable.md) $u$, add vertices $u,\bar u$, join them to each other, and join each to $B$. The [graph triangle](../../../../../../triangle-in-a-graph.md) $B,u,\bar u$ is the forcing component of the [Boolean-pair colouring gadget](../../../../../../boolean-pair-colouring-gadget.md), so the two literal vertices receive opposite colours $T,F$.

For each [Boolean clause](../../../../../../clause-of-a-boolean-formula.md), attach a fresh copy of the [three-colour clause gadget](../../../../../../three-colour-clause-gadget.md), identify its $t$ with the palette vertex $T$, and identify its three input vertices with the [Boolean clause](../../../../../../clause-of-a-boolean-formula.md)'s [Boolean literal](../../../../../../boolean-literal.md) vertices. Copies share only palette or literal vertices. A [Boolean clause](../../../../../../clause-of-a-boolean-formula.md) with one or two [Boolean literals](../../../../../../boolean-literal.md) is padded to three by repeating a literal; an empty [Boolean clause](../../../../../../clause-of-a-boolean-formula.md) can be mapped immediately to the uncolourable graph $K_4$.

Any [graph colouring](../../../../../../graph-coloring.md) with three colours gives a truth assignment by reading colour $T$ as true. The [three-colour clause gadget](../../../../../../three-colour-clause-gadget.md) forbids three false inputs, so every [Boolean clause](../../../../../../clause-of-a-boolean-formula.md) is satisfied. Conversely, any satisfying truth assignment colours the literal pairs, and the extension property proved above independently colours the fresh auxiliary vertices of each clause. Thus the entire graph is three-colourable exactly when the formula is satisfiable.

There are $3+2n+5m$ vertices for $n$ variables and $m$ nonempty padded clauses, and $O(n+m)$ edges. The construction is a [polynomial-time many-one reduction](../../../../../../polynomial-time-many-one-reduction.md). Using the permitted [NP-completeness](../../../../../../np-completeness.md) of [3-SAT](../../../../../../3-sat.md), we obtain

$$
\boxed{\text{three-colourability is NP-complete}.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
