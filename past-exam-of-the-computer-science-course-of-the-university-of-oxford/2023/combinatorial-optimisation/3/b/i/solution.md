<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [Tutte's theorem on perfect matchings](../../../../../../tutte-s-theorem-on-perfect-matchings.md): a finite [graph](../../../../../../graph-split.md) has a [perfect matching](../../../../../../perfect-matching.md) if and only if, for every $S\subseteq V$, the number $q(S)$ of [connected components of a graph](../../../../../../component-graph-theory.md) of [odd integer](../../../../../../odd-integer.md) order in $G-S$ is at most $|S|$.

First, the [handshaking lemma](../../../../../../degree-sum-formula.md) gives $3|V|=2|E|$, so $|V|$ is an [even integer](../../../../../../even-number.md). Fix $S\ne\varnothing$. For each [connected component of a graph](../../../../../../component-graph-theory.md) $C$ of [odd integer](../../../../../../odd-integer.md) order in $G-S$, let $d(C)$ count its [edges](../../../../../../edge-of-a-graph.md) to $S$. Counting [vertex degrees](../../../../../../degree-graph-theory.md) inside $C$ gives

$$
3|C|=2|E(C)|+d(C).
$$

Thus $d(C)$ is an [odd integer](../../../../../../odd-integer.md); it is positive because $G$ is a [connected graph](../../../../../../connected-graph.md). If $d(C)=1$, its unique outgoing [edge](../../../../../../edge-of-a-graph.md) is a [bridge](../../../../../../bridge-graph-theory.md). Distinct such components yield distinct [bridges](../../../../../../bridge-graph-theory.md), so there are at most two of them. Every other such component has $d(C)\geq3$. Therefore

$$
3q(S)-4\leq\sum_{C:\,|C|\text{ odd}}d(C)\leq3|S|.
$$

The last inequality holds because each [vertex](../../../../../../vertex-graph-theory.md) of $S$ has [vertex degree](../../../../../../degree-graph-theory.md) three. Furthermore,

$$
q(S)\equiv |V\setminus S|\equiv |S|\pmod2,
$$

since components of [even integer](../../../../../../even-number.md) order do not affect [parity](../../../../../../parity.md), and $|V|$ is an [even integer](../../../../../../even-number.md). If $q(S)>|S|$, this [parity](../../../../../../parity.md) forces $q(S)\geq|S|+2$, contradicting the bound $3q(S)\leq3|S|+4$.

For $S=\varnothing$, the only component is the whole [connected graph](../../../../../../connected-graph.md), of [even integer](../../../../../../even-number.md) order, so $q(\varnothing)=0$. Thus every $S$ satisfies the criterion, and **$G$ has a [perfect matching](../../../../../../perfect-matching.md)**. This proves the [perfect matching theorem for a cubic graph with at most two bridges](../../../../../../perfect-matching-theorem-for-a-cubic-graph-with-at-most-two-bridges.md) directly from [Tutte's theorem on perfect matchings](../../../../../../tutte-s-theorem-on-perfect-matchings.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Combinatorial optimisation](../../../../combinatorial-optimisation-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
