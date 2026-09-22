# Ordinal heuristic comparator

↑ **Parent:** [Heuristic function](heuristic-function.md)

A comparison oracle revealing the ordering of remaining optimal costs without returning their magnitudes. It supplies enough information for [greedy best-first search](greedy-best-first-search.md). Its ordering alone does not provide the numerical differences needed to compare sums with independently varying accumulated costs. For $g(n)=5$, $g(m)=1$, remaining costs $(1,2)$ and $(1,10)$ have the same pairwise order but give opposite orderings of $g+h^*$.

## ↑ Ancestors (7)

1. [Heuristic function](heuristic-function.md)
2. [Search problem](search-problem.md)
3. [Computational problem](computational-problem.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)
