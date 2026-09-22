<h1 id="8/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Keep a private immutable hash-map value in a mutable variable. Each update computes a complete replacement from snapshots and commits it once; this handles self-aliasing and arithmetic failure without partially modifying the receiver.

```
class MultiSetVarImp[T] extends MultiSetVar[T] {
  private var table = Map.empty[T, Int]

  def count(t: T): Int = table.getOrElse(t, 0)
  def present: Seq[T] = table.keys.toVector

  def copy(other: CompleteMultiSet[T]): Unit = {
    val saved = other.present.distinct.iterator
      .map(t => (t, other.count(t))).filter(_._2 != 0).toMap
    table = saved
  }

  private def snapshot(other: MultiSetVar[T]): Map[T, Int] =
    other.present.distinct.iterator
      .map(t => (t, other.count(t))).filter(_._2 != 0).toMap

  private def update(other: MultiSetVar[T], op: (Int, Int) => Int): Unit = {
    val left = table
    val right = snapshot(other)
    val keys = left.keySet ++ right.keySet
    val builder = Map.newBuilder[T, Int]
    keys.foreach { t =>
      val n = op(left.getOrElse(t, 0), right.getOrElse(t, 0))
      if (n != 0) builder += ((t, n))
    }
    val replacement = builder.result()
    table = replacement
  }

  def +(other: MultiSetVar[T]): Unit =
    update(other, (a, b) => java.lang.Math.addExact(a, b))

  def -(other: MultiSetVar[T]): Unit =
    update(other, (a, b) => java.lang.Math.subtractExact(a, b))

  def max(other: MultiSetVar[T]): Unit =
    update(other, (a, b) => math.max(a, b))

  def min(other: MultiSetVar[T]): Unit =
    update(other, (a, b) => math.min(a, b))

  def <=(other: CompleteMultiSet[T]): Boolean = {
    val left = table
    (left.keySet ++ other.present).forall { t =>
      left.getOrElse(t, 0) <= other.count(t)
    }
  }
}
```

The [representation invariant](../../../../../../representation-invariant.md) is a finite map of nonzero counts with no representation exposed to callers. The [abstraction function](../../../../../../abstraction-function.md) adds implicit zero elsewhere. `getOrElse` implements that default; `keys` enumerates stored keys; `distinct` removes repeated input support entries; `toMap` builds an independent immutable map; and the builder accumulates the next representation before it is assigned. The private immutable snapshots remain stable while the new state is computed.

For self-addition, both snapshots contain the same old counts, so they double; self-subtraction yields empty support; self-max and self-min leave the value unchanged. A distinct operand is never assigned or mutated. An overflow exception during building occurs before the final assignment, so the receiver remains unchanged. These are instances of [snapshot-before-update semantics](../../../../../../snapshot-before-update-semantics.md).

Lookup is expected $O(1)$ under standard hash assumptions. Enumerating `present` takes $O(K)$ for support size $K$. Combining two instances of this implementation takes expected $O(K+M)$ time and temporary storage, including snapshot construction. For an arbitrary argument implementation, add the costs of its `count` calls: copying a default list-backed [complete multiset](../../../../../../signed-multiset.md) can require $\Theta(M^2)$, whereas copying the hash-backed version is expected linear. No generic interface can guarantee another implementation's query cost. Inputs are assumed to have finite, complete support enumerations and stable counts during an operation; concurrent mutation would need a separate synchronization contract.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [E](../../e.md)
3. [8](../../../8.md)
4. [Imperative programming (resit)](../../../../imperative-programming-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
