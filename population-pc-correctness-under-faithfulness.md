# Population PC correctness under faithfulness

↑ **Parent:** [PC algorithm](pc-algorithm.md)

With an exact [conditional independence](conditional-independence.md) oracle and [faithfulness of a directed acyclic graph](faithfulness-of-a-directed-acyclic-graph.md), the skeleton phase of the [PC algorithm](pc-algorithm.md) deletes precisely the nonedges. A true edge cannot be [D-separated](d-separation.md) by a set excluding its endpoints. For nonadjacent vertices, choose the later vertex $v$ in a [topological ordering](topological-ordering.md); its parents separate it from the earlier nonparent. True parent edges survive throughout, so this separator remains available among the algorithm's candidate neighbour sets. For an unshielded triple $u-v-w$, any recorded separator of $u,w$ excludes $v$ exactly when the triple is an [unshielded collider](unshielded-collider.md). The [skeleton and collider characterization of Markov equivalence](skeleton-and-collider-characterization-of-markov-equivalence.md) therefore identifies the correct equivalence class. Directions compelled throughout that class give its [completed partially directed acyclic graph](completed-partially-directed-acyclic-graph.md).

## ↑ Ancestors (7)

1. [PC algorithm](pc-algorithm.md)
2. [Causal directed acyclic graph](causal-directed-acyclic-graph.md)
3. [Causal inference](causal-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205/4/solution.md)
