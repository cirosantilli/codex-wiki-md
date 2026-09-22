# Iterative lengthening search

↑ **Parent:** [Search algorithm](search-algorithm.md)

[Iterative lengthening search](iterative-lengthening-search.md) repeatedly runs [cost-bounded depth-first search](cost-bounded-depth-first-search.md), starting with threshold zero and replacing each unsuccessful threshold by the smallest rejected [path cost](path-cost.md). It uses a [depth-first search](depth-first-search.md) stack rather than the potentially large [search frontier](search-frontier.md) of [uniform-cost search](uniform-cost-search.md).

Suppose an optimal [plan](plan.md) has cost $C^*$ and each pass terminates. At every unsuccessful threshold $L<C^*$, some first rejected prefix of an optimal [plan](plan.md) has [path cost](path-cost.md) at most $C^*$. Therefore the next threshold is no larger than $C^*$. Any first returned [goal state](goal-state.md) has cost at most $C^*$ and hence exactly $C^*$. Finite [branching factor](branching-factor.md) and a positive lower bound on [step costs](step-cost.md) ensure that only finitely many [search nodes](search-node.md) precede that cost, giving completeness as well as optimality. With arbitrary real [step costs](step-cost.md), the threshold increments can be much smaller than the smallest [step cost](step-cost.md): the difference between two [path costs](path-cost.md) need not itself be a [step cost](step-cost.md).

## ↑ Ancestors (4)

1. [Search algorithm](search-algorithm.md)
2. [Algorithm](algorithm-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Cost-bounded depth-first search](cost-bounded-depth-first-search.md)
- [Iterative lengthening search](iterative-lengthening-search.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/artificial-intelligence/1/b/solution.md)
