<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In a cooperative scheduler, a permanently runnable background [operating-system process](../../../../../process-computing.md) that never yields can monopolize the [CPU](../../../../../central-processing-unit.md). The timer service, smoothing [operating-system process](../../../../../process-computing.md), and display may then fail to run even when their messages are ready. Correct [message passing](../../../../../message-passing.md) alone does not supply [process scheduling](../../../../../process-scheduling.md).

Use **timer-driven [scheduling preemption](../../../../../scheduling-preemption.md)**, so an [interrupt](../../../../../interrupt.md) can force a [context switch](../../../../../context-switch.md) without cooperation. To give the measurement and display work bounded response despite background computation, use [priority scheduling](../../../../../priority-scheduling.md) with the background [operating-system process](../../../../../process-computing.md) below the responsive services, or an explicit reservation policy. [Round-robin scheduling](../../../../../round-robin-scheduling.md) gives CPU access among a fixed finite runnable set, but meeting a particular deadline additionally requires bounded service execution and sufficient CPU capacity.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
