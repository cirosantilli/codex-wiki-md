<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [Horner's method](../../../../../horner-s-method.md), accumulating the high-degree coefficients before the low-degree ones:

```
def eval(x: Double): Double = {
  var i = a.length
  var value = 0.0
  while (i > 0) {
    i -= 1
    value = a(i) + x * value
  }
  value
}
```

At each [while loop](../../../../../while-loop.md) head the [loop invariant](../../../../../loop-invariant.md) is

$$
0\leq i\leq n,\qquad \mathrm{value}=\sum_{j=i}^{n-1}a(j)x^{j-i}.
$$

The initial sum is empty. Decreasing `i` and replacing the accumulator by `a(i) + x * value` extends that sum by one coefficient with the required powers shifted. The [loop variant](../../../../../loop-variant.md) is `i`; on exit it is zero, so the accumulator equals $p(x)$. The code uses **exactly $n$ [multiplications](../../../../../multiplication.md) and $O(n)$ time**, with constant auxiliary space, and also handles the empty coefficient [array](../../../../../array-data-structure.md) as the zero [polynomial](../../../../../polynomial-split.md). Initializing from the last coefficient instead would save one [multiplication](../../../../../multiplication.md) for nonempty [arrays](../../../../../array-data-structure.md).

The invariant is an exact-arithmetic specification. With `Double`, each arithmetic operation rounds; consequently the code evaluates the Horner expression in [floating-point arithmetic](../../../../../floating-point-arithmetic-split.md), rather than guaranteeing the exact real value for arbitrary coefficients.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
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
