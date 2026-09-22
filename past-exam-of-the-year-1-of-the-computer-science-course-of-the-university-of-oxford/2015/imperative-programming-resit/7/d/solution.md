<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use a [programming closure](../../../../../closure-computer-programming.md) whose private variable holds the next [Fibonacci number](../../../../../fibonacci-number.md). Use [arbitrary-precision integers](../../../../../arbitrary-precision-integer.md) to enumerate all terms exactly:
```
def fibonacci(): Iter[BigInt] = {
  var following = BigInt(1)
  val step: BigInt => BigInt = (current: BigInt) => {
    val result = following
    following = current + following
    result
  }
  new FunIter[BigInt](BigInt(0), step)
}
```
At the cell containing $F_i$, the private state immediately before computing its successor is `following = F_(i+1)`. The successor returns that value and sets `following` to $F_i+F_{i+1}=F_{i+2}$, preserving the [recursion invariant](../../../../../recursion-invariant.md). The resulting [sequence](../../../../../sequence.md) starts

$$
\boxed{0,1,1,2,3,5,8,13,21,34,\ldots.}
$$

Each successor is computed once by the memoized implementation in part (c); interleaved copies see the same already generated successor instead of independently advancing shared [programming closure](../../../../../closure-computer-programming.md) state. Replacing `BigInt` by `Int` and the two initial values by `0,1` gives exactly the hinted `Int => Int` implementation, but eventually incurs [integer overflow](../../../../../integer-overflow.md), so it does not enumerate all mathematical [Fibonacci numbers](../../../../../fibonacci-number.md).

An alternative avoiding mutable [programming closure](../../../../../closure-computer-programming.md) state represents the current and next [Fibonacci numbers](../../../../../fibonacci-number.md) by a [pair](../../../../../pair.md) $(a,b)$ and uses the [pure function](../../../../../pure-function.md) $(a,b)\mapsto(b,a+b)$ with initial state $(0,1)$; a projecting [iterator](../../../../../iterator.md) returns the first component. The closure construction above meets the suggested one-number interface directly.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
