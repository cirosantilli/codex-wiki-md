<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Give the step function one private previous-value cell, freshly allocated for each independent Fibonacci generator:

```
def fibonacci(): Iter[BigInt] = {
  var previous = BigInt(1)
  val step: BigInt => BigInt = { current =>
    val following = previous + current
    previous = current
    following
  }
  new FunIter[BigInt](BigInt(0), step)
}
```

The initial artificial previous value is $F_{-1}=1$, making the first update return one. Thereafter, just before advancing from $F_n$, the captured cell holds $F_{n-1}$; the assignment produces $F_{n+1}$ and retains $F_n$. [Induction](../../../../../mathematical-induction.md) gives **$0,1,1,2,3,5,8,\ldots$**. `BigInt` avoids the fixed-width overflow that would prevent `Int` from representing all [Fibonacci numbers](../../../../../fibonacci-number.md).

Copies made through part (c) share memoized future cells, so interleaving their traversal does not advance this private state twice for the same sequence position. A separate call to `fibonacci()` receives a separate closure. Another valid construction uses a pure step on the pair $(F_n,F_{n+1})$ and projects the first coordinate; the stateful construction above follows the suggested single-current-value approach.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
