<h1 id="7/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use relative character frequencies, an [empirical distribution](../../../../../../type-information-theory.md). A nonempty [string](../../../../../../string.md) is required because an empty sample has no normalized frequency distribution:
```
class DistFromString(s: String) extends FiniteDist[Char] {
  require(s != null && s.nonEmpty, "A nonempty string is required")
  private val chars = s.toList
  private val domain = chars.distinct

  def getDom: List[Char] = domain

  def getProb(c: Char): Double =
    chars.count(_ == c).toDouble / s.length.toDouble
}
```
`distinct` removes repeated support entries without changing which characters occur. Every returned domain element has positive frequency, and every absent character has frequency zero. The occurrence counts partition the [string](../../../../../../string.md)'s character positions, so their total is `s.length`, establishing normalization. **For `Scala`, the masses are $2/5$ for `a` and $1/5$ each for `S`, `c` and `l`.** The character units here are exactly the `Char` values supplied by `s.toList`; the interface does not specify a different notion of displayed text characters. The code has no explicit loop beyond the specified library traversals.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
