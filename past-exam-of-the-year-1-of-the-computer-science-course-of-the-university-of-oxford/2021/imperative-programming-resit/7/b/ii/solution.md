<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use a widened interval width, so the arithmetic also handles endpoints near the limits of `Int`:
```
final class Uniform(l: Int, u: Int) extends FiniteDist[Int] {
  require(l <= u)
  private val width = u.toLong - l.toLong + 1L

  def getDom: List[Int] = {
    val builder = List.newBuilder[Int]
    var value = l.toLong
    while (value <= u.toLong) {
      builder += value.toInt
      value += 1L
    }
    builder.result()
  }

  def getProb(x: Int): Double =
    if (l <= x && x <= u) 1.0 / width.toDouble else 0.0
}
```
The support [lists](../../../../../../list-abstract-data-type.md) every [integer](../../../../../../integer-split.md) in the inclusive interval once. Its [cardinality](../../../../../../cardinality.md) is `width`, so assigning each atom mass $1/width$ gives total mass one. The loop counter is also widened, preventing an increment past `Int.MaxValue` from wrapping to a negative value. Returning the full support takes time and space proportional to its width and can be impractical for a very large interval; the mass query itself is constant-time. The full [integer](../../../../../../integer-split.md) interval has width $2^{32}$, which fits `Long` but not positive `Int`.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Imperative programming (resit)](../../../../imperative-programming-resit-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
