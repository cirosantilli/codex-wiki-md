<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The following [predicate](../../../../../predicate.md) also checks the square's shape; `sort` is the three-way sorting [function](../../../../../function-split.md) from Question 2:
```
valid :: [[Int]] -> Bool
valid rows =
  let n = length rows
      symbols = [1..n]
      goodRows = all (\r -> sort r == symbols) rows
      goodColumns = all (\j -> sort [r !! j | r <- rows] == symbols)
                        [0..n-1]
  in goodRows && goodColumns

latin :: Int -> [[[Int]]]
latin = filter valid . squares
```
The row tests guarantee that each row has length $n$ and contains each allowed symbol once. Because `&&` tests this condition first, the later column indexing is safe for a finite total input. The column tests establish the remaining Latin-square condition. Filtering therefore retains precisely the valid squares; it does not remove any different ordering of rows, columns or symbols as an alleged symmetry duplicate.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
