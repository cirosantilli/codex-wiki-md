<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the semantics stipulated by the question, **write $pc+4$ to register 31 and load the next $pc$ from register $rs$**. Read $rs$ through register-file output $rd_0$. Select input two of the next-PC multiplexer, which is already wired from $rd_0$. Select destination input two, already the constant register number 31, and write-back input two, already $pc+4$.

Thus the printed diagram already contains the necessary three-way [multiplexers](../../../../../multiplexer.md) and wires. Extend the controller's opcode/function decoding to generate

$$
\begin{array}{c|ccccccccc}
&\mathrm{RegDst}&\mathrm{Branch}&\mathrm{Jump}&\mathrm{MemWrite}&\mathrm{MemToReg}&\mathrm{ALUOp}&\mathrm{MemRead}&\mathrm{ALUSrc}&\mathrm{RegWrite}\\\hline
\mathrm{jalr}&2&00&2&0&2&00&0&0&1
\end{array}.
$$

The displayed $\mathrm{ALUOp}$ and $\mathrm{ALUSrc}$ settings are arbitrary safe choices for an unused result. **No additional datapath hardware or control field is required** beyond decoding this instruction into the existing values. This uses the question's explicitly specified $pc+4$ link convention.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
