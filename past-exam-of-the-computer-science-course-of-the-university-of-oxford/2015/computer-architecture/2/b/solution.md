<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [reorder buffer](../../../../../reorder-buffer.md) records instructions in program order, including those with no destination [processor register](../../../../../processor-register.md). Each entry needs a completion state before [instruction retirement](../../../../../instruction-retirement.md) can pass it. Thus a [store instruction](../../../../../store-instruction.md) must report that its [memory address](../../../../../memory-address.md) and data are ready and whether execution detected a fault, even though it has no ordinary [register file](../../../../../register-file.md) result.

Suppose an older division occupies the head of the [reorder buffer](../../../../../reorder-buffer.md), followed by a [store instruction](../../../../../store-instruction.md) and an addition. The latter two can finish first. The [store instruction](../../../../../store-instruction.md)'s completion message identifies its [reorder buffer](../../../../../reorder-buffer.md) entry, carries or identifies the buffered [memory address](../../../../../memory-address.md) and data, and supplies its status. The entry is then ready, but its write remains private until it is the oldest instruction allowed to commit. When the division retires successfully, the [store instruction](../../../../../store-instruction.md) can commit to the [store buffer](../../../../../store-buffer.md) or memory system, and the addition can subsequently retire. If the division faults, the younger [store instruction](../../../../../store-instruction.md) is discarded without changing visible [computer memory](../../../../../computer-memory-split.md).

If the [store instruction](../../../../../store-instruction.md) never reported completion, its [reorder buffer](../../../../../reorder-buffer.md) entry would remain unready and block [instruction retirement](../../../../../instruction-retirement.md) indefinitely. Conversely, treating it as completed at issue could commit missing data or suppress its later fault. **The common data bus carries tagged completion information as well as register values.** A false-predicated instruction also needs a completion indication even when it changes no data.

This answer uses the diagram's shared result/completion path. An architecture can instead provide a dedicated [store queue](../../../../../store-queue.md) completion path to the [reorder buffer](../../../../../reorder-buffer.md); there is no universal requirement to send store data over the same physical wires as arithmetic results. What is essential is delivery of the tagged completion and exception status before [instruction retirement](../../../../../instruction-retirement.md).

$$
\boxed{\text{Stores need tagged completion before the ROB can retire them.}}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Computer architecture](../../../computer-architecture-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
