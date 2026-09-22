<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Push the right child before the left child so that the [LIFO stack](../../../../../stack-data-structure.md) exposes the left child first:
```
def preorderIterative(t: Tree): Unit = {
  val pending = new Stack
  if (t != null) pending.push(t)
  while (!pending.isEmpty) {
    val u = pending.pop
    println(u.datum)
    if (u.right != null) pending.push(u.right)
    if (u.left != null) pending.push(u.left)
  }
}
```
Let $P(u)$ be the [sequence](../../../../../sequence.md) of labels in the [preorder traversal](../../../../../preorder-traversal.md) of $u$. If the abstract pending [stack](../../../../../stack-data-structure.md), top first, is $[u_1,\ldots,u_k]$, the [loop invariant](../../../../../loop-invariant.md) is that the output already printed, followed by $P(u_1)\mathbin{+\!+}\cdots\mathbin{+\!+}P(u_k)$, is the required full output. Each pending root is non-null, and its [subtree](../../../../../subtree.md) is still unvisited. This is the pending-work form of [explicit-stack depth-first tree traversal](../../../../../explicit-stack-depth-first-tree-traversal.md).

One iteration discharges the first root's own label and replaces its remaining obligation by the left [subtree](../../../../../subtree.md) followed by the right [subtree](../../../../../subtree.md). The push order makes that precisely the new top-first pending order. Thus the [loop invariant](../../../../../loop-invariant.md) is preserved. The [loop variant](../../../../../loop-variant.md) is the sum of the numbers of [vertices](../../../../../vertex-graph-theory.md) in all pending [subtrees](../../../../../subtree.md); it decreases by exactly one per iteration, even if the number of [stack](../../../../../stack-data-structure.md) entries increases. When the [stack](../../../../../stack-data-structure.md) is empty there is no remaining output obligation, proving correctness and termination. This assumes a finite genuine [binary tree](../../../../../binary-tree.md) and, as permitted, sufficient [stack](../../../../../stack-data-structure.md) capacity. Each [vertex](../../../../../vertex-graph-theory.md) is pushed and popped once, giving **$\Theta(n)$ time** and $O(h+1)$ pending references for [binary tree](../../../../../binary-tree.md) height $h$.

## ↑ Ancestors (12)

1. [C](../c.md)
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
