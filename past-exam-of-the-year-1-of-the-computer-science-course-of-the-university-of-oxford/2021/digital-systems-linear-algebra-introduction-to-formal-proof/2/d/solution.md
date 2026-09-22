<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

On the same primary-[opcode](../../../../../opcode.md) expansion interpretation, **[opcode](../../../../../opcode.md): 9 [bits](../../../../../bit.md); each register field: 8 [bits](../../../../../bit.md)**. The printed `rd` is a naming slip: a conventional [MIPS I-type instruction](../../../../../mips-i-type-instruction.md) has fields `rs` and `rt`, with the latter sometimes serving as the destination. There is no separate `rd` field.

Keeping the original 16-[bit](../../../../../bit.md) immediate requires $9+8+8+16=\mathbf{41}$ [bits](../../../../../bit.md) per instruction. If the [instruction encoding](../../../../../instruction-encoding.md) were held at 32 [bits](../../../../../bit.md), only seven [bits](../../../../../bit.md) would remain for the immediate, reducing immediate arithmetic and addressing ranges. A uniform encoding for both enlarged formats would have to accommodate the longer R-type case too; any padding or revised format policy must be specified separately. Register count and instruction width do not determine data-word width.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
