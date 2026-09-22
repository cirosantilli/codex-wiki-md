<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The second [partial function](../../../../../partial-function.md) accepts this one's outputs. Put this method inside the invariant class in part (b):
```
def compose[V](that: PartialFn[U, V]): PartialFn[T, V] = {
  val pairs: List[(T, V)] = data.flatMap {
    case (x, y) => that.get(y).map(z => (x, z)).toList
  }
  new PartialFn[T, V](pairs)
}
```
**The represented mapping is $that\circ this$**, since the paper explicitly applies `that` second despite the method name. A pair is emitted exactly when this mapping supplies a `y` and `that.get(y)` supplies a `z`. Hence its [domain of a partial function](../../../../../domain-of-a-partial-function.md) is $\{x\in\operatorname{dom}(this):this(x)\in\operatorname{dom}(that)\}$ and its value there is $that(this(x))$. This is strict [composition of partial functions](../../../../../composition-of-partial-functions.md): either missing stage makes the composite undefined. Repeated equal input pairs still produce the same output, preserving the representation [invariant](../../../../../invariant-mathematics.md). With $m$ and $k$ pairs, direct association-list lookup gives $O(m(k+1)+1)$ worst-case [time complexity](../../../../../time-complexity.md), not a hidden constant-cost dictionary lookup.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
