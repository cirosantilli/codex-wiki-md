<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use [round-robin scheduling](../../../../../round-robin-scheduling.md) with [scheduling quantum](../../../../../scheduling-quantum.md) 2 ms. A's first burst is split by B, and A's second burst is also interrupted once. The resulting CPU intervals are

$$
\begin{array}{c|rrrrrrrrrrr}
\text{interval}&0\!:\!2&2\!:\!3&3\!:\!5&5\!:\!6&6\!:\!7&7\!:\!9&9\!:\!10&10\!:\!12&12\!:\!14&14\!:\!16&16\!:\!18\\
\text{CPU}&A&B&A&B&\text{idle}&A&B&A&\text{idle}&A&A
\end{array}
$$

A blocks for input-output during $[5,7)$ and $[12,14)$; B blocks during $[3,5)$ and $[6,8)$. At time 8, B joins the [ready queue](../../../../../ready-queue.md) while A uses the remainder of its current quantum; B runs at time 9. No other process is runnable during A's final four milliseconds, so A can continue across the time-16 quantum boundary. Consequently

$$
\boxed{C_B=10,\quad C_A=18,\quad\text{elapsed time}=18\text{ ms},\quad\text{mean turnaround}=14\text{ ms}.}
$$

## ↑ Ancestors (12)

1. [E](../e.md)
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
