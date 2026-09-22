<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Insert down the unique search route, leaving equal elements unchanged:
```
insert :: Ord a => a -> Tree a -> Tree a
insert q Empty = Tree Empty q Empty
insert q t@(Tree l x r) = case compare q x of
  LT -> Tree (insert q l) x r
  EQ -> t
  GT -> Tree l x (insert q r)
```
The [binary search tree](../../../../../binary-search-tree.md) ordering determines the only child in which a missing query can belong. The recursive call preserves that child's ordering bounds, and the other child is shared. Thus the output represents the original [set](../../../../../set-split.md) with `q` added, with duplicates suppressed. Its [time complexity](../../../../../time-complexity.md) and newly allocated route length are $O(h+1)$; it makes no balancing guarantee.

## ↑ Ancestors (12)

1. [F](../f.md)
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
