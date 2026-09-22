<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Give the visiting procedure a [procedure type](../../../../../procedure-type.md):
```
TYPE Visit = PROCEDURE(x: INTEGER);

PROCEDURE Inorder(t: Tree; p: Visit);
BEGIN
  IF t # NIL THEN
    Inorder(t.left, p);
    p(t.label);
    Inorder(t.right, p)
  END
END Inorder;
```
[Structural induction](../../../../../structural-induction.md) establishes [algorithm correctness](../../../../../algorithm-correctness.md): an empty [binary tree](../../../../../binary-tree.md) makes no calls; otherwise the first [recursive call](../../../../../recursive-call.md) visits precisely the left [subtree](../../../../../subtree.md), then the root is visited once, then the second [recursive call](../../../../../recursive-call.md) visits precisely the right [subtree](../../../../../subtree.md). Assume `p` does not modify the [binary tree](../../../../../binary-tree.md). With constant-cost `p`, there is constant work per node and empty child occurrence:

$$
\boxed{T(n)=\Theta(n+1),\qquad\text{auxiliary storage }O(h+1),}
$$

where $h$ is the [height of a binary tree](../../../../../height-of-a-binary-tree.md) and storage is the [call stack](../../../../../call-stack.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
