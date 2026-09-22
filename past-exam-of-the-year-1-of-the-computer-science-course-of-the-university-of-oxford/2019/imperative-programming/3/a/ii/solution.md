<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the already-filled prefix itself for membership tests. `Long` intermediates avoid overflow in the candidate calculations, while a checked conversion respects the required output type:
```
def recaman(a: Array[Int]): Unit = {
  if (a.length == 0) return
  a(0) = 0
  var i = 1
  while (i < a.length) {
    val candidate = a(i - 1).toLong - i.toLong
    var j = 0
    while (candidate > 0L && j < i && a(j).toLong != candidate) {
      j += 1
    }
    val next =
      if (candidate > 0L && j == i) candidate
      else a(i - 1).toLong + i.toLong
    require(next <= Int.MaxValue.toLong, "Sequence value exceeds Int")
    a(i) = next.toInt
    i += 1
  }
}
```
The outer [loop invariant](../../../../../../loop-invariant.md) is $1\leq i\leq a.length$ and $a(t)=r(t)$ for $0\leq t<i$. The inner [loop invariant](../../../../../../loop-invariant.md) says that $0\leq j\leq i$ and no processed entry before `j` equals the positive candidate. Its guard either reaches the end of the prefix, finds the candidate, or immediately rejects a nonpositive candidate. Its [loop variant](../../../../../../loop-variant.md) is $i-j$. This establishes exactly the choice required by the recurrence, so the outer [loop invariant](../../../../../../loop-invariant.md) is preserved. The outer [loop variant](../../../../../../loop-variant.md) is $a.length-i$.

**Extra storage is $O(1)$** beyond the supplied result [array](../../../../../../array-data-structure.md). Membership scans give an $O(N^2)$ upper bound for $N$ output entries. Addition, unlike the subtraction branch, is not required to avoid repeats: at indices $20$ and $24$ the value $42$ occurs twice. The code therefore does not try to enforce global distinctness. If an exact value eventually exceeds `Int`, the output interface cannot hold it; the check reports that limitation rather than wrapping the recurrence.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
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
