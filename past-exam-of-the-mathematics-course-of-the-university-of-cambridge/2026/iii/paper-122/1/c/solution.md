<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The sharp [Hamilton cycle](../../../../../../hamilton-cycle.md) threshold for the [Erdős-Rényi model](../../../../../../erdos-renyi-model.md) says that

$$
\mathbb P(G(n,p)\text{ is Hamiltonian})\longrightarrow1
$$

only above the window $np=\log n+\log\log n+o(1)$. The hypothesis therefore places $p(n)$ above that window. The [Hamiltonicity-to-pancyclicity sprinkling principle](../../../../../../hamiltonicity-to-pancyclicity-sprinkling-principle.md) then says that three independent $G(n,p(n))$ rounds contain every [cycle graph](../../../../../../cycle-graph.md) $C_\ell$, $3\leq\ell\leq n$, [with high probability](../../../../../../with-high-probability.md): one round supplies a Hamilton cycle, while the other two supply the chords and short-cycle edges used to obtain all intermediate lengths.

The union of the three rounds has individual edge probability

$$
q=1-(1-p(n))^3\leq3p(n).
$$

By the standard monotone coupling, it is a subgraph of $G(n,3p(n))$. Since being [pancyclic](../../../../../../pancyclic-graph.md) is an increasing graph property, the required probability tends to one. If $3p(n)>1$, interpret the latter parameter as $\min\{3p(n),1\}$, in which case the conclusion is immediate.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
