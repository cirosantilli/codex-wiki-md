<h1 id="4/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Merge by comparing the present heads and consuming just the chosen one. The implementation uses only the functional representation:
```
merge' :: Ord a => List a -> List a -> List a
merge' left right
  | null' left  = right
  | null' right = left
  | head' left <= head' right =
      cons' (head' left) (merge' (tail' left) right)
  | otherwise =
      cons' (head' right) (merge' left (tail' right))

mergeSort' :: Ord a => List a -> List a
mergeSort' input =
  let n = length' input
      middle = n `div` 2
  in if n <= 1 then input
     else merge' (mergeSort' (take' middle input))
                 (mergeSort' (drop' middle input))
```
The two recursive inputs are the disjoint initial and final portions of the represented [sequence](../../../../../sequence.md); they preserve every occurrence and have smaller lengths when $n\geq2$. In `merge'`, the smaller current head can precede every remaining value in both sorted inputs. Selecting the left head on equality preserves stability. Each merge step reduces the total number of remaining elements, and [induction](../../../../../mathematical-induction.md) proves a sorted [permutation](../../../../../permutation.md) of the original [sequence](../../../../../sequence.md).

This establishes [algorithm termination](../../../../../algorithm-termination.md) and correctness on total finite representations, not an unconditional $O(n\log n)$ implementation bound. Nested index [functions](../../../../../function-split.md) can make queries costly, and repeatedly finding lengths or heads may revisit them. The familiar merge-sort bound assumes suitable constant-time access or consumption primitives; the source's [function](../../../../../function-split.md)-only representation supplies no such cost guarantee.

## ↑ Ancestors (12)

1. [G](../g.md)
2. [4](../../4.md)
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
