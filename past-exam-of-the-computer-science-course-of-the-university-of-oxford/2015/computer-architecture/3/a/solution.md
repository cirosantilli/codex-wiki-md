<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A small [memory cache](../../../../../cache-computing.md) close to the [CPU](../../../../../central-processing-unit.md) can be accessed quickly, but cannot hold the entire useful data set. Increasing its capacity usually increases lookup, wiring and energy costs. A [cache hierarchy](../../../../../cache-hierarchy.md) combines a small fast first level with progressively larger levels that reduce the number of accesses reaching slow main [computer memory](../../../../../computer-memory-split.md).

In a simple serial two-level timing model, let $t_1$ be the first-level lookup time, $m_1$ its [cache miss rate](../../../../../cache-miss-rate.md), $t_2$ the additional second-level lookup time, $m_2$ the second level's local [cache miss rate](../../../../../cache-miss-rate.md) conditional on a first-level miss, and $t_M$ the remaining main-memory cost. Then

$$
\boxed{\operatorname{AMAT}=t_1+m_1(t_2+m_2t_M).}
$$

This [average memory access time](../../../../../average-memory-access-time.md) combines the common fast path with a rarer large-capacity path. **Several levels balance hit latency, capacity, cost and traffic; making one cache very large does not preserve a tiny first-level hit time.** [Temporal locality](../../../../../temporal-locality.md) and [spatial locality](../../../../../spatial-locality.md) make this arrangement useful.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Computer architecture](../../../computer-architecture-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
