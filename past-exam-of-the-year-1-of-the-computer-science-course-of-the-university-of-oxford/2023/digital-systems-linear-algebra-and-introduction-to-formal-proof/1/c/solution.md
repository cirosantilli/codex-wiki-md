<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a 32-[bit](../../../../../bit.md) [machine word](../../../../../machine-word.md) and $1\leq k\leq31$, use a [left bit shift](../../../../../left-bit-shift.md) followed by a [logical right shift](../../../../../logical-right-shift.md):
```
lsls r1, r0, #(32-k)
lsrs r1, r1, #(32-k)
```
The left shift discards all but the lowest $k$ [bits](../../../../../bit.md) and moves those retained [bits](../../../../../bit.md) to the top. The [logical right shift](../../../../../logical-right-shift.md) returns them to their original positions and fills the rest with zero. Hence **`r1` contains $a\bmod 2^k$**, the remainder identified in (b). For $k=0$ the remainder is zero; for $k=32$ it is $a$, so these endpoints can be handled directly.

On a [reduced instruction set computer](../../../../../reduced-instruction-set-computer.md), a [bit mask](../../../../../bit-mask.md) such as $2^k-1$ may not fit an instruction's immediate field. Masking may therefore require materializing the constant in another [processor register](../../../../../processor-register.md), possibly using several instructions or a memory load. Small shift counts are directly encodable, so the two shifts can save code space, a temporary [processor register](../../../../../processor-register.md), or a load. This is an architecture-dependent advantage, rather than a universal speed claim. The source's compact instruction forms support these immediate shifts, while their [bitwise AND](../../../../../bitwise-and.md) form takes its other operand from a [processor register](../../../../../processor-register.md).[page 1, Logical and Shift/rotate tables](../../../../../thumb-16-bit-instruction-set-quick-reference-by-arm.md)

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [Digital systems](../../digital-systems.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
