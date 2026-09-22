<h1 id="6/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use a fixed-size count [array](../../../../../../array-data-structure.md) and protected hooks defining a stable character-to-slot mapping. The default hooks count the ASCII lowercase interval. The document must start empty, and all subsequent edits must pass through the [mixin](../../../../../../mixin.md) methods, as they do for `new DocImp with CharCountPlugin`.

```
trait CharCountPlugin extends Doc {
  protected def firstCounted: Char = 'a'
  protected def numberCounted: Int = 26
  protected def slot(ch: Char): Int = {
    val k = ch.toInt - firstCounted.toInt
    if (0 <= k && k < numberCounted) k else -1
  }
  private lazy val totals = Array.fill(numberCounted)(0)

  abstract override def insert(pos: Int, ch: Char): Unit = {
    val k = slot(ch)
    super.insert(pos, ch)
    if (k >= 0) totals(k) += 1
  }

  abstract override def delete(pos: Int): Char = {
    val removed = super.delete(pos)
    val k = slot(removed)
    if (k >= 0) totals(k) -= 1
    removed
  }

  def count(ch: Char): Int = {
    val k = slot(ch)
    require(k >= 0, "character is outside the counted alphabet")
    totals(k)
  }
}
```

The additional [representation invariant](../../../../../../representation-invariant.md) is that each [array](../../../../../../array-data-structure.md) slot equals the number of corresponding characters in the current document. Initially all counts are zero. Each successful underlying edit changes exactly one relevant count, while a failed position check throws before any count is changed. Returning the actual deleted character lets deletion adjust the correct slot.

`count` takes **$O(1)$ time for the fixed alphabet**, as do the [mixin](../../../../../../mixin.md)'s additions to edit cost. The lazy [array](../../../../../../array-data-structure.md) avoids reading subclass-overridden size hooks during [trait](../../../../../../trait.md) construction; the hooks must remain stable. An extension can override the interval hooks, or override `slot` with another fixed finite mapping. This is [stackable modification by a trait](../../../../../../stackable-trait-modification.md): `abstract override` permits the method to call the next implementation of `super`, supplied here by `DocImp`.[Abstract override and [trait](../../../../../../trait.md) linearization](../../../../../../scala-2-13-classes-and-objects-specification.md)

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [6](../../../6.md)
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
