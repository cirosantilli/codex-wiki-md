<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Sort the two halves ascending, reverse the second, and concatenate to form a [bitonic sequence](../../../../../bitonic-sequence.md):
```
sort :: Ord a => [a] -> [a]
sort []  = []
sort [x] = [x]
sort xs  = merge (sort as ++ reverse (sort bs))
  where (as,bs) = halve xs
```
For a power-of-two length greater than one, both halves are smaller powers of two. By [induction](../../../../../mathematical-induction.md), the recursive calls return ascending [permutations](../../../../../permutation.md) of their respective inputs. Reversal makes the second half descending, so part (e)'s precondition holds and `merge` sorts their concatenation without losing entries. This proves both [sortedness](../../../../../sortedness.md) and [sorting permutation preservation](../../../../../sorting-permutation-preservation.md). Its [recurrence relation](../../../../../recurrence-relation.md) is $T(n)=2T(n/2)+\Theta(n\log n)$, so summing the levels gives **$\Theta(n(\log n)^2)$ time**. Equal keys cause no difficulty; ascending and descending here permit equality. This is a [bitonic sorting algorithm](../../../../../bitonic-sorting-algorithm.md).

## ↑ Ancestors (12)

1. [F](../f.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
