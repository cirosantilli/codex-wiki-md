<h1 id="8/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use [strength reduction](../../../../../../../strength-reduction.md) on the disassembled hot instructions. In a fixed-width wrapping integer model,

$$
\boxed{8x=x\ll3,\qquad 15x=(x\ll4)-x\pmod{2^w}.}
$$

The first replacement is a single left [bit shift](../../../../../../../bit-shift.md). For the second, preserve the original operand in a register, shift a copy left by four and subtract the original:
```
text
rOriginal = x
rResult = rOriginal << 4
rResult = rResult - rOriginal
```
This avoids a general multiplication if shifts and subtraction are cheaper on the target processor. The two identities hold for positive and negative [two's complement](../../../../../../../two-s-complement.md) operands when only the low $w$ result bits are required.

Because only a binary is available, patch the machine instructions and adjust displaced branches or use a jump to a replacement code block if the new sequence does not fit. Preserve live registers and the calling convention. If later instructions consume overflow or other condition flags, or the original multiplication produces a double-width result or traps on overflow, matching only the low-word arithmetic is insufficient: those effects must be reproduced or the transformation rejected. Finally, measure the modified program; a fast hardware multiply need not be slower than several replacement instructions.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Ia](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
