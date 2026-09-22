<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Repeated [integer division](../../../../../integer-division.md) by two generates the [binary digits](../../../../../binary-digit.md) from least significant to most significant. Reverse the accumulated characters once, and treat zero separately.

```
def binaryCon(n: Int): String = {
  require(n >= 0, "n must be nonnegative")
  if (n == 0) return "0"
  var remaining = n
  val digits = new StringBuilder
  while (remaining > 0) {
    digits.append(if (remaining % 2 == 0) '0' else '1')
    remaining /= 2
  }
  digits.reverse.toString
}
```

**Zero produces `"0"`; positive inputs produce a [binary number](../../../../../binary-number.md) without leading zeros.** No library routine performs the number-to-base conversion. Appending to the builder and reversing once gives linear work in the number of [binary digits](../../../../../binary-digit.md) and uses that much output storage.

## ↑ Ancestors (12)

1. [A](../a.md)
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
