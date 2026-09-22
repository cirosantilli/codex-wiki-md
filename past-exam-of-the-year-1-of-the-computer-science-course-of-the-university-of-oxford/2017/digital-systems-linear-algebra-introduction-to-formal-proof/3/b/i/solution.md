<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Keep storage only for registers 1 through 31, return a hardwired all-zero word on either read port when its address is zero, and set

$$
\boxed{we_i=[\mathrm{wa}=i],\qquad i=1,\ldots,31.}
$$

There is no enable for register zero and no global RegWrite input to this [register file](../../../../../../register-file.md). The right-hand diagram above shows this change. Every clock edge may select a write address; choosing zero suppresses all physical register enables. Consequently the [MIPS zero register](../../../../../../mips-zero-register.md) acts as a [write-suppression destination](../../../../../../write-suppression-destination.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Digital systems, linear algebra, introduction to formal proof](../../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
