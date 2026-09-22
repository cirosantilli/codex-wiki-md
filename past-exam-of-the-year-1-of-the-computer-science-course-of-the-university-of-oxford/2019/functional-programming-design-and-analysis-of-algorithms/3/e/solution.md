<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Record the outcome at the first completed board and otherwise branch over every available move:

```
data Outcome = Winner Player | Draw deriving (Eq,Ord,Show)

finals :: Board -> [(Board,Outcome)]
finals b@(os,xs,es)
  | won os    = [(b,Winner O)]
  | won xs    = [(b,Winner X)]
  | null es   = [(b,Draw)]
  | otherwise = concatMap (\q -> finals (play b q)) es
```

The [recursion](../../../../../recursion-computer-science.md) terminates because each recursive call decreases the number of empty positions by one. For correctness, induct on that number. A completed board contributes exactly its own outcome. Otherwise every legal continuation has a unique first available move, and the induction hypothesis covers exactly all completions after that move. [List concatenation](../../../../../list-concatenation.md) collects these branches without extending completed games. Repeated final positions are allowed here because the computation deliberately explores every legal move sequence.

## ↑ Ancestors (12)

1. [E](../e.md)
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
