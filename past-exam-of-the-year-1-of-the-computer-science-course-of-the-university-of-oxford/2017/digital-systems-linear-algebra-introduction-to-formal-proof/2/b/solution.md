<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With [nonpreemptive scheduling](../../../../../nonpreemptive-scheduling.md), a running process retains the processor until it finishes its current [CPU burst](../../../../../cpu-burst.md), blocks or voluntarily yields. With [preemptive scheduling](../../../../../preemptive-scheduling.md), the operating system may suspend a runnable process and select another one.

Time-slice preemption needs a **[hardware timer](../../../../../hardware-timer.md) delivering an [interrupt](../../../../../interrupt.md)** after bounded execution time, so control returns to the scheduler even if the running program never yields. Saving and restoring the [execution context](../../../../../execution-context.md) then lets the interrupted process resume later. The timer mechanism should remain under operating-system control.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
