<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Validate the complete input before doing the addition. The [arrays](../../../../../array-data-structure.md) use most-significant-digit-first [positional notation](../../../../../positional-notation.md). The result has one extra leading position, which contains either zero or the final carry.

```
def binaryAddition(x: Array[Int], y: Array[Int]): Array[Int] = {
  require(x != null && y != null, "arrays must not be null")
  require(x.length == y.length, "lengths must match")
  val n = x.length
  var k = 0
  while (k < n) {
    require((x(k) == 0 || x(k) == 1) &&
            (y(k) == 0 || y(k) == 1), "digits must be 0 or 1")
    k += 1
  }
  val answer = new Array[Int](n + 1)
  var carry = 0
  var j = n - 1
  while (j >= 0) {
    val column = x(j) + y(j) + carry
    answer(j + 1) = column % 2
    carry = column / 2
    j -= 1
  }
  answer(0) = carry
  answer
}
```

A failed `require` throws `IllegalArgumentException`, covering mismatched lengths, invalid [binary digits](../../../../../binary-digit.md) and null [arrays](../../../../../array-data-structure.md). The largest column sum is three, so the carry always lies in $\{0,1\}$. The [binary-addition carry invariant](../../../../../binary-addition-carry-invariant.md) says that the already processed input suffixes equal the written result suffix plus the carry shifted to the next column. After the final column, placing that carry at position zero proves the returned value is the sum. Neither input [array](../../../../../array-data-structure.md) is modified. Equal empty inputs are accepted as zero and return `Array(0)`; the specification imposes no positive-length restriction. [Running time](../../../../../running-time.md) and result storage are $O(N)$.

## ↑ Ancestors (12)

1. [B](../b.md)
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
