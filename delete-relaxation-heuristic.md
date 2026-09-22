# Delete-relaxation heuristic

↑ **Parent:** [Relaxation heuristic](relaxation-heuristic.md)

For positive-precondition [STRIPS](strips.md) with a positive conjunctive goal, remove every delete effect and use the exact shortest relaxed [plan](plan.md) cost. Every original [plan](plan.md) still succeeds in the relaxed model because facts can only accumulate, so its relaxed optimum is an [admissible heuristic](admissible-heuristic.md). The cost of an arbitrary relaxed [plan](plan.md) is an upper bound on the relaxed optimum and need not be an [admissible heuristic](admissible-heuristic.md) for the original problem.

## ↑ Ancestors (7)

1. [Relaxation heuristic](relaxation-heuristic.md)
2. [Search problem](search-problem.md)
3. [Computational problem](computational-problem.md)
4. [Computational complexity theory](computational-complexity-theory.md)
5. [Theoretical computer science](theoretical-computer-science-split.md)
6. [Computer science](computer-science-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2015/intelligent-systems/2/e/solution.md)
