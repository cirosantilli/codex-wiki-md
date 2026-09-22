<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**Directed reachability is [NL-complete](../../../../../nl-complete.md) under [logspace many-one reductions](../../../../../logspace-many-one-reduction.md).** For membership, let $N$ be the number of [vertices](../../../../../vertex-graph-theory.md). Store a current [vertex](../../../../../vertex-graph-theory.md), initially $v$, and a counter initially zero. Accept immediately if the current [vertex](../../../../../vertex-graph-theory.md) is $v'$. Otherwise guess a next [vertex](../../../../../vertex-graph-theory.md), verify by scanning the [input](../../../../../input-computer-science.md) that the appropriate directed [edge](../../../../../edge-of-a-graph.md) exists, move there and increment the counter. Reject a branch that has made $N-1$ steps without reaching $v'$.

Whenever a directed [walk](../../../../../walk-in-a-graph.md) reaches $v'$, removing closed portions between repeated [vertices](../../../../../vertex-graph-theory.md) produces a [path in a graph](../../../../../path-in-a-graph.md) with at most $N-1$ [edges](../../../../../edge-of-a-graph.md). Thus this bound preserves all yes-instances. The current and guessed [vertices](../../../../../vertex-graph-theory.md) and the counter use $O(\log N)$ [bits](../../../../../bit.md), while adjacency checks only need repeated read-only [input](../../../../../input-computer-science.md) scans. All branches halt, so directed reachability belongs to [NL](../../../../../nl-complexity.md).

For hardness, let $A\in\mathrm{NL}$ and fix a [Nondeterministic Turing machine](../../../../../nondeterministic-turing-machine.md) $M$ accepting $A$ in $O(\log n)$ work space. On [input](../../../../../input-computer-science.md) $x$, construct its [configuration graph](../../../../../configuration-graph.md) $C_x$. A [vertex](../../../../../vertex-graph-theory.md) is a possible [Turing machine configuration](../../../../../instantaneous-description-of-a-turing-machine.md) within the fixed work-space bound. Put a directed [edge](../../../../../edge-of-a-graph.md) $C\to D$ exactly when one legal transition of $M$ on $x$ changes $C$ into $D$. Take the initial [Turing machine configuration](../../../../../instantaneous-description-of-a-turing-machine.md) as source, and add a fresh target $t$ with an incoming [edge](../../../../../edge-of-a-graph.md) from every accepting [Turing machine configuration](../../../../../instantaneous-description-of-a-turing-machine.md). Then

$$
x\in A
\quad\Longleftrightarrow\quad
\text{the initial configuration reaches }t\text{ in }C_x.
$$

There are only a [polynomial](../../../../../polynomial-split.md) number of [Turing machine configurations](../../../../../instantaneous-description-of-a-turing-machine.md), by the count used in part (c). More importantly, their encodings have length $O(\log n)$. A [logspace transducer](../../../../../logspace-transducer.md) can enumerate candidate encodings and pairs of candidate encodings with $O(\log n)$ [bits](../../../../../bit.md) of counters. For each pair, it checks the finite transition rule, the scanned [input](../../../../../input-computer-science.md) symbol and the local work-tape change using $O(\log n)$ work space. It emits the corresponding [adjacency matrix](../../../../../adjacency-matrix.md) entry or [edge](../../../../../edge-of-a-graph.md)-list record. Invalid candidate encodings may be discarded or represented by isolated [vertices](../../../../../vertex-graph-theory.md).

The [configuration graph](../../../../../configuration-graph.md) is thus output by a [logspace transducer](../../../../../logspace-transducer.md), rather than stored in its work tapes. This supplies the required [logspace many-one reduction](../../../../../logspace-many-one-reduction.md) from every $A\in\mathrm{NL}$ and proves [NL-completeness](../../../../../nl-complete.md).

$$
\boxed{\mathrm{Reachability}\text{ is NL-complete}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
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
