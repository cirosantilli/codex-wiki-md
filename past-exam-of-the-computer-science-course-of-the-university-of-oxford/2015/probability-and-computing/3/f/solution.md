<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Order the [edges](../../../../../edge-of-a-graph.md) arbitrarily and fix their colours one at a time. After a partial assignment $P$, regard all unassigned [edges](../../../../../edge-of-a-graph.md) as independent fair red/blue choices, and compute

$$
Q(P)=\mathbb E[Z\mid P].
$$

The [conditional expectation of a monochromatic clique count](../../../../../conditional-expectation-of-a-monochromatic-clique-count.md) is easy to compute. For each four-[vertex](../../../../../vertex-graph-theory.md) [subset](../../../../../subset.md) $A$, let $r$ be the number of its six [edges](../../../../../edge-of-a-graph.md) still unassigned. Its contribution $q_A(P)$ to $Q(P)$ is

$$
q_A(P)=\begin{cases}
0,&\text{both colours already occur among its fixed edges},\\
2^{-r},&\text{at least one edge is fixed, all in the same colour},\\
2^{1-r}=1/32,&\text{none of its six edges is fixed}.
\end{cases}
$$

In the second case, every remaining [edge](../../../../../edge-of-a-graph.md) must match the already fixed colour; this includes a completely fixed [monochromatic](../../../../../monochromatic-set.md) copy, for which $r=0$ and the contribution is one. In the last case, the six unassigned [edges](../../../../../edge-of-a-graph.md) may become either all red or all blue. By [linearity of expectation](../../../../../linearity-of-expectation.md),

$$
Q(P)=\sum_{|A|=4}q_A(P).
$$

For the next unassigned [edge](../../../../../edge-of-a-graph.md) $e$, compute $Q(P,e=\text{red})$ and $Q(P,e=\text{blue})$. The [law of total expectation](../../../../../law-of-total-expectation.md) gives

$$
Q(P)=\frac12Q(P,e=\text{red})+\frac12Q(P,e=\text{blue}).
$$

Choose the colour with the smaller value, resolving a tie by a fixed rule. At least one is at most their average, so the [loop invariant](../../../../../loop-invariant.md) is that $Q$ never increases. Initially $Q=\binom n4/32$; once every [edge](../../../../../edge-of-a-graph.md) is fixed, there is no randomness left and $Q=Z$. Therefore the [method of conditional expectations](../../../../../method-of-conditional-probabilities.md) guarantees

$$
\boxed{Z\leq\frac1{32}\binom n4.}
$$

A direct implementation recomputes both sums over all $O(n^4)$ four-[vertex](../../../../../vertex-graph-theory.md) [subsets](../../../../../subset.md) for each of the $O(n^2)$ [edges](../../../../../edge-of-a-graph.md), requiring $O(n^6)$ arithmetic operations. The comparisons can be exact: every contribution is a multiple of $1/32$, so store $32Q$ as an [integer](../../../../../integer-split.md) with $O(\log n)$ [bits](../../../../../bit.md). This gives $O(n^6\log n)$ [bit complexity](../../../../../bit-complexity.md) with elementary arithmetic, and hence a deterministic [polynomial time](../../../../../polynomial-time.md) construction. No random sampling is performed by this [derandomization](../../../../../derandomization.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Probability and computing](../../../probability-and-computing-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
