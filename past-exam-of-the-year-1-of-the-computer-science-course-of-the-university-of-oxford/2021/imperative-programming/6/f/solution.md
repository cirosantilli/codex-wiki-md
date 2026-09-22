<h1 id="6/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Give the wrapper exclusive ownership of a fresh delegate. It maintains its own inherited size so that inherited emptiness queries remain correct:

```
class IntegerSetWithCount extends IntegerSetPattern() {
  private val delegate = new IntegerSet()
  private var attempts = BigInt(0)

  override def contains(x: Int): Boolean = delegate.contains(x)

  override def insert(x: Int): Unit = {
    attempts += 1
    val wasPresent = delegate.contains(x)
    delegate.insert(x)
    if (!wasPresent) size += 1
  }
  override def delete(x: Int): Unit = {
    val wasPresent = delegate.contains(x)
    delegate.delete(x)
    if (wasPresent) size -= 1
  }
  override def pop(): Int = {
    if (isEmpty) throw new NoSuchElementException("set is empty")
    val answer = delegate.pop()
    size -= 1
    answer
  }
  override def clear: Unit = {
    delegate.clear
    size = 0
    attempts = BigInt(0)
  }
  def getCount: BigInt = attempts
}
```

Use the explicit membership signature and fresh default-constructible concrete set qualified in part d. The [representation invariant](../../../../../representation-invariant.md) is that the wrapper's `size` equals the delegate's [cardinality](../../../../../cardinality.md) and its counter equals client insertion attempts since construction or the latest successful client clear. The updates shown preserve that invariant when delegated operations fulfill their set contracts and failure checks leave the delegate unchanged. A duplicate does not increase size; deleting an absent element does not decrease it. Size changes follow successful delegation, whereas an attempted insertion is counted immediately.

**[Object composition](../../../../../object-composition.md) prevents internal delegate calls from dispatching into the wrapper's counter [object methods](../../../../../object-method.md).** It therefore survives the particular base revision in part e. The cost is forwarding code, another [software object](../../../../../software-object.md), some redundant size state imposed by the chosen abstract superclass, and extra membership queries. Future [object interface](../../../../../object-interface.md) [additions](../../../../../addition.md) must also be forwarded explicitly. This solution is an alternative definition of the [software class](../../../../../class-programming.md) in part d, not a second simultaneous definition.

## ↑ Ancestors (12)

1. [F](../f.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
