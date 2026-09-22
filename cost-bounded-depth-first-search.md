# Cost-bounded depth-first search

↑ **Parent:** [Depth-first search](depth-first-search.md)

A [cost-bounded depth-first search](cost-bounded-depth-first-search.md) follows the usual [depth-first search](depth-first-search.md) order but immediately rejects a generated [search node](search-node.md) whose accumulated [path cost](path-cost.md) exceeds a threshold $L$. It can also return the least rejected [path cost](path-cost.md), providing the next threshold for [iterative lengthening search](iterative-lengthening-search.md). Positive [step costs](step-cost.md) ensure that a rejected prefix cannot become a cheaper extension. With finite [branching factor](branching-factor.md) and every [step cost](step-cost.md)ing at least $\epsilon>0$, every admitted [search node](search-node.md) has [search depth](search-depth.md) at most $\lfloor L/\epsilon\rfloor$, so the pass terminates. Merely requiring every individual [step cost](step-cost.md) to be positive does not exclude an infinite branch of finite total [path cost](path-cost.md).

## ↑ Ancestors (4)

1. [Depth-first search](depth-first-search.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Cost-bounded depth-first search](cost-bounded-depth-first-search.md)
- [Iterative lengthening search](iterative-lengthening-search.md)
