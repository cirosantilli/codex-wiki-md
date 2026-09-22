<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the paper's 26-letter alphabet, use the [Oberon](../../../../../oberon-programming-language.md) `CAP` operation and contiguous character codes:
```
PROCEDURE Index(c: CHAR): INTEGER;
BEGIN
  RETURN ORD(CAP(c)) - ORD("A")
END Index;
```
Both cases of a letter map to the same uppercase letter before subtraction, so **the result lies in `0..25`**. This relies on the ordinary Latin `A`–`Z` and `a`–`z` character encoding used by [Oberon](../../../../../oberon-programming-language.md); it is not a Unicode case-folding algorithm. The stipulated letter-only [precondition](../../../../../precondition.md) avoids any need to reject punctuation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
