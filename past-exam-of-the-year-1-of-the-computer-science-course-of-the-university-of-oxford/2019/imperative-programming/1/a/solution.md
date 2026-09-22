<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Accumulate the prefix by [Horner's method](../../../../../horner-s-method.md) in base two. `digit-'0'` converts either permitted digit to its numerical value:
```
var i = 0
var integerPart = 0.0
while (i < bin.length && bin(i) != '.') {
  integerPart = 2.0 * integerPart + (bin(i) - '0')
  i += 1
}
```
The [loop invariant](../../../../../loop-invariant.md), in exact arithmetic, is that `i` is the number of processed digits before the point and

$$
integerPart=\sum_{j=0}^{i-1}(bin(j)-\mathtt{'0'})2^{i-1-j}.
$$

Appending a digit shifts the old positional value by one binary place and adds that digit, which proves preservation. The [loop variant](../../../../../loop-variant.md) is $bin.length-i$. At exit, `i` is the binary-point index or the length if no point occurs, and **`integerPart` is the value of the [integer](../../../../../integer-split.md) prefix**. An empty prefix contributes zero. There is one multiplication per processed digit, with no separate powers or repeated divisions. [Short-circuit evaluation](../../../../../short-circuit-evaluation.md) prevents an out-of-range access when the point is absent.

For `Double`, this exact-arithmetic [invariant](../../../../../invariant-mathematics.md) describes the intended value; the operational value is the rounded Horner recurrence. Very long prefixes can lose precision or overflow, as discussed in part (g). A fixed-width return type cannot represent every finite binary digit [string](../../../../../string.md) exactly.

## ↑ Ancestors (12)

1. [A](../a.md)
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
