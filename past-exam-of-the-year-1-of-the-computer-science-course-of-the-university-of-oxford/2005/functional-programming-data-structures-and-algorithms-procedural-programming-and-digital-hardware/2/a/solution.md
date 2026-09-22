<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $m,n$ be the two input lengths and suppose numeric comparisons cost constant time. The [list-based set representation](../../../../../list-based-set-representation.md) determines which [representation invariant](../../../../../representation-invariant.md) each answer must preserve.

For unsorted [lists](../../../../../list-abstract-data-type.md) allowing repetition, retain every left-hand occurrence whose value appears on the right for [set intersection](../../../../../set-intersection.md), and use [list concatenation](../../../../../list-concatenation.md) for [set union](../../../../../set-union.md):

```
interR xs ys = [x | x <- xs, x `elem` ys]
unionR xs ys = xs ++ ys
```

The resulting [lists](../../../../../list-abstract-data-type.md) represent exactly the desired [sets](../../../../../set-split.md); repeated entries are permitted. Membership by [sequential search](../../../../../linear-search.md) makes `interR` take $O(mn)$ [time complexity](../../../../../time-complexity.md) in the worst case. The [list concatenation](../../../../../list-concatenation.md) in `unionR` costs $O(m)$ to build its copied left spine and shares `ys`; fully enumerating the resulting [list](../../../../../list-abstract-data-type.md) costs $O(m+n)$.

For unsorted, duplicate-free inputs, the same intersection keeps uniqueness, while the union retains `xs` and appends only right-hand elements absent from `xs`:

```
interU xs ys = [x | x <- xs, x `elem` ys]
unionU xs ys = xs ++ [y | y <- ys, not (y `elem` xs)]
```

Neither filtered [list](../../../../../list-abstract-data-type.md) has internal repetitions, and the filter in `unionU` also excludes overlap with `xs`. Both operations have worst-case $O(mn+m+n)$ [time complexity](../../../../../time-complexity.md), customarily written $O(mn)$ when both lengths are positive. Using the original `xs` for each membership test avoids searching an ever-growing output.

For sorted, duplicate-free [lists](../../../../../list-abstract-data-type.md), compare only the two current heads:

```
interS [] ys = []
interS xs [] = []
interS (x:xs) (y:ys)
  | x < y = interS xs (y:ys)
  | x > y = interS (x:xs) ys
  | otherwise = x : interS xs ys

unionS [] ys = ys
unionS xs [] = xs
unionS (x:xs) (y:ys)
  | x < y = x : unionS xs (y:ys)
  | x > y = y : unionS (x:xs) ys
  | otherwise = x : unionS xs ys
```

When $x<y$, sortedness proves that $x$ cannot occur anywhere in the right [list](../../../../../list-abstract-data-type.md), so it can be discarded from the [set intersection](../../../../../set-intersection.md) or immediately emitted to the [set union](../../../../../set-union.md). The symmetric argument handles $y<x$; equal heads are consumed together. Each step consumes at least one input head, so both have $O(m+n)$ worst-case [time complexity](../../../../../time-complexity.md). These bounds assume the sorted [representation invariant](../../../../../representation-invariant.md) is already established; sorting arbitrary inputs has its own cost.

| Representation | [Set intersection](../../../../../set-intersection.md) | [Set union](../../../../../set-union.md), including output traversal |
| --- | --- | --- |
| Unsorted, repetitions allowed | $O(mn+m+n)$ | $O(m+n)$ |
| Unsorted, unique | $O(mn+m+n)$ | $O(mn+m+n)$ |
| Sorted, unique | $O(m+n)$ | $O(m+n)$ |

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
