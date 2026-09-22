<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Choose the first unclassified element as the next [equivalence class representative](../../../../../equivalence-class-representative.md):
```
equiv :: Eq a => [a] -> [[a]]
equiv [] = []
equiv (x:xs) = (x:same) : equiv rest
  where ~(same,rest) = partition (== x) xs
```
Assume the `Eq` instance is an [equivalence relation](../../../../../equivalence-relation.md). The [stable list partition](../../../../../stable-list-partition.md) collects every later occurrence equivalent to `x`, and `rest` contains none of that [equivalence class](../../../../../equivalence-class.md). [Induction](../../../../../mathematical-induction.md) therefore gives exactly one group per class, preserving order within each group and ordering groups by their first occurrence. For $d$ distinct classes, each input element is tested against at most $d$ representatives: the cost is $O(nd)$ and **$\Theta(n^2)$ in the all-distinct worst case**; a single class takes $\Theta(n)$.

The [equality-only grouping lower bound](../../../../../equality-only-grouping-lower-bound.md) shows that this worst case is unavoidable in the unrestricted equality-oracle model. On an all-distinct input, an untested pair could instead be equal without changing any observed comparison. Certifying that all $n$ elements belong to different classes therefore requires all $\binom n2$ pairwise [equality tests](../../../../../equality-test.md).

## ↑ Ancestors (12)

1. [F](../f.md)
2. [3](../../3.md)
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
