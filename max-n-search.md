# Max-n search

↑ **Parent:** [Game tree](game-tree.md)

[Backward induction](backward-induction.md) with an $n$-component [utility](utility.md) vector. At a node controlled by player $i$, evaluate each child, choose a child maximizing coordinate $i$ and copy its entire vector. A fixed tie rule makes the returned vector well defined. By [mathematical induction](mathematical-induction.md) from terminal positions, the selected continuation is a best response at every node of a finite [perfect-information game](perfect-information-game.md), giving a [pure strategy](pure-strategy.md) [subgame perfect equilibrium](subgame-perfect-equilibrium.md). The vector must be copied intact; separate coordinatewise maxima need not describe any attainable outcome.

**Table of contents**

- [Nearly-zero-sum pruning](nearly-zero-sum-pruning.md)

## ↑ Ancestors (6)

1. [Game tree](game-tree.md)
2. [Game theory](game-theory-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [General-sum game](general-sum-game.md)
- [Nearly-zero-sum pruning](nearly-zero-sum-pruning.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/3/e/solution.md)
- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2020/artificial-intelligence/3/g/solution.md)
