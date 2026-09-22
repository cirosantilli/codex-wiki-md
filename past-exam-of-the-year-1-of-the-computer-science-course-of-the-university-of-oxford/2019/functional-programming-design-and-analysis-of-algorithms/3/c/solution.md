<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume the board satisfies the [representation invariant](../../../../../representation-invariant.md). Reject completed boards and occupied or out-of-range coordinates; testing membership in the empty component covers both coordinate failures.

```
finished :: Board -> Bool
finished (os,xs,es) = won os || won xs || null es

play :: Board -> Place -> Board
play b@(os,xs,es) q
  | finished b     = error "play: completed game"
  | q `notElem` es = error "play: unavailable place"
  | length os == length xs = (q:os,xs,rest)
  | otherwise             = (os,q:xs,rest)
  where rest = filter (/=q) es
```

Here `won` is defined in part d. Moving one available coordinate into the appropriate occupied component preserves the [set partition](../../../../../set-partition.md) and the alternating-count rule. Checking completion first preserves the no-moves-after-a-win invariant.

## ↑ Ancestors (12)

1. [C](../c.md)
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
