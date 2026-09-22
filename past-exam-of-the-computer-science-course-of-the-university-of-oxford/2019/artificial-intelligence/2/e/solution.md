<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

**The depth assertion is false.** Each move occupies one new square, so the general bound is $n^2$, not $n$. On a $2\times2$ board no knights attack, and a play has four moves. More generally, filling a single checkerboard colour gives a legal partial play of length $\lceil n^2/2\rceil$, since knight moves always change colour.

**The opponent-independent “best possible move” assertion is false.** [Minimax search](../../../../../minimax-search.md) maximizes the guaranteed [utility](../../../../../utility.md) against an opponent choosing the worst continuation. It need not maximize the outcome against a particular weaker opponent. If a winning [strategy](../../../../../strategy-in-an-infinite-game.md) is available, its guaranteed win cannot be improved on in win/loss utility; if every root move loses against perfect play, all have the same minimax value, yet some may exploit a weaker opponent better. Thus the valid universal statement is that a minimax [strategy](../../../../../strategy-in-an-infinite-game.md) guarantees its minimax value, not that its root choice is best for every possible opponent behavior.[§3.2, opening assumption: the opponent chooses the move worst for the agent](../../../../../cs-188-minimax-notes.md)

**The $O(n)$ storage assertion is false for the usual minimax implementation.** Here the maximum [branching factor](../../../../../branching-factor.md) is $O(n^2)$ and maximum depth is $O(n^2)$. A conventional [depth-first search](../../../../../depth-first-search.md) retaining pending successors uses the usual $O(bm)=O(n^4)$ search-node bound. Generating successors lazily and applying/undoing moves in one board can reduce this to $O(n^2)$ stack frames plus board storage; neither accounting should confuse the board side length $n$ with its $n^2$ squares.

**The winning-strategy assertion is true.** The game is finite, has perfect information, alternates two players, and has no draw under the [normal-play convention](../../../../../normal-play-convention.md). A terminal position is losing for the player to move. By [backward induction](../../../../../backward-induction.md), a nonterminal position is winning exactly when at least one legal move reaches a losing position; otherwise it is losing. This labels every position, including the initial board, so exactly one of the two players has a winning [strategy](../../../../../strategy-in-an-infinite-game.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
