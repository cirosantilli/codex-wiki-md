<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [store buffer](../../../../../store-buffer.md) holds the [memory address](../../../../../memory-address.md) and value of a [store instruction](../../../../../store-instruction.md) while the [memory cache](../../../../../cache-computing.md) or backing [computer memory](../../../../../computer-memory-split.md) completes the write. The [in-order pipeline](../../../../../in-order-pipeline.md) can continue after enqueueing the write, rather than waiting for a possibly long [memory access latency](../../../../../memory-access-latency.md). A full [store buffer](../../../../../store-buffer.md) eventually causes a [pipeline stall](../../../../../pipeline-stall.md); buffering hides finite delays, not an indefinitely inadequate service rate.

Without a [memory management unit](../../../../../memory-management-unit.md), the comparison can use the actual [physical addresses](../../../../../physical-address.md); there is no [address translation](../../../../../address-translation.md) or synonym problem to solve. Suppose `x` initially contains zero and these operations execute in order:
```
STORE [x], 7
LOAD  r1, [x]
```
If the write is still in the [store buffer](../../../../../store-buffer.md), reading only [computer memory](../../../../../computer-memory-split.md) could incorrectly return zero. The [load instruction](../../../../../load-instruction.md) searches older buffered [store instructions](../../../../../store-instruction.md) for an overlapping [memory address](../../../../../memory-address.md). If the newest matching write covers the requested [bytes](../../../../../byte.md) and its data are ready, [store-to-load forwarding](../../../../../store-to-load-forwarding.md) returns seven directly. With several pending writes to `x`, the youngest older matching write wins. If the relevant data are not ready, the [load instruction](../../../../../load-instruction.md) waits; partial overlaps require merging the covered [bytes](../../../../../byte.md) or conservatively waiting for the writes to drain.

A [load instruction](../../../../../load-instruction.md) from an unrelated address `y` can bypass those buffered writes, subject to the architecture's [memory model](../../../../../memory-model.md). **Buffer writes to overlap them with useful execution, but preserve each load's dependence on older writes to the same bytes.** Device accesses through [memory-mapped input-output](../../../../../memory-mapped-input-output.md) need their specified ordering and should not be treated as ordinary cacheable [computer memory](../../../../../computer-memory-split.md).

$$
\boxed{\text{Buffer stores, but forward or wait when a later load overlaps them.}}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Computer architecture](../../../computer-architecture-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
