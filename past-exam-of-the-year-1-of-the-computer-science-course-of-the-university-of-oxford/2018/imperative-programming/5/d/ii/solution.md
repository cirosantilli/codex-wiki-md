<h1 id="5/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Perform a [destructive binary search tree flattening](../../../../../../destructive-binary-search-tree-flattening.md) by converting both child [subtrees](../../../../../../subtree.md) and splicing their endpoints around the original root:
```
def flatten(t: Tree): (Tree, Tree) = {
  if (t == null) (null, null)
  else {
    val oldLeft = t.left
    val oldRight = t.right
    val (ls, le) = flatten(oldLeft)
    val (rs, re) = flatten(oldRight)
    t.left = le
    if (le != null) le.right = t
    t.right = rs
    if (rs != null) rs.left = t
    val start = if (ls == null) t else ls
    val end = if (re == null) t else re
    (start, end)
  }
}
```
Save the child references before changing their interpretation. The input is a finite [binary search tree](../../../../../../binary-search-tree.md) satisfying part (b), and no external client may simultaneously rely on the old tree links. By [structural induction](../../../../../../structural-induction.md), the two [recursive calls](../../../../../../recursive-call.md) return disjoint, ordered [doubly linked lists](../../../../../../doubly-linked-list.md) containing exactly their original entries. The [binary search tree](../../../../../../binary-search-tree.md) bounds place every left word before `t.word` and every right word after it. Splicing the left end, `t`, and the right start therefore preserves strict order and reciprocal links. A missing left list makes `t.left` null and `t` the start; a missing right list similarly makes `t` the end. The resulting outside links are null as required by part (i).

The recursive [loop variant](../../../../../../loop-variant.md) analogue is the strictly smaller number of entries in each child [subtree](../../../../../../subtree.md). Every entry is processed once and incurs a constant number of link writes, so [time complexity](../../../../../../time-complexity.md) is $O(n+1)$ and recursion uses $O(h+1)$ [auxiliary space](../../../../../../auxiliary-space.md). **No new `Tree` entry is created**; returning endpoint [tuples](../../../../../../finite-tuple.md) and using a call [stack](../../../../../../stack-data-structure.md) are permitted auxiliary storage. The old [binary search tree](../../../../../../binary-search-tree.md) representation is consumed by this operation.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [5](../../../5.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
