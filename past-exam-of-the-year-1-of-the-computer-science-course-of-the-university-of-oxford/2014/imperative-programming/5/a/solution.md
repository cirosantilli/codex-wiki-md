<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Interpret `step` as a positive increment, consistent with the increasing [sequence](../../../../../sequence.md) and exclusive upper bound. State this precondition explicitly; a zero increment would not define the intended finite progression. Use a wider cursor to avoid [integer overflow](../../../../../integer-overflow.md) on the update after the last valid `Int` result.
```
class RangeIter(lower: Int, upper: Int, step: Int) extends Iter[Int] {
  require(step > 0)
  private var current = lower.toLong
  def hasNext: Boolean = current < upper.toLong
  def next(): Int = {
    require(hasNext)
    val answer = current.toInt
    current += step.toLong
    answer
  }
}
```
After $q$ calls to `next`, the [abstraction function](../../../../../abstraction-function.md) is the [sequence](../../../../../sequence.md) of values $\mathrm{lower}+t\,\mathrm{step}<\mathrm{upper}$ with $t\geq q$, in increasing order. Repeated calls to `hasNext` do not change it; `next` removes precisely its first value. Therefore

$$
\boxed{1,3,5,7,9,11\quad\text{for }\mathrm{RangeIter}(1,13,2).}
$$

If `lower >= upper`, the represented [sequence](../../../../../sequence.md) is empty immediately. The paper does not specify a descending-range convention; this implementation exposes its positive-step precondition rather than assigning one implicitly.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
