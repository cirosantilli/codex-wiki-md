<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $w,x,y,z$ as the four input [bits](../../../../../bit.md), of weights $8,4,2,1$, and let 1 light a segment of the [seven-segment display](../../../../../seven-segment-display.md). The required [truth table](../../../../../truth-table.md) is
```
value   wxyz   abcdefg
 0      0000   1111110
 1      0001   0110000
 2      0010   1101101
 3      0011   1111001
 4      0100   0110011
 5      0101   1011011
 6      0110   1011111
 7      0111   1110000
 8      1000   1111111
 9      1001   1111011
10      1010   0000000
11      1011   0000000
12      1100   0000000
13      1101   0000000
14      1110   0000000
15      1111   0000000
```
Here [binary-coded decimal](../../../../../binary-coded-decimal.md) represents one decimal digit per group of four bits. The six unused codes must be zeros in every output for this part; they are not [don't-care conditions](../../../../../don-t-care-term.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
