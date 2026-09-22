<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Implement the [Bernoulli distribution](../../../../../../bernoulli-distribution.md), taking special care that a zero-mass outcome is excluded from the [support of a probability distribution](../../../../../../support-of-a-probability-distribution.md):
```
class Flip(p: Double) extends FiniteDist[Boolean] {
  require(!p.isNaN && 0.0 <= p && p <= 1.0)

  def getDom: List[Boolean] =
    if (p == 0.0) List(false)
    else if (p == 1.0) List(true)
    else List(true, false)

  def getProb(x: Boolean): Double =
    if (x) p else 1.0 - p
}
```
The [precondition](../../../../../../precondition.md) excludes NaN and all values outside $[0,1]$, including infinities. The two masses are nonnegative and sum mathematically to one. **Endpoint domains are singleton lists**, while an interior parameter lists both outcomes exactly once. Treating `getDom` as always containing both [Booleans](../../../../../../boolean-data-type.md) would violate its positive-support contract at the endpoints.

## ↑ Ancestors (13)

1. [I](../i.md)
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
