<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Count each invocation before delegating, including duplicate insertions, and reset after clearing:

```
class IntegerSetWithCount extends IntegerSet() {
  private var attempts = BigInt(0)

  override def insert(x: Int): Unit = {
    attempts += 1
    super.insert(x)
  }
  override def clear: Unit = {
    super.clear
    attempts = BigInt(0)
  }
  def getCount: BigInt = attempts
}
```

The inherited implementation already maintains `size`; the new counter measures insertion attempts, not successful increases in [cardinality](../../../../../cardinality.md). Deletion and popping do not subtract from it. Incrementing before delegation also counts an attempted insertion that subsequently fails a capacity check. [Arbitrary-precision arithmetic](../../../../../arbitrary-precision-arithmetic.md) avoids silently wrapping the historical count, though its arithmetic is not constant-cost for arbitrarily large counts.

As the source supplies no [object constructor](../../../../../object-constructor.md) signature for the concrete set, this code uses a fresh default-constructible `IntegerSet`, with matching default capacity. Its correct behavior also assumes the base implementation does not internally invoke these overridable operations in a way that interferes with the counter. Part e exhibits that dependency.

**Source-signature qualification for the following set implementations:** the intended membership query must be declared `def contains(x: Int): Boolean`. The printed abstract declaration omits its result type; interpreted literally as [Scala](../../../../../scala.md) 2 procedure syntax, it returns `Unit`. The solutions use the explicit Boolean query contract, and `Unit` for the two mutators. Parameterless `clear` is overridden without adding parentheses.[Procedures: a method declaration omitting its result type implicitly has Unit result](../../../../../scala-2-13-basic-declarations-and-definitions-specification.md)

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
