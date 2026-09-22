<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Store **three state bits**: a two-bit index $L\in\{0,1,2,3\}$ identifying the most recent recipient, and a valid bit $V$ indicating whether that recipient is receiving service in the current cycle. Then

$$
g_i=V\land[L=i].
$$

When no requests are present at a decision edge, clear $V$ but preserve $L$. Preserving $L$ implements [round-robin arbitration with idle memory](../../../../../round-robin-arbitration-with-idle-memory.md). Four possible last recipients each have an active and an idle state, giving eight states. The four idle states have equal outputs but different future priorities, so they cannot all be merged. One valid reset is $L=3,V=0$, which gives requester zero first priority at startup.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
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
