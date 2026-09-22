<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [utilities](../../../../../utility.md) from A's viewpoint, with A maximizing and B minimizing. The following [alpha-beta pruning](../../../../../alpha-beta-pruning.md) code assumes a finite horizon or terminating [game tree](../../../../../game-tree.md); leaf evaluation uses terminal [utility](../../../../../utility.md) when available and a specified horizon estimate otherwise.

```
ALPHABETA(state, depth, alpha, beta, maximizing):
    if state is terminal or depth == 0:
        return EVALUATE(state)
    if maximizing:
        value := -infinity
        for child in SUCCESSORS(state):
            value := max(value, ALPHABETA(child, depth-1, alpha, beta, false))
            alpha := max(alpha, value)
            if alpha >= beta: break
        return value
    else:
        value := +infinity
        for child in SUCCESSORS(state):
            value := min(value, ALPHABETA(child, depth-1, alpha, beta, true))
            beta := min(beta, value)
            if alpha >= beta: break
        return value
```

Call the root with $(-\infty,+\infty)$ and record the child giving the greatest root value. In a nonterminal game state, SUCCESSORS must supply the game's legal moves, including any mandatory pass; a player with no moves must be handled according to the rules rather than left as an accidental empty loop.

The bound $\alpha$ records an outcome already available to MAX on the active ancestor path; $\beta$ records one already available to MIN. At a MIN node, once a child gives value at most $\alpha$, further children can only decrease the node's minimum, so MAX need not choose that branch. The dual argument applies at MAX when its current value is at least $\beta$. Returned values from cut-off subtrees can be bounds rather than exact local [minimax search](../../../../../minimax-search.md) values, while the unrestricted root value is exact. Equal-value pruning preserves that value; retaining the first best root action gives a fixed tie rule.[§3.2.1, Alpha-Beta Pruning: ancestor alternatives and cutoffs](../../../../../cs-188-minimax-notes.md)

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
