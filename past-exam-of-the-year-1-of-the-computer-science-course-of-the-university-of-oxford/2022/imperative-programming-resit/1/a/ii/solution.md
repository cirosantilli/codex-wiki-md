<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use [exponentiation by squaring](../../../../../../exponentiation-by-squaring.md) with the remaining exponent halved on every iteration:

```
def eaFast(n: Int): Double = {
  require(n > 0)
  var remaining = n
  var base = 1.0 + 1.0 / n.toDouble
  var result = 1.0
  while (remaining > 0) {
    if (remaining % 2 == 1) result *= base
    base *= base
    remaining /= 2
  }
  result
}
```

Writing $a=1+1/n$, the exact-arithmetic [loop invariant](../../../../../../loop-invariant.md) is $remaining\geq0$ and $result\,base^{remaining}=a^n$. For an [even integer](../../../../../../even-number.md) exponent $2q$, replace the base by its square and the exponent by $q$. For an [odd integer](../../../../../../odd-integer.md) exponent $2q+1$, first multiply the accumulator by the base and then make the same replacement. Both preserve the product. The [loop variant](../../../../../../loop-variant.md) is `remaining`, which strictly decreases while positive. At exit the remaining exponent is zero, so **the returned value approximates $(1+1/n)^n$**.

There are $L=\lfloor\log_2 n\rfloor+1$ iterations, $L$ squarings and one accumulator multiplication for each set [bit](../../../../../../bit.md) of $n$: between $L+1$ and $2L$ multiplications. Thus the bound is $\Theta(\log n)$ as $n\to\infty$, or $\Theta(1+\log n)$ including the small case $n=1$. All power variables are `Double`; no unintended `Int` squaring occurs.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Imperative programming (resit)](../../../../imperative-programming-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
