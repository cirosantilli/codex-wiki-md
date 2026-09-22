<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Store the equal bucket at each internal node:
```
data Tree a = Empty | Node (Tree a) [a] (Tree a)

toTree :: Ord a => [a] -> Tree a
toTree [] = Empty
toTree (pivot:xs) =
  let (lo,eq,hi) = partition3 pivot xs
  in Node (toTree lo) (pivot:eq) (toTree hi)

fromTree :: Tree a -> [a]
fromTree Empty = []
fromTree (Node left equal right) =
  fromTree left ++ equal ++ fromTree right
```
The representation [invariant](../../../../../invariant-mathematics.md) for a tree produced by `toTree` is that its bucket is nonempty and contains equal keys, every left-subtree key is smaller, and every right-subtree key is larger. Its multiplicities are preserved. Substituting the two equations for `toTree` into `fromTree` gives exactly the two defining equations for `sort`; [induction](../../../../../mathematical-induction.md) proves **`sort = fromTree . toTree`** on finite inputs.

Both versions call the same partition helper on the same pivot and sublists. The flattening stage makes no key comparisons. Thus fully producing the answer makes the same comparison decisions as the direct [algorithm](../../../../../algorithm-split.md); no additional comparison against stored tree keys is introduced.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
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
