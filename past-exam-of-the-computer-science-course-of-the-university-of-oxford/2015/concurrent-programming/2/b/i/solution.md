<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the recorded child [list](../../../../../../list-abstract-data-type.md) as the [depth-first traversal](../../../../../../depth-first-search.md) order. A [leaf of a tree](../../../../../../leaf-of-a-tree.md) has no children, so it contributes its own identity once. Closure cancels the remaining traversal; a normal completion closes the output so that a consumer can detect end-of-fringe.

```
def dfFringe(node: Array[Node], root: NodeId, fringe: ![NodeId]): PROC = proc {
  def walk(v: NodeId): Unit = {
    val cs = node(v).children
    if (cs.isEmpty) fringe ! v
    else cs.foreach(walk)
  }
  try { walk(root) }
  catch { case _: io.threadcso.process.Stopped => () }
  finally { fringe.closeOut }
}
```

A completed finite [spanning tree](../../../../../../spanning-tree.md) has no recursive child [graph cycle](../../../../../../cycle-in-a-graph.md), so this visits a finite number of [vertices](../../../../../../vertex-graph-theory.md). A blocked leaf send is released if its output closes. A singleton root is itself a [leaf of a tree](../../../../../../leaf-of-a-tree.md) and is output once. With sufficient call-stack space,

$$
\boxed{\text{emit each leaf once in child-list depth-first order; catch closure and close the port}.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Concurrent programming](../../../../concurrent-programming-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
