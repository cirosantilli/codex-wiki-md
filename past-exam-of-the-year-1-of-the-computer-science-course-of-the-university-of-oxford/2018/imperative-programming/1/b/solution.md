<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Generate each reciprocal [factorial](../../../../../factorial.md) from the preceding one, instead of recomputing a [factorial](../../../../../factorial.md) for every summand:
```
def eb(n: Int): Double = {
  require(n >= 0)
  var i = 0
  var term = 1.0
  var sum = 1.0
  while (i < n) {
    i += 1
    term /= i.toDouble
    sum += term
  }
  sum
}
```
The [loop invariant](../../../../../loop-invariant.md) is $0\leq i\leq n$, $term=1/i!$, and $sum=\sum_{j=0}^{i}1/j!$. Initially $i=0$ and $0!=1$. The division produces $1/(i+1)!$, which is then added to the previous partial [sum](../../../../../sum.md). The [loop variant](../../../../../loop-variant.md) is $n-i$. Consequently **the returned value is $e_b(n)$**, using exactly $n$ divisions and $n$ additions, no multiplications, and $O(n)$ [time complexity](../../../../../time-complexity.md). The slightly weaker [precondition](../../../../../precondition.md) also permits the useful zero-term boundary case. For `Double`, small positive terms eventually cease to change `sum` because of [floating-point rounding](../../../../../floating-point-rounding.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
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
