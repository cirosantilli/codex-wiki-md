<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**[Minimax search](../../../../../minimax-search.md) applies because this is a finite, deterministic two-player [zero-sum game](../../../../../zero-sum-game.md) with perfect information.** Each move assigns a previously unassigned [Boolean variable](../../../../../boolean-variable.md), so play terminates after exactly $N$ moves. Both players observe the whole partial [Boolean valuation](../../../../../boolean-valuation.md), and there are no chance moves. Give terminal positions [payoff](../../../../../payoff.md) $+1$ when the [propositional formula](../../../../../propositional-formula.md) is true and $-1$ when it is false, measured for $A$. At an $A$-node take the maximum child value and at a $B$-node the minimum. [Backward induction](../../../../../backward-induction.md) then computes the winner and a corresponding [winning strategy](../../../../../winning-strategy-in-an-infinite-game.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2021](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
