# Numerical upper-bound pruning without a solution witness

↑ **Parent:** [A-star search](a-star-search.md)

Suppose $0\le h(n)\le h^*(n)\le u(n)$ in a [search problem](search-problem.md), with $h^*=\infty$ at dead ends. Every finite $g(n)+u(n)$ bounds some reachable solution cost from above, so their running minimum $B$ is at least the global optimum $C^*$. Every node of an optimal path has $g+h\le C^*\le B$, and therefore survives the displayed strict pruning rule. Ordinary [A-star search](a-star-search.md) can continue to a selected goal without receiving a path witnessing $u$.

Equality pruning is unsafe without a stored incumbent solution: when $B=C^*$, it could delete every optimal continuation. A numerical upper bound does not by itself provide a [plan](plan.md) to return. This distinguishes an upper-bound certificate from a constructed solution in [branch and bound](branch-and-bound.md).

## ↑ Ancestors (9)

1. [A-star search](a-star-search.md)
2. [Best-first search](best-first-search.md)
3. [Graph search](graph-search.md)
4. [Graph](graph-split.md)
5. [Graph theory](graph-theory-split.md)
6. [Foundations of mathematics](foundations-of-mathematics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
