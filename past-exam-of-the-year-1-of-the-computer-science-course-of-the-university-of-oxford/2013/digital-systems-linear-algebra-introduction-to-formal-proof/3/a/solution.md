<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [hard disk drive](../../../../../hard-disk-drive.md) pays substantial [seek time](../../../../../seek-time.md) to position the head and [rotational latency](../../../../../rotational-latency.md) to reach the desired sector. After that positioning, neighboring bytes stream past the head quickly. A larger transfer therefore amortizes positioning and command overhead over many bytes.

The physical sector also needs framing, synchronization and error-correcting redundancy. Transferring one byte at a time would spend an excessive fraction of the medium and controller work on that overhead. A controller buffer and a block transfer can efficiently deliver the sector to [computer memory](../../../../../computer-memory-split.md), often using [direct memory access](../../../../../direct-memory-access.md).

Thus

$$
\boxed{\text{larger transfers amortize positioning, framing and command costs}.}
$$

The choice is a compromise: excessively large blocks waste transfer time for small requests and can increase [internal fragmentation](../../../../../internal-fragmentation.md) in a [file system](../../../../../file-system-split.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
