<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the stipulated [MIPS I-type instruction](../../../../../mips-i-type-instruction.md) encoding, whose unused $rt$ field is zero, so register-file output $rd_1$ supplies the hardwired zero register. With $\mathrm{ALUSrc}=0$ and subtraction selected, the [arithmetic logic unit](../../../../../arithmetic-logic-unit.md) computes $R[rs]-0$. Its [zero flag](../../../../../zero-flag.md) detects $R[rs]=0$, while bit 31 of $rd_0$ is the sign in [two's complement](../../../../../two-s-complement.md). Therefore the required signed test is

$$
R[rs]>0\iff\neg\mathrm{Zero}\land\neg rd_0[31].
$$

Introduce one new control bit $GT$, and replace the zero-flag input to the existing branch XOR by

$$
Z^*=\mathrm{Zero}\lor(GT\land rd_0[31]).
$$

This needs an AND gate, an OR gate and a tap of the sign bit. With $GT=0$, existing branch behavior is unchanged. With $GT=1$ and $\mathrm{Branch}=11$, the existing branch-taken circuit gives $\neg Z^*$, exactly the positive test. Its output still selects between $pc+4$ and the usual sign-extended branch target. The complete control row is

$$
\begin{array}{c|cccccccccc}
&\mathrm{RegDst}&\mathrm{Branch}&\mathrm{Jump}&\mathrm{MemWrite}&\mathrm{MemToReg}&\mathrm{ALUOp}&\mathrm{MemRead}&\mathrm{ALUSrc}&\mathrm{RegWrite}&GT\\\hline
\mathrm{bgtz}&-&11&0&0&-&01&0&0&0&1
\end{array}.
$$

Set $GT=0$ for each instruction in parts (a)–(c). Registers and data memory remain unchanged. The available signed `slt` operation could support a different design; the sign-and-zero design above avoids adding an ALU-input swap and explicitly distinguishes zero from positive values.

## ↑ Ancestors (12)

1. [D](../d.md)
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
