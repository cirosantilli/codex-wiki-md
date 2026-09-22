<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the empty reference as the [base case](../../../../../base-case.md):
```
def printInorder(root: Tree): Unit = {
  if (root != null) {
    printInorder(root.left)
    println(root.datum)
    printInorder(root.right)
  }
}
```
[Induction](../../../../../mathematical-induction.md) on the tree proves the order: the first [recursive call](../../../../../recursive-call.md) prints exactly the left [subtree](../../../../../subtree.md), then the procedure prints the root, then the final call prints exactly the right [subtree](../../../../../subtree.md). A finite acyclic tree supplies decreasing proper [subtrees](../../../../../subtree.md), so the [recursion](../../../../../recursion-computer-science.md) terminates. The traversal is valid for arbitrary [integer](../../../../../integer-split.md) labels; sorted output would additionally require a [binary search tree](../../../../../binary-search-tree.md) [invariant](../../../../../invariant-mathematics.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
