# Prime-regular subgraph from Boolean polynomial constraints

↑ **Parent:** [Combinatorial Nullstellensatz](combinatorial-nullstellensatz.md)

For [prime](prime-number.md) $p$, a [graph](graph-split.md) with $m>(p-1)n$ [edges](edge-of-a-graph.md) and maximum degree at most $2p-1$ contains a nonempty $p$-regular subgraph. Over $\mathbb F_p$, apply the [Combinatorial Nullstellensatz](combinatorial-nullstellensatz.md) on the Boolean edge-variable cube to

$$
\prod_v\left(1-\left(\sum_{e\ni v}x_e\right)^{p-1}\right)-\prod_e(1-x_e).
$$

Its full squarefree [coefficient](coefficient.md) is nonzero because the first product has degree below $m$. A nonzero value cannot occur at the zero vector; at any other Boolean vector the second product vanishes, and the first forces all selected degrees to be multiples of $p$. The maximum-degree condition makes every positive selected degree exactly $p$.

## ↑ Ancestors (7)

1. [Combinatorial Nullstellensatz](combinatorial-nullstellensatz.md)
2. [Alon-Tarsi lemma](alon-tarsi-lemma.md)
3. [Polynomial method in combinatorics](polynomial-method-in-combinatorics.md)
4. [Combinatorics](combinatorics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Nested matching criterion for a regular subgraph](nested-matching-criterion-for-a-regular-subgraph.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-11/3/i/solution.md)
