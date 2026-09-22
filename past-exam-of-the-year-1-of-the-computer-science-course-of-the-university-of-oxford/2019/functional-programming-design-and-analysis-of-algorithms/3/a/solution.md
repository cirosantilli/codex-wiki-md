<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use coordinates with row and column in $\{0,1,2\}$:

```
type Place  = (Int,Int)
type Places = [Place]
type Board  = (Places,Places,Places)
data Player = O | X deriving (Eq,Ord,Show)
```

The components of `Board` record the positions occupied by `O`, occupied by `X`, and still empty, respectively. On a nonterminal legal board, **equal occupied counts mean `O` moves next; one extra `O` means `X` moves next**.

The [type synonym](../../../../../type-synonym.md) does not enforce the [representation invariant](../../../../../representation-invariant.md): coordinates are in range; each component has no duplicates; the three represented [sets](../../../../../set-split.md) form a [set partition](../../../../../set-partition.md) of the nine positions; and the occupied counts differ as just described. Both players cannot have won. A winning `O` board has one extra `O`, and a winning `X` board has equal counts. More fundamentally, a legal [tic-tac-toe](../../../../../tic-tac-toe.md) state has a legal alternating history that stops at the first win: satisfying a type alone never licenses continuing an already completed game.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
