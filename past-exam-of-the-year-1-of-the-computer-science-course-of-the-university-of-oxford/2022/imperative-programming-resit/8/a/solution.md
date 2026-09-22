<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [complete multiset](../../../../../signed-multiset.md) is a finite-support signed count function. An absent key has count zero; negative counts are allowed. One simple default implementation uses a protected immutable association list with unique keys and nonzero values. Its default is empty, and optimized subclasses may override the public queries.

```
trait CompleteMultiSet[T] {
  // Representation contract: finite, immutable, unique keys, nonzero counts.
  protected def entries: List[(T, Int)] = Nil

  def count(t: T): Int =
    entries.find { case (key, _) => key == t }.map(_._2).getOrElse(0)

  lazy val present: Seq[T] = entries.map(_._1)

  private def combine(other: CompleteMultiSet[T],
                      op: (Int, Int) => Int): CompleteMultiSet[T] = {
    val keys = (present.toList ++ other.present.toList).distinct
    val resultRows = keys.flatMap { t =>
      val n = op(count(t), other.count(t))
      if (n == 0) Nil else List((t, n))
    }
    new CompleteMultiSet[T] {
      override protected val entries: List[(T, Int)] = resultRows
    }
  }

  def +(other: CompleteMultiSet[T]): CompleteMultiSet[T] =
    combine(other, (a, b) => java.lang.Math.addExact(a, b))

  def -(other: CompleteMultiSet[T]): CompleteMultiSet[T] =
    combine(other, (a, b) => java.lang.Math.subtractExact(a, b))

  def max(other: CompleteMultiSet[T]): CompleteMultiSet[T] =
    combine(other, (a, b) => math.max(a, b))

  def min(other: CompleteMultiSet[T]): CompleteMultiSet[T] =
    combine(other, (a, b) => math.min(a, b))

  def <=(other: CompleteMultiSet[T]): Boolean =
    (present.toList ++ other.present.toList).distinct.forall { t =>
      count(t) <= other.count(t)
    }

  override def toString: String =
    present.distinct.filter(t => count(t) != 0)
      .map(t => s"$t:${count(t)}").mkString("{", ", ", "}")
}
```

The [representation invariant](../../../../../representation-invariant.md) and [abstraction function](../../../../../abstraction-function.md) assign the association-list value at a stored key and zero elsewhere. Every operation preserves both operands and returns a fresh immutable value. The [finite-support pointwise operations](../../../../../finite-support-pointwise-operations.md) principle makes the support union sufficient because every operation sends $(0,0)$ to zero. It is necessary for signed counts: **the empty value is not at most a value having count $-1$ at one key**, although the empty left support alone would give a vacuous true comparison. Likewise, pointwise minimum can retain a negative count appearing only in the other operand.

**`present == List()` represents the all-zero, empty [complete multiset](../../../../../signed-multiset.md).** The list-backed default `count` takes $\Theta(1)$ time for a first-entry hit or an empty list, and $\Theta(N)$ in the worst case for a missing or final key, assuming constant-cost key equality. The default binary operations can consequently take quadratic time; they are deliberately simple defaults, not optimized implementations. The lazy `present` avoids an early call to a subclass's representation during initialization.

Counts use `Int`, so addition and subtraction explicitly throw `ArithmeticException` when the mathematical result is unrepresentable instead of silently wrapping. Equivalently, their mathematical [precondition](../../../../../precondition.md) requires representable result counts. This machine-size restriction is separate from permitting negative counts.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
