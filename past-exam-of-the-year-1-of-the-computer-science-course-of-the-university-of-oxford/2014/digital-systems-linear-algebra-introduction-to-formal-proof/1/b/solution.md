<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Add [zero extension](../../../../../zero-extension.md) alongside [sign extension](../../../../../sign-extension.md), and a [multiplexer](../../../../../multiplexer.md) controlled by a new signal `ExtSign` to select between them before the existing immediate-input connection. Equivalently, make the extender itself selectable:

$$
\boxed{\mathrm{extended}_{15:0}=n,\qquad \mathrm{extended}_{31:16}=\begin{cases}n_{15}\cdots n_{15},&\mathrm{ExtSign}=1,\\0\cdots0,&\mathrm{ExtSign}=0.\end{cases}}
$$

Decode `ori` to `ExtSign=0`, `RegDst=0`, `ALUSrc=1`, `RegWrite=1` and `ALUFunc=OR`. The [arithmetic logic unit](../../../../../arithmetic-logic-unit.md) then performs [bitwise OR](../../../../../bitwise-or.md) between $y$ and the zero-extended [immediate operand](../../../../../immediate-operand.md) and writes the result to $x$. Extend the [arithmetic logic unit](../../../../../arithmetic-logic-unit.md)'s control decoding if OR was not already available. Decode `addi` to `ExtSign=1`; the new signal is irrelevant for [MIPS R-type instructions](../../../../../mips-r-type-instruction.md) because `ALUSrc=0`.

[Zero extension](../../../../../zero-extension.md) matters even when the most significant immediate [bit](../../../../../bit.md) is one: `ori` with `0x8000` must only affect the low half of the destination, whereas [sign extension](../../../../../sign-extension.md) would incorrectly force every high [bit](../../../../../bit.md) to one.[ORI instruction entry: the 16-bit immediate is zero-extended before the logical operation](../../../../../mips32-architecture-for-programmers-volume-ii-by-mips-technologies.md)

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
