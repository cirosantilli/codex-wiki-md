<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The `addi` [immediate operand](../../../../../immediate-operand.md) is a [byte-lane immediate](../../../../../byte-lane-immediate.md): an unsigned eight-bit quantity shifted by $0,8,16$ or $24$ positions. Thus

$$
\boxed{E(x)=b2^{8j},\qquad 0\leq b\leq255,\quad 0\leq j\leq3.}
$$

It is not the [sign extension](../../../../../sign-extension.md) of a 16-bit constant used by the [MIPS instruction](../../../../../mips-instruction.md) `addi`. For example, this design can add $\mathtt{0x12000000}$ directly, but cannot add $\mathtt{0x00000123}$ in a single immediate instruction. A field containing byte $\mathtt{FF}$ in the low lane adds 255, not $-1$.

The `load` and `store` memory address is exactly the content of $r_s$. The [arithmetic logic unit](../../../../../arithmetic-logic-unit.md) result is not connected to the memory-address input. Therefore

$$
\boxed{\text{native address}=R_s,\qquad\text{MIPS address}=R_s+\operatorname{signextend}_{16}(\text{offset}).}
$$

There is no native base-plus-offset calculation during either memory instruction. The paper does not specify exception behavior for signed overflow, so the representable constants and address calculation are the justified differences; the [datapath](../../../../../datapath.md) alone cannot establish MIPS-compatible overflow traps.

## ↑ Ancestors (12)

1. [D](../d.md)
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
