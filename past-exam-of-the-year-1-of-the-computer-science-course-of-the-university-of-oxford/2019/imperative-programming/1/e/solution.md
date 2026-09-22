<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Generate the fractional bits by repeated doubling, keeping only the unconverted residual:
```
res(digits) = '.'
var fraction = dec - int_part.toDouble
var out = digits + 1
while (out < res.length) {
  fraction = 2.0 * fraction
  if (fraction >= 1.0) {
    res(out) = '1'
    fraction -= 1.0
  } else res(out) = '0'
  out += 1
}
```
Let $f_0=dec-int\_part$ and $k=out-digits-1$. The [loop invariant](../../../../../loop-invariant.md) is $0\leq fraction<1$, the first $k$ fractional digits have been written, and, in exact arithmetic,

$$
f_0=\sum_{t=1}^{k}(res(digits+t)-\mathtt{'0'})2^{-t}+fraction\,2^{-k}.
$$

Doubling exposes the next digit, and subtracting that digit leaves the next residual in $[0,1)$. This proves preservation. The [loop variant](../../../../../loop-variant.md) is $res.length-out$. The loop fills the whole suffix, even when the residual has become zero; subsequent bits are zero. There is one multiplication per output bit. With $F=res.length-digits-1$ fractional positions, **the result is truncated, with exact-arithmetic error $0\leq dec-value(res)<2^{-F}$**. An [integer](../../../../../integer-split.md) has an all-zero suffix. No rounding-up step is performed.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
