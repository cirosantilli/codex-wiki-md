<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Execute this [MIPS instruction](../../../../../../mips-instruction.md) fragment twice, once with equal operands and once with unequal operands, and observe whether its conditional branch is taken:
```
beq $t0, $t1, hit
sll $zero, $zero, 0
sll $zero, $zero, 0
hit:
sll $zero, $zero, 0
```
Use `$t0=7,$t1=7` for the first test and `$t0=7,$t1=8` for the second. All padding instructions are explicit harmless [MIPS instructions](../../../../../../mips-instruction.md). In the pictured single-cycle model, the next [program counter](../../../../../../instruction-pointer.md) after `beq` is either `hit` or the sequential address. The branch target is deliberately different from the next sequential instruction. The extra padding also keeps a [branch delay slot](../../../../../../branch-delay-slot.md) harmless if a test fixture uses an implementation with one, although the pictured model itself has none.

A healthy `zero` line reports the first subtraction as zero and the second as nonzero. A line stuck at zero prevents both branches, while a line stuck at one forces both branches. Therefore

$$
\boxed{\begin{array}{c|c}
\text{zero state}&(\text{equal test taken},\text{unequal test taken})\\\hline
\text{normal}&(\text{yes},\text{no})\\
\text{stuck at 0}&(\text{no},\text{no})\\
\text{stuck at 1}&(\text{yes},\text{yes})
\end{array}}
$$

Observe the branch decision or execution trace itself; an alleged unconditional `beq` used to skip result-recording code would also be affected by the fault.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
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
