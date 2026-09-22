<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The first tree's root is the first element. Deleting that root either discards a singleton or exposes two equal-sized child trees:
```
head :: List a -> a
head (List ((_,Leaf x):_))     = x
head (List ((_,Node x _ _):_)) = x
head (List []) = error "head: empty list"

tail :: List a -> List a
tail (List ((_,Leaf _):ts)) = List ts
tail (List ((w,Node _ l r):ts)) =
  let h = w `div` 2 in List ((h,l):(h,r):ts)
tail (List []) = error "tail: empty list"
```
For a node of size $w=2h+1$, both children have size $h$. Their order agrees with the old [preorder traversal](../../../../../preorder-traversal.md), and they become the sole permitted initial duplicate. The rest of the [forest](../../../../../forest.md) was no smaller than the old root tree. Thus both operations preserve the representation invariant and take **worst-case $O(1)$ time** on a nonempty [skew-binary random-access list](../../../../../skew-binary-random-access-list.md).

## ↑ Ancestors (12)

1. [F](../f.md)
2. [2](../../2.md)
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
