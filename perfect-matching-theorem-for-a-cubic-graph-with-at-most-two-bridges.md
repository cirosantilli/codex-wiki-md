# Perfect matching theorem for a cubic graph with at most two bridges

↑ **Parent:** [Cubic graph](cubic-graph.md)

Every finite connected [cubic graph](cubic-graph.md) with at most two [bridges](bridge-graph-theory.md) has a [perfect matching](perfect-matching.md).

**Proof.** The [handshaking lemma](degree-sum-formula.md) implies that the number $n$ of [vertices](vertex-graph-theory.md) is an [even integer](even-number.md). Fix a nonempty [subset](subset.md) $S$ of the [vertex set](vertex-set.md), and let $q$ count the components of $G-S$ of [odd integer](odd-integer.md) order. For such a component $C$, counting [vertex degrees](degree-graph-theory.md) gives $3|C|=2|E(C)|+d(C)$, where $d(C)$ counts its [edges](edge-of-a-graph.md) to $S$. Thus $d(C)$ is a positive [odd integer](odd-integer.md). If it is one, the unique outgoing [edge](edge-of-a-graph.md) is a [bridge](bridge-graph-theory.md); this happens for at most two components. For all others $d(C)\geq3$. Therefore $3q-4\leq3|S|$. Meanwhile $q\equiv n-|S|\equiv |S|\pmod2$. If $q>|S|$, the same [parity](parity.md) would force $q\geq|S|+2$, contradicting the preceding bound. For $S=\varnothing$ there is one component of [even integer](even-number.md) order and hence $q=0$. Apply [Tutte's theorem on perfect matchings](tutte-s-theorem-on-perfect-matchings.md).

## ↑ Ancestors (7)

1. [Cubic graph](cubic-graph.md)
2. [Graph](graph-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Non-bipartite matching lecture notes by MIT](non-bipartite-matching-lecture-notes-by-mit.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/combinatorial-optimisation/3/b/i/solution.md)
- [Three-edge path decomposition from a perfect matching](three-edge-path-decomposition-from-a-perfect-matching.md)
- [Tutte's theorem on perfect matchings](tutte-s-theorem-on-perfect-matchings.md)
