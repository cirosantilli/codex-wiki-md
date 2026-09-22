<h1 id="7/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The inclusive interval is nonempty exactly when **$l\leq u$**. Reject $l>u$ with a failed [precondition](../../../../../../precondition.md), rather than assigning a nonexistent normalization to an empty interval. Compute its width in `Long` before taking a reciprocal:
```
class Uniform(l: Int, u: Int) extends FiniteDist[Int] {
  require(l <= u, "Empty uniform interval")
  private val width = u.toLong - l.toLong + 1L
  private val mass = 1.0 / width.toDouble

  def getProb(x: Int): Double =
    if (l <= x && x <= u) mass else 0.0

  def getDom: List[Int] = {
    var x = l.toLong
    var rev = List.empty[Int]
    while (x <= u.toLong) {
      rev = x.toInt :: rev
      x += 1L
    }
    rev.reverse
  }
}
```
The [loop invariant](../../../../../../loop-invariant.md) says that $l\leq x\leq u+1$ and `rev` contains exactly the [integers](../../../../../../integer-split.md) $l,\ldots,x-1$ in reverse order. The [loop variant](../../../../../../loop-variant.md) is $u-x+1$ while the guard is true. `Long` handles both the full interval width $2^{32}$ and the increment past `Int.MaxValue`. At exit, reversing yields each support value once. All support values have mass $1/(u-l+1)$, so their exact sum is one; `Double` approximates that [rational number](../../../../../../rational-number.md). Very large valid domains require correspondingly large lists and sufficient memory; that resource issue does not make the mathematical endpoint values invalid.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [Imperative programming resit](../../../../imperative-programming-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
