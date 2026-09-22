<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume both processes are available at time zero and run the listed order, A followed by B, with no overlap even during [input-output](../../../../../input-output.md). A takes $12+4=16$ ms; B then takes $3+4=7$ ms. Thus

$$
\boxed{\text{elapsed time}=23\text{ ms},\qquad\text{mean turnaround}=\frac{16+23}{2}=19.5\text{ ms}.}
$$

The [scheduling turnaround time](../../../../../scheduling-turnaround-time.md) includes the time waiting before a process first runs. Reversing the serial order would leave the total at 23 ms but change completion times to 7 and 23 ms, with mean 15 ms. If arrivals were instead delayed until each serial launch, that would define a different turnaround measurement; the simultaneous-arrival convention is used for comparing the schedulers below.

## ↑ Ancestors (12)

1. [C](../c.md)
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
