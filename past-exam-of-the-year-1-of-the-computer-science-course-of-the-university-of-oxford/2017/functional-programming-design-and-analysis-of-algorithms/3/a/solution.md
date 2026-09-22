<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Using only [list comprehensions](../../../../../list-comprehension.md):

```
type Matrix a = [[a]]
type Grid = Matrix Int

choicesComp :: Grid -> Matrix [Int]
choicesComp rows =
  [[[d | d <- [1..9], n == 0 || d == n] | n <- row] | row <- rows]
```

The input contract restricts each cell to zero or a digit from one to nine. A definition using standard list functions is:

```
choicesMap :: Grid -> Matrix [Int]
choicesMap = map (map choice)
  where
    choice :: Int -> [Int]
    choice 0 = [1..9]
    choice n = [n]

choices :: Grid -> Matrix [Int]
choices = choicesMap
```

Both preserve the row structure and construct the initial [constraint domains](../../../../../constraint-domain.md) of the [Sudoku](../../../../../sudoku.md) problem. The alternative names let both definitions coexist; either can supply `choices`.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
