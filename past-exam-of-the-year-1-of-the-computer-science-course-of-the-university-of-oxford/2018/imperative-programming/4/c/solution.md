<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The following class uses the bounded insertion contract from part (b). `slot` performs mathematical circular indexing with a wider intermediate, so even large legal indices do not overflow before reduction:
```
class ArrayDoubleEndedQueue(val MAX: Int) extends DoubleEndedQueue {
  require(MAX > 0)
  private val a = new Array[Int](MAX)
  private var head = 0
  private var size = 0

  private def slot(offset: Int): Int =
    ((head.toLong + offset.toLong) % MAX.toLong).toInt

  private def before(i: Int): Int = if (i == 0) MAX - 1 else i - 1
  private def after(i: Int): Int = if (i == MAX - 1) 0 else i + 1

  def isEmpty: Boolean = size == 0

  def addLeft(x: Int): Unit = {
    require(size < MAX)
    head = before(head)
    a(head) = x
    size += 1
  }

  def addRight(x: Int): Unit = {
    require(size < MAX)
    a(slot(size)) = x
    size += 1
  }

  def getLeft(): Int = {
    require(size > 0)
    val x = a(head)
    head = after(head)
    size -= 1
    x
  }

  def getRight(): Int = {
    require(size > 0)
    val x = a(slot(size - 1))
    size -= 1
    x
  }
}
```
For `addLeft`, moving the first position back one slot makes the old position the new logical index one; inserting at the new position prepends `x`. For `addRight`, the old `size` is the first unoccupied logical index, so writing there appends `x`. The removals read the appropriate endpoint and exclude that slot from the occupied interval. Every operation preserves the [representation invariant](../../../../../representation-invariant.md) and realizes the [abstraction function](../../../../../abstraction-function.md) postcondition. Old contents in unused slots cannot be observed through this interface. Each operation performs a fixed number of accesses and arithmetic operations, hence has [constant time](../../../../../constant-time.md) and [constant space](../../../../../constant-space.md) per call, apart from the class's $O(MAX)$ backing storage.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
