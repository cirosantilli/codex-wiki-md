<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[SP-relative addressing](../../../../../sp-relative-addressing.md) forms an effective memory address by adding an offset to the [stack pointer](../../../../../stack-pointer.md). It accesses local variables, saved [processor registers](../../../../../processor-register.md) or other stack-frame data without dedicating a separate base [processor register](../../../../../processor-register.md) for each object. The supplied reference gives word-aligned SP-relative offsets from $0$ to $1020$, which corresponds to an eight-bit nonnegative field scaled by four.

In the modified [datapath](../../../../../datapath.md), select the [stack pointer](../../../../../stack-pointer.md) for the unshifted [ALU](../../../../../arithmetic-logic-unit.md) input, the instruction [immediate operand](../../../../../immediate-operand.md) for the [barrel shifter](../../../../../barrel-shifter.md) input, and [ALU](../../../../../arithmetic-logic-unit.md) addition. The effective address can then be **$\mathrm{SP}+(\mathrm{imm}\ll s)$**. Scaling the [immediate operand](../../../../../immediate-operand.md) changes the reachable displacement range without storing a larger [immediate operand](../../../../../immediate-operand.md). For example, an eight-bit field shifted by two reaches offsets through $255\times4=1020$; shifting it by four reaches through $4080$, but only on a sixteen-byte grid. Larger range and finer address granularity are different properties, so the extra reach is not free arbitrary-byte addressing.

The parallel layout cannot feed a shifted [immediate operand](../../../../../immediate-operand.md) directly into its address-producing [ALU](../../../../../arithmetic-logic-unit.md) in the same pass. The serial layout can. The actual [immediate operand](../../../../../immediate-operand.md) width and permitted shift encodings of a new instruction must be specified; the question does not fix them, so no particular enlarged instruction encoding is implied.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
