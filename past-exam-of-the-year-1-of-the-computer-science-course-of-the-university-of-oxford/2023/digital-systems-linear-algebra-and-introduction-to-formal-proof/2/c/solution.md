<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**A [LIFO stack](../../../../../stack-data-structure.md) can make waiting clients starve.** Suppose client $A$ waits at the bottom of the [stack](../../../../../stack-data-structure.md). Before each current owner releases, a fresh client submits a request. That newest request is pushed above $A$ and is selected next. Every animation can finish promptly while $A$ waits forever.

This is [LIFO starvation](../../../../../lifo-starvation.md): service completion alone does not ensure [starvation freedom](../../../../../starvation-freedom.md). A [FIFO queue](../../../../../fifo-queue.md) prevents newer same-priority requests from passing $A$, whereas replacing either priority-class [FIFO queue](../../../../../fifo-queue.md) by a [LIFO stack](../../../../../stack-data-structure.md) adds this problem even within one priority class. Strict priority can already starve ordinary work, as in (b); the [LIFO stack](../../../../../stack-data-structure.md) introduces a further unfairness that can also affect urgent work.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [Digital systems](../../digital-systems.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
