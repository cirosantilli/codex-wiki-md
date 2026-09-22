# Even-length directed reachability

↑ **Parent:** [ST-connectivity](st-connectivity.md)

Decide whether a finite [directed graph](directed-graph.md) has an even-length directed [walk](walk-in-a-graph.md) from a specified source $s$ to a specified target $t$. [Vertices](vertex-graph-theory.md) may repeat and a zero-length [walk](walk-in-a-graph.md) is allowed. The [NL](nl-complexity.md)-completeness proof uses the [graph](graph-split.md) of pairs $(v,b)$ with $b\in\{0,1\}$ tracking [integer parity](parity-mathematics.md): every original [edge](edge-of-a-graph.md) flips $b$, and acceptance means reaching $(t,0)$ from $(s,0)$. At most $2|V|-1$ steps are needed in the parity [graph](graph-split.md). For hardness, subdivide every [edge](edge-of-a-graph.md) of an ordinary reachability instance into two directed [edges](edge-of-a-graph.md). Both constructions are computable by [logspace transducers](logspace-transducer.md). Requiring a simple [path in a graph](path-in-a-graph.md) in the original [graph](graph-split.md) changes the question; deleting an odd closed portion need not preserve [integer parity](parity-mathematics.md).

## ↑ Ancestors (10)

1. [ST-connectivity](st-connectivity.md)
2. [NL-complete](nl-complete.md)
3. [NL (complexity)](nl-complexity.md)
4. [Logarithmic space](logarithmic-space.md)
5. [Space complexity](space-complexity.md)
6. [Complexity class](complexity-class.md)
7. [Computational complexity theory](computational-complexity-theory.md)
8. [Theoretical computer science](theoretical-computer-science-split.md)
9. [Computer science](computer-science-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Computational Complexity examination paper of the University of Oxford (2015)](computational-complexity-examination-paper-of-the-university-of-oxford-2015.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/computational-complexity/3/e/solution.md)
