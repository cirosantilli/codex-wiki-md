<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a [logical right shift](../../../../../logical-right-shift.md) to discard one inspected bit at a time. The following [Thumb instruction set](../../../../../thumb-instruction-set.md) subroutine accepts the word in `r0`, returns its [population count](../../../../../hamming-weight.md) in `r0`, preserves `r4`, and otherwise uses caller-saved [processor registers](../../../../../processor-register.md).

```
popcount_loop:
    push {r4}
    movs r1, #0
    movs r2, #1
    movs r3, #32
pop_loop:
    movs r4, r0
    ands r4, r4, r2
    adds r1, r1, r4
    lsrs r0, r0, #1
    subs r3, r3, #1
    bne pop_loop
    movs r0, r1
    pop {r4}
    bx lr
```

`ands` extracts the current least significant bit; `adds` includes it in the count. `lsrs` fills the newly vacant high position with zero. `subs` immediately precedes `bne`, so the branch tests the [zero flag](../../../../../zero-flag.md) from decrementing the loop counter, not a flag left by the shift.

After $k$ iterations, the accumulator contains the number of one bits in the original word's $k$ lowest positions, and the remaining word is the original [unsigned interpretation](../../../../../unsigned-interpretation-of-a-bit-string.md) shifted right by $k$. This [loop invariant](../../../../../loop-invariant.md) holds initially and is preserved by each iteration. At $k=32$ every position has been inspected, proving the result. The given example therefore returns **10**, and the all-zero and all-one words return **0** and **32**. The accumulator cannot overflow: it never exceeds 32.

## ↑ Ancestors (12)

1. [A](../a.md)
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
