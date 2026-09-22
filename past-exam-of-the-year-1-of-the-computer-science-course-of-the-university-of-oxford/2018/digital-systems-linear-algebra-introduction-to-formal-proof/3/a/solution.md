<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fetch the [MIPS instruction](../../../../../mips-instruction.md) at the [program counter](../../../../../instruction-pointer.md), and compute $pc+4$. The opcode selects an [MIPS R-type instruction](../../../../../mips-r-type-instruction.md); register-file read addresses $rs$ and $rt$ select the two operands. The function field selects ALU addition. The result returns through write-back multiplexer input zero to destination $rd$, and the next [program counter](../../../../../instruction-pointer.md) is $pc+4$.

Using the diagram's actual selector encodings, the [control signals](../../../../../control-input.md) are

$$
\begin{array}{c|ccccccccc}
&\mathrm{RegDst}&\mathrm{Branch}&\mathrm{Jump}&\mathrm{MemWrite}&\mathrm{MemToReg}&\mathrm{ALUOp}&\mathrm{MemRead}&\mathrm{ALUSrc}&\mathrm{RegWrite}\\\hline
\mathrm{add}&1&00&0&0&0&10&0&0&1
\end{array}.
$$

Here $\mathrm{ALUOp}=10$ means decode the function field; $00$ means add and $01$ means subtract. The source's $\mathrm{Branch}=(Br_1,Br_0)$ is a two-bit control: the branch-taken output is $Br_1\land(Br_0\mathbin{\oplus}\mathrm{Zero})$. With $Br_1=0$, $Br_0$ is immaterial; zero is a convenient concrete setting. No data-memory access occurs.

## ↑ Ancestors (12)

1. [A](../a.md)
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
