<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Extract successive bytes into indices of the [byte-table population count](../../../../../byte-table-population-count.md) table. The last shift leaves only the original high byte, so that index needs no final mask.

```
popcount_table:
    push {r4}
    adr r2, popbyte
    movs r3, #255
    movs r1, r0
    ands r1, r1, r3
    ldrb r4, [r2, r1]
    lsrs r0, r0, #8
    movs r1, r0
    ands r1, r1, r3
    ldrb r1, [r2, r1]
    adds r4, r4, r1
    lsrs r0, r0, #8
    movs r1, r0
    ands r1, r1, r3
    ldrb r1, [r2, r1]
    adds r4, r4, r1
    lsrs r0, r0, #8
    ldrb r1, [r2, r0]
    adds r0, r4, r1
    pop {r4}
    bx lr
```

Place the byte table at an aligned nearby label in the instruction-address range of `adr`. That instruction forms the table's address relative to the [program counter](../../../../../instruction-pointer.md); it does not load a table entry. Each `ldrb` uses [register-offset addressing](../../../../../register-offset-addressing.md): the base is `r2`, the byte offset is the index register, and the loaded byte is zero-extended. Because entries occupy one byte, the index needs no scaling. `ldrb r1, [r2, r1]` uses the old `r1` to form the address before overwriting it with the result.

Every bit belongs to exactly one extracted byte, so adding the four table counts gives **the whole word's [population count](../../../../../hamming-weight.md)**, independently of [endianness](../../../../../endianness.md). The calculation reads four bytes from the table and contains no loop.

## ↑ Ancestors (12)

1. [B](../b.md)
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
