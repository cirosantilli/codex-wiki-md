<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Decompose the 32-bit pattern of $n$ into bytes:

$$
n\equiv b_0+2^8b_1+2^{16}b_2+2^{24}b_3\pmod{2^{32}},\qquad 0\leq b_j\leq255.
$$

Let $x_j=256j+b_j$ be its ten-bit encoding, so $E(x_j)=b_j2^{8j}$. The following custom-ISA [assembly language](../../../../../assembly-language.md) sequence implements the requested sum:

```
addi t,s,x0
addi t,t,x1
addi t,t,x2
addi t,t,x3
```

The symbols `x0` through `x3` stand for the **encoded ten-bit fields**, not for the expanded 32-bit values. After line $j+1$, the destination contains $R_s+\sum_{i=0}^jb_i2^{8i}$ [modulo](../../../../../modulo-operation.md) $2^{32}$. Hence

$$
\boxed{R_t\gets R_s+n\pmod{2^{32}}\quad\text{in at most four instructions}.}
$$

If $t=s$, each instruction correctly uses the preceding partial sum. Zero-byte additions can be omitted except that, when $t\ne s$, an initial instruction must still copy the original source if all earlier omitted bytes are zero. An [assembler](../../../../../assembler.md) can initialize `t` with `add t,s,0` instead and then emit only nonzero lanes. If $t=0$, the intended register effect is discarded.

For a [MIPS instruction](../../../../../mips-instruction.md) `lw t,k(s)`, first construct $R_u=R_s+\operatorname{signextend}_{16}(k)$ in a scratch [processor register](../../../../../processor-register.md) $u$, using the four-lane sequence above with destination $u$, and then issue

```
load t,(u)
```

For `sw t,k(s)`, construct the same address in $u$ and issue

```
store t,(u)
```

Choose $u\ne0,s,t$, or preserve a live scratch [processor register](../../../../../processor-register.md) according to the calling convention. In particular the store sequence must retain the original data in $t$, even when $s=t$. Both expansions need at most five custom instructions and have the same address and memory-word effects as the corresponding [MIPS instructions](../../../../../mips-instruction.md), assuming aligned valid memory and 32-bit modular address arithmetic. When $k=0$, the memory instruction alone suffices. These are listings for the examination's custom [instruction set architecture](../../../../../instruction-set-architecture.md), not native MIPS encodings; exact exception and pipeline behavior is outside the specified [datapath](../../../../../datapath.md).

## ↑ Ancestors (12)

1. [E](../e.md)
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
