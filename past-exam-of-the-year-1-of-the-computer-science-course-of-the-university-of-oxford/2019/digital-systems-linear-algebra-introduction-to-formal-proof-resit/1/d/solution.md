<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let the new byte table store $L[0]=8$ and, for $1\le b\le255$, $L[b]=7-\lfloor\log_2 b\rfloor$. Thus it stores the number of leading zeros in an eight-bit argument: $L[1]=7$, $L[2]=L[3]=6$, and $L[128],\ldots,L[255]=0$. All entries fit in one byte.

```
countlz:
    adr r3, lzbyte
    movs r1, #0
    lsrs r2, r0, #24
    bne lz_found
    movs r1, #8
    lsrs r2, r0, #16
    bne lz_found
    movs r1, #16
    lsrs r2, r0, #8
    bne lz_found
    movs r1, #24
    movs r2, r0
lz_found:
    ldrb r2, [r3, r2]
    adds r0, r1, r2
    bx lr
```

The high byte is tried first. A failed test proves that byte was zero, so the next right-shifted value is again a byte-sized index without masking: all higher bytes have already been proved zero. The offset in `r1` counts those skipped zero bytes in bits. Adding the table result for the first nonzero byte gives the [leading-zero count](../../../../../count-leading-zeros.md). If every byte is zero, the last lookup contributes eight to the offset 24, giving **32**. The example with high byte one gives **7**. At most three conditional branches and one table read are needed; no per-bit loop is used.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
