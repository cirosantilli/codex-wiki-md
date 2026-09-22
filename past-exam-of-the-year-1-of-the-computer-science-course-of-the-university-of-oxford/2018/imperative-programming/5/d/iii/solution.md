<h1 id="5/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Replace suspended [recursive calls](../../../../../../recursive-call.md) by an explicit [stack](../../../../../../stack-data-structure.md) for an [inorder traversal](../../../../../../inorder-traversal.md). Save each original right child before overwriting that link:
```
def flattenIterative(): (Tree, Tree) = {
  val pending = new scala.collection.mutable.Stack[Tree]
  var current = root
  var start: Tree = null
  var end: Tree = null
  while (current != null || pending.nonEmpty) {
    while (current != null) {
      pending.push(current)
      current = current.left
    }
    val t = pending.pop()
    val nextSubtree = t.right
    t.left = end
    if (end == null) start = t else end.right = t
    t.right = null
    end = t
    current = nextSubtree
  }
  root = null
  (start, end)
}
```
The method belongs to the concrete class owning `root`. Clearing `root` records that ownership has transferred to the returned [doubly linked list](../../../../../../doubly-linked-list.md); callers retain both returned endpoints. The inner [loop invariant](../../../../../../loop-invariant.md) says that the current [subtree](../../../../../../subtree.md) lies before all its pending ancestors in [inorder traversal](../../../../../../inorder-traversal.md); pushing and descending left preserves this fact. Its [loop variant](../../../../../../loop-variant.md) is the number of entries along the remaining left-child path, a finite decreasing quantity.

The outer [loop invariant](../../../../../../loop-invariant.md) says that `start` through `end` is precisely the already emitted sorted prefix, with reciprocal links and null outside endpoints. `current` and the pending ancestors describe exactly the remaining traversal in order; original links that are still needed have been retained. A pending ancestor has not yet had its right child overwritten. The next popped entry is therefore the next sorted entry. Saving `nextSubtree` preserves its future work before assigning `t.right = null`; linking it to `end` extends the prefix by exactly one entry. The number of original entries not yet emitted is an outer [loop variant](../../../../../../loop-variant.md), since each full outer iteration emits one. At exit nothing remains, proving the same preservation and ordering [postconditions](../../../../../../postcondition.md) as the recursive version.

Each entry is pushed and popped once, giving $O(n+1)$ [time complexity](../../../../../../time-complexity.md) and $O(h+1)$ [auxiliary space](../../../../../../auxiliary-space.md). No new `Tree` entries are allocated. The historical mutable [stack](../../../../../../stack-data-structure.md) interface provides the `push` and `pop` operations used here; its later deprecation does not change their meaning.[Scala 2.12.6, constructors, push(elem), pop(), nonEmpty](../../../../../../scala-2-12-mutable-stack-api-documentation.md)

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
