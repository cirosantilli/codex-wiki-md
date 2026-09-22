<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The printed question calls the route a [path in a graph](../../../../../path-in-a-graph.md) and writes $p\subseteq E(G)$, without specifying whether repeated [vertices](../../../../../vertex-graph-theory.md) are allowed.[Printed p. 4, Question 3(e)](../../../../../computational-complexity-examination-paper-of-the-university-of-oxford-2015.md) Use the computational reachability convention that a permitted route is a directed [walk](../../../../../walk-in-a-graph.md): repeated [vertices](../../../../../vertex-graph-theory.md) are allowed and length counts traversed [edges](../../../../../edge-of-a-graph.md) with multiplicity. This matters for the [integer parity](../../../../../parity-mathematics.md) restriction, because deleting a closed portion of odd length can change the [integer parity](../../../../../parity-mathematics.md). The proof below establishes the stated [NL](../../../../../nl-complexity.md)-completeness for this convention; it does not establish that claim for a simple [path in a graph](../../../../../path-in-a-graph.md).

For membership of [even-length directed reachability](../../../../../even-length-directed-reachability.md) in [NL](../../../../../nl-complexity.md), form the conceptual parity [graph](../../../../../graph-split.md) with [vertex set](../../../../../vertex-set.md)

$$
V(G)\times\{0,1\}
$$

and directed [edges](../../../../../edge-of-a-graph.md)

$$
(u,b)\longrightarrow(w,1-b)
\quad\Longleftrightarrow\quad (u,w)\in E(G).
$$

After a directed [walk](../../../../../walk-in-a-graph.md) of length $j$ from $(v,0)$, the second coordinate equals $j\bmod2$. Therefore there is an even-length directed [walk](../../../../../walk-in-a-graph.md) from $v$ to $v'$ in $G$ exactly when $(v',0)$ is reachable from $(v,0)$ in this parity [graph](../../../../../graph-split.md). It has $2N$ [vertices](../../../../../vertex-graph-theory.md). Guess successive [edges](../../../../../edge-of-a-graph.md) while storing the original current [vertex](../../../../../vertex-graph-theory.md), one [parity bit](../../../../../parity-bit.md), and a counter bounded by $2N-1$. If the target pair is reachable, it has a simple [path in a graph](../../../../../path-in-a-graph.md) in this enlarged [graph](../../../../../graph-split.md) of at most $2N-1$ [edges](../../../../../edge-of-a-graph.md). This is an [NL](../../../../../nl-complexity.md) procedure; the parity [graph](../../../../../graph-split.md) need not be materialized.

For [NL](../../../../../nl-complexity.md)-hardness, reduce directed reachability by subdividing each directed [edge](../../../../../edge-of-a-graph.md) $(u,w)$ with its own new [vertex](../../../../../vertex-graph-theory.md) $a_{uw}$:

$$
u\longrightarrow a_{uw}\longrightarrow w.
$$

Retain $v,v'$ as the endpoints and add no other [edges](../../../../../edge-of-a-graph.md). Every original directed [walk](../../../../../walk-in-a-graph.md) of length $j$ becomes a directed [walk](../../../../../walk-in-a-graph.md) of even length $2j$. Conversely, a directed [walk](../../../../../walk-in-a-graph.md) between original [vertices](../../../../../vertex-graph-theory.md) in the new [graph](../../../../../graph-split.md) must alternate original and subdivision [vertices](../../../../../vertex-graph-theory.md). Compressing each two-[edge](../../../../../edge-of-a-graph.md) segment recovers a directed [walk](../../../../../walk-in-a-graph.md) in $G$. Hence

$$
\langle G,v,v'\rangle\in\mathrm{Reachability}
\quad\Longleftrightarrow\quad
\langle G',v,v'\rangle\in\mathrm{E\text{-}Reachability}.
$$

A [logspace transducer](../../../../../logspace-transducer.md) enumerates the original [edges](../../../../../edge-of-a-graph.md), labels each new [vertex](../../../../../vertex-graph-theory.md) by its [edge](../../../../../edge-of-a-graph.md) endpoints or its position in the [input](../../../../../input-computer-science.md), and emits its two replacement [edges](../../../../../edge-of-a-graph.md). All labels and counters take $O(\log n)$ [bits](../../../../../bit.md), and the output is of [polynomial](../../../../../polynomial-split.md) size. Thus this is a [logspace many-one reduction](../../../../../logspace-many-one-reduction.md), proving

$$
\boxed{\mathrm{E\text{-}Reachability}\text{ is NL-complete}.}
$$

As in ordinary reachability, a zero-length directed [walk](../../../../../walk-in-a-graph.md) is permitted, so $v=v'$ is an immediate yes-instance. Both the membership procedure and the subdivision [many-one reduction](../../../../../many-one-reduction.md) preserve that case.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Computational complexity](../../../computational-complexity-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
