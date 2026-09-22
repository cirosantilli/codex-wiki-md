<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Implement the count [function](../../../../../function-split.md) directly in a private [array](../../../../../array-data-structure.md):
```
class ArrayIntBag(val MAX: Int) extends IntBag {
  require(MAX > 0)
  private val c = new Array[Int](MAX)
  private def inRange(x: Int): Boolean = 0 <= x && x < MAX

  def add(x: Int): Unit = {
    require(inRange(x))
    require(c(x) < Int.MaxValue)
    c(x) += 1
  }
  def remove(x: Int): Unit = {
    require(inRange(x))
    require(c(x) > 0)
    c(x) -= 1
  }
  def count(x: Int): Int = {
    require(inRange(x))
    c(x)
  }
}
```
The [representation invariant](../../../../../representation-invariant.md) is that `c` has length `MAX` and every stored count is nonnegative. The [abstraction function](../../../../../abstraction-function.md) gives $bag(x)=c(x)$ in range and zero outside it. Zero initialization establishes the [invariant](../../../../../invariant-mathematics.md). An allowed [addition](../../../../../addition.md) changes exactly one entry without overflow; an allowed removal changes exactly one positive entry without making it negative; querying changes none. Thus each method implements its abstract [postcondition](../../../../../postcondition.md) as well as preserving the [representation invariant](../../../../../representation-invariant.md). The private [array](../../../../../array-data-structure.md) prevents clients from bypassing those guarantees.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
