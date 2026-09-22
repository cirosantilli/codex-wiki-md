<h1 id="3/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $N$ result entries the largest required index is $N-1$, so the bound in part (a)(iii) permits universe size $M=N(N-1)/2+1$. Check that the chosen universe can itself be expressed as an [array](../../../../../../array-data-structure.md) length:
```
def recamanBitmap(a: Array[Int]): Unit = {
  val n = a.length
  if (n == 0) return
  val capacity = n.toLong * (n.toLong - 1L) / 2L + 1L
  require(capacity <= Int.MaxValue.toLong, "Bitmap universe too large")
  val seen = new BitMapSet(capacity.toInt)
  a(0) = 0
  seen.add(0)
  var i = 1
  while (i < n) {
    val candidate = a(i - 1).toLong - i.toLong
    val next =
      if (candidate > 0L && !seen.contains(candidate.toInt)) candidate
      else a(i - 1).toLong + i.toLong
    a(i) = next.toInt
    seen.add(a(i))
    i += 1
  }
}
```
The [loop invariant](../../../../../../loop-invariant.md) is that the result prefix contains exactly $r(0),\ldots,r(i-1)$ and the [abstraction function](../../../../../../abstraction-function.md) of `seen` is their [set](../../../../../../set-split.md) of values. The universe bound ensures that each positive candidate being queried and each actual next value is less than `capacity`; values are nonnegative. Thus the conversions and the restricted `add` [precondition](../../../../../../precondition.md) are justified, rather than merely hoped to succeed. At a repeated addition, `add` returning false is harmless: the set of previously seen values is still updated correctly. The [loop variant](../../../../../../loop-variant.md) is $n-i$. **At return every result entry agrees with the original recurrence.**

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [3](../../../3.md)
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
