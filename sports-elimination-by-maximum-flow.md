# Sports elimination by maximum flow

↑ **Parent:** [Maximum flow problem](maximum-flow-problem.md)

For a league in which every remaining game gives exactly one win, first give the target team all its remaining wins, obtaining $W$. Make a node for each unordered pair of other teams, with source capacity equal to their remaining games. Route each game-node flow to one of its two teams, and cap the team's total additional wins at $W-w_i-1$ for a strict target victory. A negative cap immediately rules out success. Otherwise an integral [maximum flow](maximum-flow-problem.md) saturating every game-source arc specifies the winners of all games and proves feasibility. Each actual game is counted once; duplicating ordered pairs changes the problem.

## ↑ Ancestors (7)

1. [Maximum flow problem](maximum-flow-problem.md)
2. [Flow network](flow-network.md)
3. [Graph theory](graph-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33/2/solution.md)
