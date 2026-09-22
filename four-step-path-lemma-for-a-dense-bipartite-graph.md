# Four-step path lemma for a dense bipartite graph

↑ **Parent:** [Graph form of the Balog-Szemerédi-Gowers theorem](graph-form-of-the-balog-szemeredi-gowers-theorem.md)

Let a [bipartite graph](bipartite-graph.md) have $n$ vertices in each class and at least $\rho n^2$ edges. There is a subset $B$ of one class with $|B|\geq\rho n/4$ such that every pair of its vertices has at least $\rho^5n^3/4096$ four-edge walks between them. Declare a pair of left vertices bad if it has fewer than $\tau n$ common neighbours, with $\tau=\rho^2/32$. For a random right vertex $y$, put $U=N(y)$ and let $b(U)$ count ordered bad pairs inside $U$. Then $\mathbb E|U|\geq\rho n$ and $\mathbb Eb(U)\leq\tau n^2$. Some $y$ has $|U|-16b(U)/(\rho n)\geq\rho n/2$, so $|U|\geq\rho n/2$ and $b(U)\leq|U|^2/8$. Remove vertices with more than $|U|/4$ bad partners. At least half remain. For any two remaining vertices, at least $|U|/2$ middle vertices are good partners of both. Each supplies at least $(\tau n)^2$ walks, giving the bound.

## ↑ Ancestors (8)

1. [Graph form of the Balog-Szemerédi-Gowers theorem](graph-form-of-the-balog-szemeredi-gowers-theorem.md)
2. [Balog-Szemerédi-Gowers theorem](balog-szemeredi-gowers-theorem.md)
3. [Additive energy](additive-energy.md)
4. [Additive combinatorics](additive-combinatorics-split.md)
5. [Combinatorics](combinatorics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-76/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-16/2/i/solution.md)
