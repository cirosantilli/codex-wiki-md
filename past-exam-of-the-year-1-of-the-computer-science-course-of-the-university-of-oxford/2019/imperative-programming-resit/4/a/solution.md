<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Treat a null reference as the empty [binary tree](../../../../../binary-tree.md) and perform the visit before descending:
```
def preorderRecursive(t: Tree): Unit = {
  if (t != null) {
    println(t.datum)
    preorderRecursive(t.left)
    preorderRecursive(t.right)
  }
}
```
By [structural induction](../../../../../structural-induction.md), the empty [binary tree](../../../../../binary-tree.md) produces the empty output. A nonempty [binary tree](../../../../../binary-tree.md) prints its root label, then the complete [preorder traversal](../../../../../preorder-traversal.md) of the left [subtree](../../../../../subtree.md), then that of the right [subtree](../../../../../subtree.md). These are exactly the required output positions. The [recursion](../../../../../recursion-computer-science.md) terminates on a finite [binary tree](../../../../../binary-tree.md) because each recursive call has strictly fewer [vertices](../../../../../vertex-graph-theory.md). For the three-node example, **the output order is $2,1,3$**. The [time complexity](../../../../../time-complexity.md) is linear in the number of [vertices](../../../../../vertex-graph-theory.md), with [call stack](../../../../../call-stack.md) depth bounded by the [height of a binary tree](../../../../../height-of-a-binary-tree.md) plus a constant.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Imperative programming resit](../../../imperative-programming-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
