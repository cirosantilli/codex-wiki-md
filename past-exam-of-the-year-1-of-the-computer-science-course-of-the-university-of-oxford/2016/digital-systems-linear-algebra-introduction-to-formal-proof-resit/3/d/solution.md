<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At 6000 revolutions per minute the disk makes 100 revolutions per second, so one turn takes 10 ms and the mean [rotational latency](../../../../../rotational-latency.md) is 5 ms. Adding [seek time](../../../../../seek-time.md), [data transfer time](../../../../../data-transfer-time.md) and controller overhead gives, using decimal MB,

$$
\boxed{12+5+\frac{512}{5\cdot10^6}\,10^3+2=19.1024\text{ ms}\approx19.1\text{ ms}.}
$$

Using $1\mathrm{MB}=2^{20}$ bytes instead gives 19.09765625 ms, with the same rounded answer. The calculation assumes the stated rate applies to the sector transfer and that the seek and overhead are each paid once.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof (resit)](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
