<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Fold into a membership [predicate](../../../../../predicate.md):
```
find :: Ord a => Tree a -> a -> Bool
find = foldTree node (const False)
  where
    node left x right q = case compare q x of
      LT -> left q
      EQ -> True
      GT -> right q
```
At an empty tree the [predicate](../../../../../predicate.md) is always false. At a nonempty [binary search tree](../../../../../binary-search-tree.md), an unequal query can occur only in the indicated child, while equality finds the root. This proves correctness inductively. Under [lazy evaluation](../../../../../lazy-evaluation.md), the unused folded child is not demanded; lookup follows one root-to-leaf route and takes $O(h+1)$ comparisons in a tree of height $h$. Defining the [predicate](../../../../../predicate.md) by a fold does not require visiting both subtrees for each query.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
