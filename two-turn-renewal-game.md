# Two-turn renewal game

↑ **Parent:** [First-step analysis](first-step-analysis.md)

Suppose each independent turn makes the current player win with [probability](probability.md) $p$, lose with probability $q$, or pass with probability $r$, with $p+q+r=1$ and $r<1$. The players have identical turn rules and alternate after a pass. Before the first pair of turns finishes, the starting player wins with probability $p+rq$. Passing twice returns to the initial state with probability $r^2$. [First-step analysis](first-step-analysis.md) therefore gives $P=p+rq+r^2P$, proving the formula. The [geometric series](geometric-series.md) of repeated restarts converges because $r<1$; infinite play has probability zero. For $r=1$, nobody ever wins, so that excluded case has no eventual winning probability summing to one.

## ↑ Ancestors (5)

1. [First-step analysis](first-step-analysis.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1/7/b/iii/solution.md)
