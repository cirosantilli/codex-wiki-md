# Forward state-space planning

↑ **Parent:** [Classical planning](classical-planning.md)

Expand a concrete state by applying every action whose [preconditions](precondition.md) hold, and search the resulting state [graph](graph-split.md) for a goal. For [STRIPS](strips.md), the successor is $(S\setminus\operatorname{Del}(a))\cup\operatorname{Add}(a)$. A valid expansion checks the complete [precondition](precondition.md) set, including resource markers such as an empty hand, rather than only an action's geometric destination.

## ↑ Ancestors (5)

1. [Classical planning](classical-planning.md)
2. [Automated planning](automated-planning.md)
3. [Artificial intelligence](artificial-intelligence-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2021/artificial-intelligence/3/b/solution.md)
