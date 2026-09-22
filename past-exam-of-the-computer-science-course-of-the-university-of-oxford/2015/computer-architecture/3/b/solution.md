<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use two different shared locations `x` and `y`, initially zero, and two [CPU cores](../../../../../cpu-core.md). The following are architectural memory operations, with each result kept in its own [processor register](../../../../../processor-register.md):

| Core 0 | Core 1 |
| --- | --- |
| `STORE [x], 1` | `STORE [y], 1` |
| `LOAD r0, [y]` | `LOAD r1, [x]` |

Each [CPU core](../../../../../cpu-core.md) can retire its write into its own [store buffer](../../../../../store-buffer.md). Before either write drains, Core 0's [load instruction](../../../../../load-instruction.md) misses its own [store buffer](../../../../../store-buffer.md) because it asks for `y`, while Core 1's asks for `x`. Both can read the old shared values. Afterwards the buffers drain and both locations become one. Thus

$$
\boxed{r_0=r_1=0\quad\text{is possible with separate store buffers}.}
$$

There is no contradiction with [cache coherence](../../../../../cache-coherence.md): each location still has an agreed write order. The unusual observation concerns ordering across two different locations. This is the standard store-buffering example, also permitted by [total store order](../../../../../total-store-order.md).[§2.1, “SB: Store Buffering”, printed p. 2](../../../../../understanding-power-multiprocessors-2011.md)

On a single [CPU core](../../../../../cpu-core.md) executing the two logical participants in an ordinary [thread interleaving](../../../../../thread-interleaving.md), the same pair of zero observations is impossible under the usual shared-buffer and own-write-forwarding behavior. To read `y=0`, Core-0's logical read must precede the other participant's write of `y`; to read `x=0`, the other read must precede the write of `x`. Combining these requirements with each participant's program order gives the impossible cycle

$$
W_x<R_y<W_y<R_x<W_x.
$$

If a write is still buffered across a context switch on that single [CPU core](../../../../../cpu-core.md), a later read of the same address sees it through [store-to-load forwarding](../../../../../store-to-load-forwarding.md) rather than returning an older value. Hence separate [store buffers](../../../../../store-buffer.md) on different [CPU cores](../../../../../cpu-core.md) enable the observation; the comparison assumes ordinary coherent cacheable [computer memory](../../../../../computer-memory-split.md) and no device accesses or additional writes. **A locally completed store need not yet be visible to another core.**

## ↑ Ancestors (11)

1. [B](../b.md)
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
