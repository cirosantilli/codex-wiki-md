# Heuristic dominance

↑ **Parent:** [Heuristic function](heuristic-function.md)

A [heuristic function](heuristic-function.md) $h_2$ dominates $h_1$ if $h_2(s)\ge h_1(s)$ everywhere. When both are [admissible heuristics](admissible-heuristic.md), the larger estimate is at least as informative for [A-star search](a-star-search.md): for a fixed accumulated path cost $g$ and optimal solution cost $C^*$, $g+h_2<C^*$ implies $g+h_1<C^*$. This compares the compulsory search region, not arbitrary tie handling at $C^*$, evaluation overhead or wall-clock time.

## ↑ Ancestors (7)

1. [Heuristic function](heuristic-function.md)
2. [Search problem](search-problem.md)
3. [Computational problem](computational-problem.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Admissible heuristic combination](admissible-heuristic-combination.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/intelligent-systems/1/f/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2022/artificial-intelligence/2/e/solution.md)
