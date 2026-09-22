<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [opcode](../../../../../opcode.md) occupies bits $31:26$, the [arithmetic logic unit](../../../../../arithmetic-logic-unit.md) operation is wired directly to $15:10$, and an [immediate operand](../../../../../immediate-operand.md) uses all of $9:0$. A three-register instruction needs fifteen register-selection [bits](../../../../../bit.md), whereas an immediate instruction must retain independent source and destination selectors outside $9:0$.

Thus put $r_s$ and $r_d$ in the ten bits $25:16$, and place $r_t$ in five of $9:0$, where it can overlap the unused [immediate operand](../../../../../immediate-operand.md) of a register instruction. One valid [instruction encoding](../../../../../instruction-encoding.md) is

$$
\boxed{r_s=I[25:21],\qquad r_d=I[20:16],\qquad r_t=I[9:5].}
$$

Bits $4:0$ are unused for a three-register instruction. In an immediate instruction, $r_t$ has no effect because its read value is deselected by the `ToAlu` [multiplexer](../../../../../multiplexer.md). In a `store`, $r_s$ selects the address and $r_t$ selects the data; $r_d$ must be zero to suppress the incidental register write. These observations follow the original [datapath](../../../../../datapath.md), particularly its direct $val_s$ memory-address connection and the connection from the `ToAlu` output to memory write data.[Printed p. 3, processor block diagram](../../../../../digital-systems-linear-algebra-introduction-to-formal-proof-examination-paper-by-the-university-of-oxford-2013.md)

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
