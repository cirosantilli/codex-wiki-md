<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose the middle element as the root:
```
build :: [a] -> Tree a
build [] = Empty
build xs = Tree (build ls) x (build rs)
  where
    (ls,x:rs) = splitAt (length xs `div` 2) xs
```
The input is a finite, strictly ascending [list](../../../../../list-abstract-data-type.md), as required for distinct elements of a [set](../../../../../set-split.md). The two child lengths differ by at most one. Applying the same argument recursively gives a [balanced binary tree](../../../../../balanced-binary-tree.md) of logarithmic height. All values on each side retain their original order, proving the [binary search tree](../../../../../binary-search-tree.md) property. With linked lists, the repeated splitting gives $O(n\log n)$ time; it does not repeatedly insert values into a skewed tree.

## ↑ Ancestors (12)

1. [C](../c.md)
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
