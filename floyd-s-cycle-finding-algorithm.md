<h1 id="floyd-s-cycle-finding-algorithm">Floyd's cycle-finding algorithm</h1>

↑ **Parent:** [Algorithm](algorithm-split.md)

For a deterministic iteration $x_{n+1}=f(x_n)$ on a [finite set](finite-set.md), move one pointer by one step and another by two steps. They eventually meet inside the repeated cycle. Restarting one pointer at the initial state and advancing both by one step locates the cycle entrance; a further traversal measures its length. The method uses constant extra [space complexity](space-complexity.md) and time proportional to the preperiod plus cycle length.

## ↑ Ancestors (3)

1. [Algorithm](algorithm-split.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Cycle detection](cycle-detection.md)
- [Pollard's rho algorithm](pollard-s-rho-algorithm.md)
