# Dependency-degree obstruction on a rooted tree

↑ **Parent:** [Lovász local lemma](lovasz-local-lemma.md)

Let $B_v$ be independent [Bernoulli random variables](bernoulli-distribution.md) on a rooted $d$-ary [tree](tree-graph-theory.md), and put $A_v=\{B_v=1,\ B_w=0\text{ for every child }w\}$. Events at nonadjacent vertices use disjoint variables, giving a [dependency graph of events](dependency-graph-of-events.md) of maximum degree $d+1$. Assign leaf success probability $p$ and successive probabilities $r_{j+1}=p/(1-r_j)^d$. If $p>\max_{0\leq r\leq1}r(1-r)^d=p_d$, the recursion eventually reaches one. Set the final root success probability to one. Each event has probability at most $p$, but following success vertices down from the root must reach an occurring event. Thus the bad events cover the sample space. This gives an upper bound for uniform avoidance thresholds without assuming a converse to the [Lovász local lemma](lovasz-local-lemma.md).

## ↑ Ancestors (7)

1. [Lovász local lemma](lovasz-local-lemma.md)
2. [Probabilistic combinatorics](probabilistic-combinatorics-split.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-13/1/i/solution.md)
