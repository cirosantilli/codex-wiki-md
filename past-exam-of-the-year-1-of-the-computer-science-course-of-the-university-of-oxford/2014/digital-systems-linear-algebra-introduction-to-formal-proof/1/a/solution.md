<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [MIPS R-type instruction](../../../../../mips-r-type-instruction.md) has the 32-[bit](../../../../../bit.md) [instruction encoding](../../../../../instruction-encoding.md)

$$
\underbrace{\mathrm{op}}_{6}\ \underbrace{\mathrm{rs}}_{5}\ \underbrace{\mathrm{rt}}_{5}\ \underbrace{\mathrm{rd}}_{5}\ \underbrace{\mathrm{shamt}}_{5}\ \underbrace{\mathrm{funct}}_{6}.
$$

For `add $x,$y,$z`, the [processor register](../../../../../processor-register.md) indices are $\mathrm{rs}=y$, $\mathrm{rt}=z$ and $\mathrm{rd}=x$, while $\mathrm{shamt}=0$. The main [opcode](../../../../../opcode.md) selects the R-type family and the function field selects addition. The [register file](../../../../../register-file.md) reads its two operands from instruction [bits](../../../../../bit.md) 25:21 and 20:16. In the original [datapath](../../../../../datapath.md), `RegDst=1` selects [bits](../../../../../bit.md) 15:11 as the destination, `ALUSrc=0` selects the second [register file](../../../../../register-file.md) output, and `ALUFunc=ADD` makes the [arithmetic logic unit](../../../../../arithmetic-logic-unit.md) add its inputs. The result returns to `wdata`; `RegWrite=1` writes it to $x$ at the active [clock edge](../../../../../clock-edge.md). The `zero` output is irrelevant here.[Question 1 datapath, printed page 2: the input-0 and input-1 multiplexer labels determine these control polarities](../../../../../digital-systems-linear-algebra-introduction-to-formal-proof-examination-paper-by-the-university-of-oxford-2014.md)

A [MIPS I-type instruction](../../../../../mips-i-type-instruction.md) instead has the [instruction encoding](../../../../../instruction-encoding.md)

$$
\underbrace{\mathrm{op}}_{6}\ \underbrace{\mathrm{rs}}_{5}\ \underbrace{\mathrm{rt}}_{5}\ \underbrace{\mathrm{immediate}}_{16}.
$$

For `addi $x,$y,n`, $\mathrm{rs}=y$, $\mathrm{rt}=x$, and the low sixteen [bits](../../../../../bit.md) contain the [immediate operand](../../../../../immediate-operand.md). The [register file](../../../../../register-file.md) supplies $y$ to the first [arithmetic logic unit](../../../../../arithmetic-logic-unit.md) input. Set `RegDst=0` to select [bits](../../../../../bit.md) 20:16 for the destination, and `ALUSrc=1` to select the extended [immediate operand](../../../../../immediate-operand.md) for the second input. The [opcode](../../../../../opcode.md) directly requests addition, so `ALUFunc=ADD` and `RegWrite=1`. The second [register file](../../../../../register-file.md) read is unused. The returned result is written into $x$.

The [sign extension](../../../../../sign-extension.md) circuit retains the low sixteen [bits](../../../../../bit.md) and copies [bit](../../../../../bit.md) 15 into all sixteen new high positions:

$$
\boxed{\operatorname{sext}(n)_{15:0}=n,\qquad \operatorname{sext}(n)_{31:16}=\underbrace{n_{15}\cdots n_{15}}_{16\text{ copies}}.}
$$

Thus [sign extension](../../../../../sign-extension.md) preserves the signed [two's complement](../../../../../two-s-complement.md) value: `0x7fff` becomes `0x00007fff`, whereas `0x8000` becomes `0xffff8000`. For both instructions, the architectural result above assumes no signed overflow; the full [MIPS architecture](../../../../../mips-architecture.md) specifies an overflow exception, which is outside this simplified [datapath](../../../../../datapath.md).

## ↑ Ancestors (12)

1. [A](../a.md)
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
