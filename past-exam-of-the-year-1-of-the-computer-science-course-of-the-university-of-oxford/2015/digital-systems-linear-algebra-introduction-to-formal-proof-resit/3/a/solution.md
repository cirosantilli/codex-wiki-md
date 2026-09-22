<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In the pictured single-cycle [MIPS architecture](../../../../../mips-architecture.md), `RegDst` selects the write address of the [register file](../../../../../register-file.md): zero selects instruction bits $20\ldots16$, the `rt` field used by a load; one selects bits $15\ldots11$, the `rd` field used by an [MIPS R-type instruction](../../../../../mips-r-type-instruction.md). `RegWrite` enables the clocked write to the selected [processor register](../../../../../processor-register.md).

`ALUSrc` selects the second [ALU](../../../../../arithmetic-logic-unit.md) input: zero uses the second [register file](../../../../../register-file.md) read output, while one uses the sign-extended 16-[bit](../../../../../bit.md) immediate field. The `zero` signal is produced by the [ALU](../../../../../arithmetic-logic-unit.md), rather than being an opcode-decoder output: it is one exactly when the [ALU](../../../../../arithmetic-logic-unit.md) result is zero. During `beq`, the [ALU](../../../../../arithmetic-logic-unit.md) subtracts its operands, so `zero` tests equality. The diagram combines it with `Branch` to select the branch target instead of $PC+4$.

$$
\boxed{\operatorname{TakeBranch}=\operatorname{Branch}\land\operatorname{zero}.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
