<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Run two `dfFringe` producers on synchronous one-to-one [message-passing channels](../../../../../../message-passing-channel.md), and compare one received leaf from each. Catch closure separately on each input: otherwise the first closure could hide an extra value in the other fringe. An extra value or unequal pair is enough to stop immediately.

```
def sameFringe(node1: Array[Node], root1: NodeId,
               node2: Array[Node], root2: NodeId): Boolean = {
  val a = OneOne[NodeId]
  val b = OneOne[NodeId]
  var equal = true

  def next(p: ?[NodeId]): Option[NodeId] =
    try { Some(p ? ()) }
    catch { case _: io.threadcso.process.Stopped => None }

  val compare = proc {
    var done = false
    try {
      while (!done) {
        val x = next(a)
        val y = next(b)
        (x, y) match {
          case (None, None) => done = true
          case (Some(u), Some(v)) if u == v => ()
          case _ => equal = false; done = true
        }
      }
    } finally { a.closeIn; b.closeIn }
  }
  (dfFringe(node1, root1, a) || dfFringe(node2, root2, b) || compare)()
  equal
}
```

After $k$ successful comparisons, the first $k$ identities in the two leaf [sequences](../../../../../../sequence.md) agree. The first differing pair disproves [equality](../../../../../../equality-mathematics.md) of [sequences](../../../../../../sequence.md); simultaneous exhaustion proves it; exhaustion on exactly one side disproves it. Therefore,

$$
\boxed{\mathrm{sameFringe}=\mathrm{true}\iff\text{the ordered leaf sequences agree, including length}.}
$$

Closing both inputs on every comparator exit releases either producer if it is waiting in an output. The closure handler in `dfFringe` then returns normally, and the parallel composition joins before `equal` is read. For finite [trees](../../../../../../tree-graph-theory-split.md) and eventual scheduling, the comparator's next read either obtains a leaf or observes completion, so there is no [deadlock](../../../../../../deadlock.md) caused by reading the two inputs in a fixed order.

Only a constant amount of leaf data is stored. After an early mismatch, each producer may already have traversed toward its next leaf and be blocked offering it; cancellation prevents unbounded speculation or deliberate construction of the remaining fringe. Occasionally a short unequal fringe is already completely traversed when its final distinguishing value is compared. The streaming guarantee is that neither complete fringe needs to be materialized in advance, and work stops as soon as inequality is established.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
