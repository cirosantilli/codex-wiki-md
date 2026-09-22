<h1 id="1/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Cache prefetching](../../../../../../cache-prefetching.md) moves a [cache line](../../../../../../cache-line.md) towards the [CPU](../../../../../../central-processing-unit.md) before a demand access needs it. A correctly timed request overlaps the [cache miss penalty](../../../../../../cache-miss-penalty.md) with earlier computation, so a subsequent [load instruction](../../../../../../load-instruction.md) can find a [cache hit](../../../../../../cache-hit.md) instead of stopping the [in-order pipeline](../../../../../../in-order-pipeline.md) in MEM. Requests directed at several levels of a [cache hierarchy](../../../../../../cache-hierarchy.md) can prepare nearby data in a small fast [memory cache](../../../../../../cache-computing.md) while staging more distant future data in larger levels. The separate request [computer bus](../../../../../../computer-bus.md) avoids making those address requests compete directly with returning data; returned [cache lines](../../../../../../cache-line.md) still consume transfer capacity.

For a [store instruction](../../../../../../store-instruction.md), the gain depends on the write policy. With a [write-allocate cache](../../../../../../write-allocate-cache.md), fetching its target [cache line](../../../../../../cache-line.md) early can avoid the allocation [cache miss](../../../../../../cache-miss.md) and help the [store buffer](../../../../../../store-buffer.md) drain. On a [multicore processor](../../../../../../multicore-processor.md), a write-oriented prefetch may additionally obtain [cache coherence](../../../../../../cache-coherence.md) ownership; an ordinary read prefetch alone does not guarantee write permission. A [store buffer](../../../../../../store-buffer.md) can already hide an individual write's [latency](../../../../../../latency-engineering.md), so the visible gain may appear only when it would otherwise fill. With a [no-write-allocate cache](../../../../../../no-write-allocate-cache.md), fetching the [cache line](../../../../../../cache-line.md) just to overwrite it can be unnecessary. **Loads benefit directly from earlier data arrival; stores benefit when prefetching removes a required allocation or ownership delay.**

$$
\boxed{\text{Overlap cache filling with work before a demand access.}}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
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
