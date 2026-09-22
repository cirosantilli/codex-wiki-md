<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Construct each possible winning line, then test whether one is contained in the player's occupancy [set](../../../../../set-split.md):

```
winningLines :: [Places]
winningLines =
  [[(r,c) | c <- [0..2]] | r <- [0..2]] ++
  [[(r,c) | r <- [0..2]] | c <- [0..2]] ++
  [[(i,i) | i <- [0..2]], [(i,2-i) | i <- [0..2]]]

won :: Places -> Bool
won ps = any (\line -> all (`elem` ps) line) winningLines
```

The [list comprehension](../../../../../list-comprehension.md) generates three rows, three columns and two diagonals. Each has exactly three coordinates; therefore `all` holds precisely when every coordinate of that line is occupied by this player. Taking `any` over the eight lines proves the win test correct.

## ↑ Ancestors (12)

1. [D](../d.md)
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
