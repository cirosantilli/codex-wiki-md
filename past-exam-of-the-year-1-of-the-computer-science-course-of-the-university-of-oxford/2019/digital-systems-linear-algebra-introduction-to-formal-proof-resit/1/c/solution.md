<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Count executed instructions, excluding the caller's branch-with-link and assuming the register-return and stack instructions shown above. The shift loop executes six instructions per iteration, plus four entry instructions and three exit instructions: **$6\cdot32+7=199$ instructions**. The unrolled table subroutine executes **21 instructions**, including four byte loads.

If every instruction, including a table load and a branch, costs one time unit, the ratio is **$199/21\approx9.48$** in favour of the table version. A more informative simple model assigns cost $L$ to each table load and unit cost to the other displayed instructions: its cost is $17+4L$, versus 199 for the loop under the same unit branch assumption. Thus this model favours lookup when $L<45.5$.

Real [running time](../../../../../running-time.md) depends on the processor and memory system. Taken branches can incur extra instruction-fetch or pipeline costs, favouring the unrolled version; slow flash or [cache miss](../../../../../cache-miss.md) events on the 256-byte table can erode that advantage. Instruction and table placement also matter. These assumptions prevent instruction counts from becoming an unsupported universal cycle claim. For a fixed 32-bit argument both implementations have constant worst-case work; the gain is a constant factor, not a different asymptotic class.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
