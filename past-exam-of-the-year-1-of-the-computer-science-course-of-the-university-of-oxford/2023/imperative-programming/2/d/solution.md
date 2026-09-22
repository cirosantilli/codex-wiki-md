<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The algorithmic intention is **[exponentiation by squaring](../../../../../exponentiation-by-squaring.md) to compute $x^n$ for $n\geq0$**. With exact arithmetic, its [loop invariant](../../../../../loop-invariant.md) is

$$
i\geq0,\qquad result\,y^i=x^n.
$$

Initially `result = 1`, `y = x`, and `i = n`. For an [even integer](../../../../../even-number.md) $i=2q$, squaring `y` and replacing `i` by $q$ preserves the product. For an [odd integer](../../../../../odd-integer.md) $i=2q+1$, first multiply `result` by `y`; then $(result\,y)(y^2)^q=result\,y^{2q+1}$. The nonnegative [loop variant](../../../../../loop-variant.md) `i` decreases by halving whenever positive. At exit $i=0$, so the [loop invariant](../../../../../loop-invariant.md) yields `result = x^n`. There are $O(\log(n+1))$ multiplication steps.

Two qualifications are essential for the actual source. There is no requirement that `n` be nonnegative: **for every `n <= 0` the printed function simply returns `1.0`**. Also, `var y = x` infers `Int`, so `y *= y` uses wrapping [integer arithmetic](../../../../../integer-arithmetic.md), while the accumulator uses [floating-point arithmetic](../../../../../floating-point-arithmetic-split.md). For example, **`anotherfunc(50000, 2L)` returns `-1794967296.0`, rather than `2500000000.0`**. An exact-power [loop invariant](../../../../../loop-invariant.md) cannot prove a false claim about that execution.

More precisely, for positive `n`, after $k$ iterations the remaining exponent is $\lfloor n/2^k\rfloor$, and the `Int` base is the signed 32-bit representative of $x^{2^k}$ modulo $2^{32}$. The accumulator multiplies those signed representatives for the set [bits](../../../../../bit.md) of `n`, in increasing bit order, with a floating-point rounding after each multiplication. This describes the actual code even when the intended power law fails. In an exact implementation, use a nonnegative-exponent [precondition](../../../../../precondition.md) and arbitrary-precision [integers](../../../../../integer-split.md), for example:

```
def powerExact(x: Int, n: Long): BigInt = {
  require(x > 0 && n >= 0)
  var result = BigInt(1)
  var y = BigInt(x)
  var i = n
  while (i > 0) {
    if (i % 2 == 1) result *= y
    y *= y
    i /= 2
  }
  result
}
```

The displayed [loop invariant](../../../../../loop-invariant.md) applies exactly to this version. It performs logarithmically many arbitrary-precision multiplications; their bit cost grows with operand size, so that statement is not an $O(\log n)$ bit-complexity bound. Merely making the accumulator a `Double` does not widen the separate `Int` base variable.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
