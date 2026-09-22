<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In a [preorder traversal](../../../../../preorder-traversal.md), visit the root before the left [subtree](../../../../../subtree.md), then visit the right [subtree](../../../../../subtree.md). The `NIL` test prevents visiting or dereferencing an empty [binary tree](../../../../../binary-tree.md):

```
PROCEDURE preorder(t : node);
BEGIN
  IF t # NIL THEN
    visit(t);
    preorder(t.left);
    preorder(t.right)
  END
END preorder;
```

[Structural induction](../../../../../structural-induction.md) proves correctness. The empty [binary tree](../../../../../binary-tree.md) has nothing to visit. For a nonempty root, `visit(t)` comes first; by the [induction hypothesis](../../../../../induction-hypothesis.md), each recursive call visits exactly its own [subtree](../../../../../subtree.md) in [preorder traversal](../../../../../preorder-traversal.md) order, and the left call finishes before the right begins. Each recursive call receives a strictly smaller finite [tree](../../../../../tree-graph-theory-split.md), proving termination. Assuming `visit` neither changes the child links nor fails to return, the procedure therefore realizes

$$
\boxed{\operatorname{preorder}(t)=t,\ \operatorname{preorder}(t.left),\ \operatorname{preorder}(t.right).}
$$

For $m$ nodes, overhead is $\Theta(m+1)$ and [recursion](../../../../../recursion-computer-science.md) depth is $O(h+1)$ for height $h$, in addition to the cost of `visit`. The claim presumes an actual [binary tree](../../../../../binary-tree.md); cycles or shared nodes in an arbitrary pointer [graph](../../../../../graph-split.md) need additional handling if each object is to be visited exactly once.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
