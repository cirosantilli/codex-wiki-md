# Avoiding short repetitions in an edge coloring

↑ **Parent:** [Repetitively colored path](repetitively-colored-path.md)

For a finite [graph](graph-split.md) of [maximum degree](maximum-degree.md) $\Delta\geq1$, a random independent [edge coloring](edge-coloring.md) and the [Lovász local lemma](lovasz-local-lemma.md) prove existence of a coloring with no repetitively colored four-edge path when $k\geq8\Delta^{3/2}$, and no repetitively colored six-edge path when $k\geq5\Delta^{5/3}$.

A fixed edge lies in at most $\ell\Delta^{\ell-1}$ unoriented paths of length $\ell$. Hence a four-edge event has a closed dependency neighbourhood of size at most $16\Delta^3$ and probability $k^{-2}$; the symmetric local-lemma product is at most $16e\Delta^3/k^2$. The corresponding six-edge quantities are $36\Delta^5$, $k^{-3}$ and $36e\Delta^5/k^3$. The stated constants make both products less than one.

Both lengths can be excluded simultaneously with $k\geq C\Delta^{5/3}$ for an absolute constant $C$. Apply the [asymmetric Lovász local lemma](asymmetric-lovasz-local-lemma.md) with parameters $x_4=2/k^2$, $x_6=2/k^3$. A path of length $\ell\in\{4,6\}$ meets at most $4\ell\Delta^3$ four-edge paths and $6\ell\Delta^5$ six-edge paths. The sums of neighbour parameters are therefore bounded by constants times $C^{-2}\Delta^{-1/3}+C^{-3}$. Choosing $C$ sufficiently large makes both products in the local-lemma inequalities at least one half, establishing the claim.

## ↑ Ancestors (7)

1. [Repetitively colored path](repetitively-colored-path.md)
2. [Path in a graph](path-in-a-graph.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford/2009/b/6/b/iii/solution.md)
