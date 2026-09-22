<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Validate the parameter, and include exactly the outcomes of positive mass:
```
final class Flip(p: Double) extends FiniteDist[Boolean] {
  require(p >= 0.0 && p <= 1.0)

  def getDom: List[Boolean] =
    if (p == 0.0) List(false)
    else if (p == 1.0) List(true)
    else List(false, true)

  def getProb(x: Boolean): Double = if (x) p else 1.0 - p
}
```
The range test also rejects `NaN`, since its ordered comparisons are false. At the endpoints one outcome has zero mass and must be omitted from the support; listing both unconditionally would violate the supplied interface contract. For an interior parameter the two masses are positive and sum to one.

## ↑ Ancestors (13)

1. [I](../i.md)
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
