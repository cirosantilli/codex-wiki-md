<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Reusing a block-oriented [file system](../../../../../file-system-split.md) preserves existing operating-system interfaces, tools, consistency procedures and on-disk formats. It also permits common buffering and caching policies. Large transfers can still amortize software and controller overhead, and [flash memory](../../../../../flash-memory.md) itself has page-program and erase-block constraints, so a [block device](../../../../../block-device.md) abstraction is often useful even without mechanical motion.

The costs are that a fine-grained change may require reading and rewriting a larger logical block, and a small [computer file](../../../../../computer-file.md) can waste part of its final [file data block](../../../../../file-data-block.md). Structures optimized to reduce [seek time](../../../../../seek-time.md) need not be best for [non-volatile memory](../../../../../non-volatile-memory.md). For [flash memory](../../../../../flash-memory.md), repeated metadata updates and erasing or relocating larger regions can increase physical writes and consume finite program/erase endurance. A translation layer can hide these constraints but adds mapping space and work.

Consequently

$$
\boxed{\text{compatibility and reuse trade against wasted space, extra writes and missed device-specific optimizations}.}
$$

The balance depends on the actual medium: byte-addressable [non-volatile memory](../../../../../non-volatile-memory.md) and page/erase-based [flash memory](../../../../../flash-memory.md) have different physical constraints.

## ↑ Ancestors (12)

1. [B](../b.md)
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
