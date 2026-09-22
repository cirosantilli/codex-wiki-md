<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A writing [MIPS instruction](../../../../../../mips-instruction.md) distinguishes a line stuck at zero. With `$t0=7`, `$t1=5`, `$t2=99`, execute
```
add $t2, $t0, $t1
```
A healthy line or a line stuck at one produces `$t2=12`; a line stuck at zero leaves `$t2=99`.

To distinguish normal operation from stuck at one, execute a normally nonwriting [MIPS instruction](../../../../../../mips-instruction.md). The following functional test uses the usual concrete controller choice `MemToReg=0` during `sw`, selecting the [ALU](../../../../../../arithmetic-logic-unit.md) result on the write-data bus. Prepare `$t0=37` and `$s0=L-16384`, for an aligned writable address $L\ne37$, then execute
```
sw $t0, 16384($s0)
```
The [ALU](../../../../../../arithmetic-logic-unit.md) computes $L$. Here `rt` is register 8 (`$t0`), and immediate $16384=\mathtt{0x4000}$ also puts 8 into bits $15\ldots11$. Thus either value of the otherwise irrelevant `RegDst` selects `$t0`. With a healthy `RegWrite`, `$t0` remains 37. With `RegWrite` stuck at one and the specified write-data selection, the unwanted [register file](../../../../../../register-file.md) write changes `$t0` to $L$. Combining the two independent observations gives

$$
\boxed{\begin{array}{c|c}
\text{RegWrite state}&(t2\text{ after add},t0\text{ after store})\\\hline
\text{normal}&(12,37)\\
\text{stuck at 0}&(99,37)\\
\text{stuck at 1}&(12,L)
\end{array}}
$$

**Controller qualification.** The source diagram does not specify values of otherwise irrelevant control outputs during a store. `MemToReg` is a [don't-care condition](../../../../../../don-t-care-term.md) when `RegWrite=0`; its chosen implementation matters when that enable line is faulty. The functional test above explicitly fixes this convention instead of assuming that all implementations resolve it identically. A manufacturing fixture can also observe the [register file](../../../../../../register-file.md) write-enable directly while executing `add` followed by `sw`: the expected pairs are $(1,0)$ normally, $(0,0)$ stuck at zero, and $(1,1)$ stuck at one. This second observation does not depend on unused write-data controls or on whether an unwanted write happens to repeat an old value.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
