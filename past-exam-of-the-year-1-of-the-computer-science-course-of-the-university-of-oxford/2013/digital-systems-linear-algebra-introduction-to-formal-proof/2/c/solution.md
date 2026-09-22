<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose `ToAlu=0` for the $val_t$ input and `ToAlu=1` for the expanded [immediate operand](../../../../../immediate-operand.md). Choose `ToReg=0` for the [arithmetic logic unit](../../../../../arithmetic-logic-unit.md) result and `ToReg=1` for memory read data. The diagram does not label the [multiplexer](../../../../../multiplexer.md) polarities, so these are explicit conventions.

Let $F_+$ and $F_{\lor}$ denote the six-bit [arithmetic logic unit](../../../../../arithmetic-logic-unit.md) operation codes for addition and [bitwise OR](../../../../../bitwise-or.md). Their numerical codes are not specified by the paper. The [opcode](../../../../../opcode.md) needs to distinguish register, immediate, load and store modes; `add` and `or` can share register mode, and `addi` and `ori` can share immediate mode, since $15:10$ selects the operation directly. For example, choose $o_R=000000$, $o_I=000001$, $o_L=000010$ and $o_S=000011$. With $X$ denoting a field whose bits do not matter, the formats are:

<a id="2/c/table-one-consistent-allocation-of-instruction-encoding-fields"></a>
| Instruction | $31:26$ | $25:21$ | $20:16$ | $15:10$ | $9:5$ | $4:0$ |
| --- | --- | --- | --- | --- | --- | --- |
| `add d,s,t` | $o_R$ | $s$ | $d$ | $F_+$ | $t$ | $X$ |
| `or d,s,t` | $o_R$ | $s$ | $d$ | $F_{\lor}$ | $t$ | $X$ |
| `addi d,s,x` | $o_I$ | $s$ | $d$ | $F_+$ | Upper five bits of $x$ | Lower five bits of $x$ |
| `ori d,s,x` | $o_I$ | $s$ | $d$ | $F_{\lor}$ | Upper five bits of $x$ | Lower five bits of $x$ |
| `load d,(s)` | $o_L$ | $s$ | $d$ | $X$ | $X$ | $X$ |
| `store t,(s)` | $o_S$ | $s$ | $0$ | $X$ | $t$ | $X$ |

The required [opcode](../../../../../opcode.md) control table is:

<a id="2/c/table-control-values-required-by-the-pictured-datapath"></a>
| Mode and instructions | `ToAlu` | `MemWr` | `MemRd` | `ToReg` |
| --- | --- | --- | --- | --- |
| $o_R$: `add`, `or` | $0$ | $0$ | $X$ | $0$ |
| $o_I$: `addi`, `ori` | $1$ | $0$ | $X$ | $0$ |
| $o_L$: `load` | $X$ | $0$ | $1$ | $1$ |
| $o_S$: `store` | $0$ | $1$ | $X$ | $X$ |

Here `MemRd` is irrelevant whenever read data is unused, under the ordinary side-effect-free memory interpretation of the diagram. It is sensible to choose zero for those $X$ entries to save activity; memory-mapped devices with read side effects would require that choice. For `store`, `ToReg` is irrelevant because $r_d=0$; `ToAlu` is essential because its output supplies **both** the second [arithmetic logic unit](../../../../../arithmetic-logic-unit.md) operand and memory write data. For `load`, the memory address is $val_s$ independently of `ToAlu` and of $15:10$.

The resulting effects, with 32-bit addition, are

$$
\boxed{\begin{aligned}
\operatorname{add}:&\quad R_d\gets R_s+R_t,&\operatorname{or}:&\quad R_d\gets R_s\mathbin{\vert}R_t,\\
\operatorname{addi}:&\quad R_d\gets R_s+E(x),&\operatorname{ori}:&\quad R_d\gets R_s\mathbin{\vert}E(x),\\
\operatorname{load}:&\quad R_d\gets M[R_s],&\operatorname{store}:&\quad M[R_s]\gets R_t,
\end{aligned}}
$$

where $E(x)=(x\bmod256)2^{8\lfloor x/256\rfloor}$ for the ten-bit field $x$.

## ↑ Ancestors (12)

1. [C](../c.md)
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
