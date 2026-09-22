<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The implementation maintains the two boundaries from part b:

```
class ArrayDoubleStack(val MAX: Int) extends DoubleStack {
  require(MAX >= 0)
  private val data = new Array[Int](MAX)
  private var left = 0
  private var right = MAX

  def isEmptya: Boolean = left == 0
  def isEmptyb: Boolean = right == MAX

  def pusha(x: Int): Unit = {
    require(left < right, "double stack is full")
    data(left) = x
    left += 1
  }
  def pushb(x: Int): Unit = {
    require(left < right, "double stack is full")
    right -= 1
    data(right) = x
  }
  def popa: Int = {
    require(left > 0, "stack a is empty")
    left -= 1
    data(left)
  }
  def popb: Int = {
    require(right < MAX, "stack b is empty")
    val answer = data(right)
    right += 1
    answer
  }
}
```

Initialization gives empty abstract [lists](../../../../../list-abstract-data-type.md). Each push consumes one free position next to the appropriate top; each pop returns that top and releases its position. The guards preserve the ordering of the two boundaries and prevent invalid indexing. The [abstraction function](../../../../../abstraction-function.md) shows directly that the untouched [stack](../../../../../stack-data-structure.md) is unchanged. Keeping `data` private prevents clients from violating the [representation invariant](../../../../../representation-invariant.md); this strengthens [encapsulation](../../../../../encapsulation-computer-programming.md) relative to a publicly exposed implementation field without changing the six required operations.

**All six operations run in $O(1)$ time**, with a fixed [array](../../../../../array-data-structure.md) of `MAX` [integers](../../../../../integer-split.md) and constant extra state. Creating and zero-initializing the [array](../../../../../array-data-structure.md) takes $O(\mathrm{MAX})$ time, outside those operation bounds. Capacity zero gives a valid always-empty bounded structure whose pushes fail their [precondition](../../../../../precondition.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
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
