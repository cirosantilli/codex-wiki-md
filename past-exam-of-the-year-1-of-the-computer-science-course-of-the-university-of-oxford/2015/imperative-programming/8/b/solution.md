<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Reject the empty [string](../../../../../string.md), because the given formula would divide by zero and no normalized [probability distribution](../../../../../probability-distribution-split.md) exists on its empty observed support. Remove repeated characters from `getDom`, but include all their occurrences when computing [probability](../../../../../probability.md).
```
class DistFromString(s: String) extends FiniteDist[Char] {
  require(s.nonEmpty)
  private val chars = s.toList
  private val dom = chars.distinct
  def getDom: List[Char] = dom
  def getProb(x: Char): Double =
    chars.count(c => c == x).toDouble / chars.length.toDouble
}
```
The [probability mass function](../../../../../probability-mass-function.md) is an [empirical probability distribution](../../../../../empirical-probability-distribution.md):

$$
\boxed{p(c)=\frac{\#\{i:s_i=c\}}{|s|}.}
$$

Every character occurrence contributes exactly once to the total count, so the [probabilities](../../../../../probability.md) sum to one. Absent characters have count zero. For `"Scala"`, the support is `List('S','c','a','l')`, with [probabilities](../../../../../probability.md) $1/5,1/5,2/5,1/5$ respectively. Here `Char` means the language's UTF-16 code unit, matching the supplied interface rather than assuming one [Unicode](../../../../../unicode.md) code point per element.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [8](../../8.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
