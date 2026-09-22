<h1 id="10/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Choose bit zero of each integer to represent the leftmost cell in its group of 32 columns. Then use a quotient to choose the word and a remainder to choose the bit:
```
java
static boolean getBit(int[][] board, int i, int j) {
    return ((board[i][j >>> 5] >>> (j & 31)) & 1) != 0;
}
```
For valid $0\leq i,j<1024$, `j >>> 5` is $\lfloor j/32\rfloor$ and ranges from zero to 31. The [bit mask](../../../../../../bit-mask.md) `j & 31` is the offset $j\bmod32$. The logical right [bit shift](../../../../../../bit-shift.md) brings the desired bit to position zero; the final mask selects only that bit. **Even bit 31 of a negative stored word is extracted correctly**, because `>>>` inserts zeros. A different convention, with the leftmost cell in the most significant bit, would instead shift by `31 - (j & 31)` and must be used consistently.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [10](../../10.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
