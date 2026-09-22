<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let `point` be the known point index. Work backwards so that each step uses just one division, rather than separately computing positional weights:
```
var j = bin.length - 1
var fractionalPart = 0.0
while (j > point) {
  fractionalPart = (fractionalPart + (bin(j) - '0')) / 2.0
  j -= 1
}
```
The [loop invariant](../../../../../loop-invariant.md), under exact arithmetic, is

$$
fractionalPart=\sum_{t=j+1}^{bin.length-1}(bin(t)-\mathtt{'0'})2^{j-t}.
$$

Initially the suffix is empty. Incorporating digit $j$ and dividing by two gives exactly the same formula with $j$ replaced by $j-1$. At exit $j=point$, **the result is $\sum_{t>point}(bin(t)-\mathtt{'0'})2^{point-t}$**. The [loop variant](../../../../../loop-variant.md) is $j-point$ when a point exists. If a no-point input is handled by setting `point=bin.length`, the loop is skipped and the fractional contribution is zero; $\max(0,j-point)$ is a [loop variant](../../../../../loop-variant.md) covering that convention too. Trailing zeroes and an empty fractional suffix require no special arithmetic. [Floating-point rounding](../../../../../floating-point-rounding.md) qualifies the exact formula for long inputs.

## ↑ Ancestors (12)

1. [B](../b.md)
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
