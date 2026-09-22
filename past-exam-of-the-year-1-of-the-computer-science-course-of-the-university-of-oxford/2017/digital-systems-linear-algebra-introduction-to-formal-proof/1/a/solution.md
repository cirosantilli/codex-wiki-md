<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use four request [bits](../../../../../bit.md) $r_0,r_1,r_2,r_3$ and four grant bits $g_0,g_1,g_2,g_3$. A high $r_i$ requests service for the coming allocation period, and a high $g_i$ identifies the requester granted the resource during the current period. At most one grant may be high. An all-zero grant vector means idle. The [synchronous sequential circuit](../../../../../synchronous-sequential-circuit.md) also has a [clock](../../../../../clock.md) and an initialization signal.

Requests are sampled at a [clock edge](../../../../../clock-edge.md); the resulting allocation appears during the following cycle. This fixes the [Moore machine](../../../../../moore-machine.md) timing convention: current grants depend on the stored state, rather than combinationally on requests that can change within the cycle.

## ↑ Ancestors (12)

1. [A](../a.md)
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
