<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Test each positive candidate [divisor](../../../../../divisor.md) and count the successful remainder tests:
```
def divisors(n: Int): Int = {
  require(n >= 1)
  var candidate = 1L
  var count = 0
  while (candidate <= n.toLong) {
    if (n.toLong % candidate == 0L) count += 1
    candidate += 1L
  }
  count
}
```
The [loop invariant](../../../../../loop-invariant.md) is $1\leq d\leq n+1$ and $count=|\{j:1\leq j<d,\ j\mid n\}|$, where $d$ denotes `candidate`. A successful test adds exactly the new [divisor](../../../../../divisor.md); an unsuccessful test leaves the count unchanged. The [loop variant](../../../../../loop-variant.md) is $n+1-d$, which decreases by one. At termination $d=n+1$, so **the returned value is $\tau(n)$**. A `Long` loop counter prevents the increment after the last positive `Int` candidate from wrapping around.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
