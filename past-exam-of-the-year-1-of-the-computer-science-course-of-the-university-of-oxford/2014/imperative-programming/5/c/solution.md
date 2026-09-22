<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [iterator](../../../../../iterator.md) adapter from part (b) with a [primality test](../../../../../primality-testing.md) by [trial division](../../../../../trial-division.md). A composite positive [integer](../../../../../integer-split.md) has a divisor no greater than its [square root](../../../../../square-root.md).
```
def primeIter(upperBound: Int): Iter[Int] = {
  def isPrime(n: Int): Boolean = {
    if (n < 2) false
    else {
      var d = 2
      while (d <= n / d && n % d != 0) d += 1
      d > n / d
    }
  }
  filterIter[Int](isPrime _, new RangeIter(2, upperBound, 1))
}
```
Before each [trial division](../../../../../trial-division.md) iteration, no [integer](../../../../../integer-split.md) in $[2,d)$ divides `n`. If division succeeds, the condition becomes false with $d\leq n/d$, and `isPrime` returns false. Otherwise the loop ends with $d>n/d$, so every possible small [divisor](../../../../../divisor.md) has been excluded. The quotient comparison is equivalent to $d^2\leq n$ for positive values and avoids [integer overflow](../../../../../integer-overflow.md) in `d*d`.

$$
\boxed{\mathrm{primeIter}(23):\quad2,3,5,7,11,13,17,19.}
$$

Bounds at most two give an empty [iterator](../../../../../iterator.md). This method tests candidates lazily and uses $O(\sqrt n)$ [trial divisions](../../../../../trial-division.md) for candidate $n$; no efficiency requirement in the question forces a [sieve of Eratosthenes](../../../../../sieve-of-eratosthenes.md) implementation.

## ↑ Ancestors (12)

1. [C](../c.md)
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
