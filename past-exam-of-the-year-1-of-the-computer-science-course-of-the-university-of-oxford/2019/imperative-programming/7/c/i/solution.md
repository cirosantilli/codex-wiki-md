<h1 id="7/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Compare areas before and after each completed setter call. Widen before multiplication so all products of two `Int` dimensions are represented exactly:
```
class LoggedResizableFrame(h: Int, w: Int) extends ResizableFrame(h, w) {
  private var increases = BigInt(0)

  private def actualArea: Long = height.toLong * width.toLong

  override def height_=(h: Int): Unit = {
    val before = actualArea
    super.height_=(h)
    if (actualArea > before) increases += 1
  }

  override def width_=(w: Int): Unit = {
    val before = actualArea
    super.width_=(w)
    if (actualArea > before) increases += 1
  }

  def getIncreases: BigInt = increases
}
```
The history [invariant](../../../../../../invariant-mathematics.md) is that `increases` counts exactly the completed dimension updates whose new area strictly exceeds their immediately preceding area. The constructor's starting area is a baseline, not an increase. Each overriding setter invokes the superclass setter once and increments precisely when its comparison succeeds. Equal-area changes do not count. **The comparison is on area, not merely on which dimension increased**; this also handles zero or signed dimensions without adding an unstated input restriction. An [arbitrary-precision integer](../../../../../../arbitrary-precision-integer.md) avoids eventual counter overflow.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [7](../../../7.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
