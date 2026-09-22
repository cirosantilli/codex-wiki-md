<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fetch and decode the [MIPS I-type instruction](../../../../../mips-i-type-instruction.md), read $rs$ and $rt$, and subtract their values in the [arithmetic logic unit](../../../../../arithmetic-logic-unit.md). The [zero flag](../../../../../zero-flag.md) is one exactly when they are equal. The branch target is

$$
\mathrm{BrT}=(pc+4)+\bigl(\operatorname{signextend}(imm)\ll2\bigr).
$$

The branch selector chooses that target when $Br_1=1$ and $Br_0=0$ make the diagram's condition equal to $\mathrm{Zero}$. Otherwise it chooses $pc+4$. Neither registers nor data memory are written. The [control signals](../../../../../control-input.md) are

$$
\begin{array}{c|ccccccccc}
&\mathrm{RegDst}&\mathrm{Branch}&\mathrm{Jump}&\mathrm{MemWrite}&\mathrm{MemToReg}&\mathrm{ALUOp}&\mathrm{MemRead}&\mathrm{ALUSrc}&\mathrm{RegWrite}\\\hline
\mathrm{beq}&-&10&0&0&-&01&0&0&0
\end{array}.
$$

Dashes are [don't-care conditions](../../../../../don-t-care-term.md) because register write enable is zero. The immediate goes to the branch-target adder, while the main ALU's second input remains the value in $rt$.

## ↑ Ancestors (12)

1. [B](../b.md)
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
