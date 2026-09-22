<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [merge sort](../../../../../merge-sort.md), then project the second component of each [pair](../../../../../pair.md). Under the ordinary [Haskell Ord class](../../../../../haskell-ord-class.md) instance for pairs, “ascending” means [lexicographic order](../../../../../lexicographic-order.md), requiring both component types to be ordered:
```
sort :: (Ord a, Ord b) => [(a,b)] -> [b]
sort = map snd . mergeSort

mergeSort :: Ord a => [a] -> [a]
mergeSort [] = []
mergeSort [x] = [x]
mergeSort xs = merge (mergeSort left) (mergeSort right)
  where (left,right) = splitAt (length xs `div` 2) xs

merge :: Ord a => [a] -> [a] -> [a]
merge [] ys = ys
merge xs [] = xs
merge (x:xs) (y:ys)
  | x <= y    = x : merge xs (y:ys)
  | otherwise = y : merge (x:xs) ys
```
If the intended convention is to sort only by the first component as a [sort key](../../../../../sort-key.md), replace `x <= y` by `fst x <= fst y` and specialize the merge routines to pairs. The weaker signature is then `sort :: Ord a => [(a,b)] -> [b]`, and equal keys keep their original order. These conventions differ when first components tie; the question does not explicitly specify that tie rule.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
