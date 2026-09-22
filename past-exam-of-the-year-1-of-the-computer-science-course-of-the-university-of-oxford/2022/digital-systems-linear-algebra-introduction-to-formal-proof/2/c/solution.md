<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Keep `total` in the [callee-saved register](../../../../../callee-saved-register.md) `r4`, and the first returned [sum](../../../../../sum.md) in the [callee-saved register](../../../../../callee-saved-register.md) `r5`. Suppose the surrounding function has made an aligned [stack frame](../../../../../stack-frame.md) with the local seven-halfword [array](../../../../../array-data-structure.md) at the current `sp`, occupying fourteen bytes in a sixteen-byte slot. One possible frame setup is `push {r4,r5,r6,lr}` followed by `sub sp,sp,#16`; the earlier code initializes `total`, `regular`, and `special` before this fragment.

```
    ldr  r0, =regular       @ assembler literal load of the global array address
    movs r1, #7
    bl   sum16
    movs r5, r0             @ first sum must survive the next call

    add  r0, sp, #0         @ current frame's local special array
    movs r1, #7
    bl   sum16
    muls r0, r5, r0         @ second sum times first sum
    adds r4, r4, r0         @ update total
```

The [AAPCS32](../../../../../aapcs32.md) permits each call to overwrite `r0`–`r3`, `r12`, and condition flags, but requires preservation of `r4`–`r8`, `r10`, `r11`, and `sp`. Thus both `r4` and `r5` remain valid even if `sum16` is replaced by another conforming implementation. `bl` changes the link [processor register](../../../../../processor-register.md) `lr`, so the enclosing function saves its own return address in its prologue. Its epilogue can use `add sp,sp,#16` and `pop {r4,r5,r6,pc}`. The frame uses thirty-two bytes in total, preserving the required eight-byte [stack pointer](../../../../../stack-pointer.md) alignment at both calls.[Sections 6.1.1, 6.2.1.2 and 6.4: scratch/preserved registers, public-interface alignment and word return](../../../../../procedure-call-standard-for-the-arm-architecture-by-arm-limited.md)

The two calls may be evaluated in this order. Assume the product and final addition fit the signed 32-[bit](../../../../../bit.md) result expected by the source program; unlike each individual seven-element [sum](../../../../../sum.md), their product need not fit. The [assembly language](../../../../../assembly-language.md) operations retain their low 32 [bits](../../../../../bit.md) if this assumption fails, whereas signed [integer overflow](../../../../../integer-overflow.md) in the [C programming language](../../../../../c-programming-language.md) has different semantics.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
