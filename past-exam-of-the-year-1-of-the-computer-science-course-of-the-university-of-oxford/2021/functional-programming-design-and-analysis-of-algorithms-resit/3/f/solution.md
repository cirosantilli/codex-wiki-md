<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Generate a row while respecting the forbidden symbols in each column. Selection returns an element together with the still-available elements:
```
select :: [a] -> [(a,[a])]
select [] = []
select (x:xs) = (x,xs) : [(y,x:ys) | (y,ys) <- select xs]

row :: [Int] -> [[Int]] -> [[Int]]
row [] [] = [[]]
row remaining (used:otherColumns) =
  [x:rest | (x,available) <- select remaining,
            x `notElem` used,
            rest <- row available otherColumns]
row _ _ = []

latinPruned :: Int -> [[[Int]]]
latinPruned n
  | n < 0     = error "negative order"
  | otherwise = build n (replicate n [])
  where
    build 0 usedColumns = [[]]
    build remainingRows usedColumns =
      [r:rest | r <- row [1..n] usedColumns,
                rest <- build (remainingRows-1)
                              (zipWith (:) r usedColumns)]
```
The [invariant](../../../../../invariant-mathematics.md) of `row` is that `remaining` contains exactly the unused symbols of this row, while each member of the column [list](../../../../../list-abstract-data-type.md) records symbols used by earlier rows. Selecting removes a symbol, so it cannot repeat in the current row; the membership test prevents a column repetition. A complete row uses every symbol once. Updating the column histories preserves the [invariant](../../../../../invariant-mathematics.md) for the next [recursive call](../../../../../recursive-call.md).

Every complete generated square is therefore valid without a final filter. Conversely, take any valid target square: its next row passes every selection and column test, so [induction](../../../../../mathematical-induction.md) keeps a branch constructing that target. Distinct choices from the initially distinct symbols cannot generate the same square twice. Dead-end partial squares may still be explored; the method promises to avoid constructing complete invalid squares, not to foresee every future dead end. Independent enumeration gives 1, 2, 12 and 576 squares at orders one through four.

## ↑ Ancestors (12)

1. [F](../f.md)
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
