<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [AAPCS32](../../../../../aapcs32.md) convention: `r0` holds the input address, `r1` the length, and `r0` receives the result. The following [Thumb instruction set](../../../../../thumb-instruction-set.md) [assembly language](../../../../../assembly-language.md) uses only scratch [processor registers](../../../../../processor-register.md), so no [callee-saved registers](../../../../../callee-saved-register.md) need saving. Assume the [array](../../../../../array-data-structure.md) is valid, halfword-aligned, and has nonnegative length; for the mathematical [sum](../../../../../sum.md) assume it fits a signed 32-[bit](../../../../../bit.md) [two's complement](../../../../../two-s-complement.md) [integer](../../../../../integer-split.md).

```
.syntax unified
.thumb
.thumb_func
sum16:
    movs r2, #0             @ accumulated sum
    cmp  r1, #0
    ble  .Ldone             @ empty array; also returns 0 if n < 0
.Lloop:
    movs r3, #0             @ Thumb signed load needs a register offset
    ldrsh r3, [r0, r3]      @ signed halfword at a; offset read before r3 changes
    adds r2, r2, r3         @ include this signed value
    adds r0, r0, #2         @ advance by one short, not one byte
    subs r1, r1, #1         @ one fewer element remains
    bne  .Lloop
.Ldone:
    movs r0, r2             @ result register
    bx   lr                 @ leaf routine: lr was not overwritten
```

After $j$ iterations, the [loop invariant](../../../../../loop-invariant.md) is that `r2` contains the first $j$ elements' [sum](../../../../../sum.md), `r0` points to element $j$, and `r1` is $n-j$. The [sign extension](../../../../../sign-extension.md) in `ldrsh` supplies the correct signed addend. One iteration preserves this [loop invariant](../../../../../loop-invariant.md), and the decreasing remaining length proves [algorithm termination](../../../../../algorithm-termination.md). For the seven-element calls, the [sum](../../../../../sum.md) lies between $-229376$ and $229369$, so it fits. For longer [arrays](../../../../../array-data-structure.md) that overflow, these instructions compute the [sum](../../../../../sum.md) modulo $2^{32}$; that is not a claim about defined signed [C programming language](../../../../../c-programming-language.md) overflow behavior. The operand forms are those of the paper's reference sheet.[Load: signed halfword; Add/Subtract; Branch](../../../../../thumb-16-bit-instruction-set-quick-reference-by-arm.md)

## ↑ Ancestors (12)

1. [A](../a.md)
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
