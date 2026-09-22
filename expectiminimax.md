# Expectiminimax

↑ **Parent:** [Adversarial search](adversarial-search.md)

[Backward induction](backward-induction.md) on a finite [game tree](game-tree.md) containing maximizing choices, minimizing choices and [chance nodes](chance-node.md). Terminal [utilities](utility.md) are backed up by $\max$, $\min$ and $\sum_jp_jV_j$, respectively. Exact [chance node](chance-node.md) evaluation generally needs every positive-[probability](probability.md) outcome; ordinary [alpha-beta pruning](alpha-beta-pruning.md) does not transfer unchanged because one child's value does not bound the full weighted sum.

## ↑ Ancestors (7)

1. [Adversarial search](adversarial-search.md)
2. [Search problem](search-problem.md)
3. [Computational problem](computational-problem.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/3/d/solution.md)
