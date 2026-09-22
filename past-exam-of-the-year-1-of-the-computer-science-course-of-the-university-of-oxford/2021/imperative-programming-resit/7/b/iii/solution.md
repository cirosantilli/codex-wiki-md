<h1 id="7/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Reject the empty [string](../../../../../../string.md) because it has no positive total count to normalize:
```
final class DistFromString(s: String) extends FiniteDist[Char] {
  require(s.nonEmpty)
  private val frequencies =
    s.foldLeft(Map.empty[Char, Int]) { (counts, c) =>
      counts.updated(c, counts.getOrElse(c, 0) + 1)
    }

  def getDom: List[Char] = s.toList.distinct

  def getProb(c: Char): Double =
    frequencies.getOrElse(c, 0).toDouble / s.length.toDouble
}
```
The support contains each occurring character once, and a character absent from the [string](../../../../../../string.md) gets mass zero. The occurrence counts sum to the nonzero [string](../../../../../../string.md) length, proving normalization. For a separate example, the [string](../../../../../../string.md) `"aba"` gives masses $2/3$ and $1/3$ to its two characters. The interpretation follows [Scala](../../../../../../scala.md)'s `Char` elements, so it counts UTF-16 code units rather than imposing a separate Unicode-code-point representation. The `Double` results approximate the corresponding rational probabilities.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
