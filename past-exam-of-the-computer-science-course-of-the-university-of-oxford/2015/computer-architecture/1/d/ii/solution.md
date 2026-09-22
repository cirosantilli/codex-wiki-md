<h1 id="1/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Define `PREFETCH [a]` as a [software prefetch](../../../../../../software-prefetch.md) hint: initiate a request for the [cache line](../../../../../../cache-line.md) containing [memory address](../../../../../../memory-address.md) `a`, then continue without waiting for that [cache line](../../../../../../cache-line.md) to arrive. It produces no value in a destination [processor register](../../../../../../processor-register.md), changes no program data and creates no data-result dependence for later instructions. It may be ignored if resources are unavailable. A useful hint is nonfaulting for an inaccessible or untranslated target: a later real [load instruction](../../../../../../load-instruction.md) must still perform its ordinary access checks. This is a proposed contract for the instruction, rather than a guarantee that the patent abstract alone fixes every detail of its semantics.

For example, after reading the next [pointer](../../../../../../pointer-computer-programming.md) of a [linked list node](../../../../../../linked-list-node.md), prefetch that next [linked list node](../../../../../../linked-list-node.md) while processing the current one. Replacing the hint by an otherwise unused ordinary [load instruction](../../../../../../load-instruction.md) on this [in-order pipeline](../../../../../../in-order-pipeline.md) would wait in MEM on a [cache miss](../../../../../../cache-miss.md) before the current computation could start. It would also consume a destination [processor register](../../../../../../processor-register.md) and might raise a [synchronous processor exception](../../../../../../synchronous-processor-exception.md). A harmless hint can be scheduled earlier, even on a path where the data will never be demanded. **The crucial semantic difference is that cache filling may continue after the prefetch instruction itself has finished.**

A [software prefetch](../../../../../../software-prefetch.md) is not a [memory barrier](../../../../../../memory-barrier.md) and does not establish [acquire-release synchronization](../../../../../../acquire-release-synchronization.md) or promise that later accesses will hit. Its purpose is performance; correctness must survive the hint being ignored.

$$
\boxed{\text{A nonblocking hint produces no register result and may be ignored.}}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Computer architecture](../../../../computer-architecture-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
