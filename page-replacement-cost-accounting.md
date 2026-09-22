# Page-replacement cost accounting

↑ **Parent:** [Page replacement](page-replacement.md)

Let $n$ be the number of accesses, $M$ the miss count and $D$ the number of dirty-victim [page writebacks](page-writeback.md). Assume every requested [memory page](memory-page.md) has a backing copy, every miss reads it, writes modify only part of its contents, transfers succeed and occur serially, and there is no background or final flushing. With common access cost $h$, additional load cost $r$ per miss, and additional outgoing write cost $w$ per dirty victim, an illustrative total service time is

$$
T=nh+Mr+Dw.
$$

Bookkeeping and other [operating system](operating-system-split.md) costs are omitted. The two transfer directions are separate: a miss can require a read with no write, or both a victim write and a requested-page read. A retained [dirty memory page](dirty-memory-page.md) contributes no outgoing write to this finite-[page-reference trace](page-reference-trace.md) count until evicted. Future flushing would need its own accounting boundary.

For three-[page frame](page-frame.md) [FIFO page replacement](fifo-page-replacement.md) on the displayed [page-reference trace](page-reference-trace.md), all reads give $(n,M,D)=(12,9,0)$. Change only access 1 to a partial write of [memory page](memory-page.md) 1. Its initial miss still loads the old contents, the write marks it dirty, and eviction at access 4 adds exactly one [page writeback](page-writeback.md). Later loads of [memory page](memory-page.md) 1 are clean because the remaining accesses read. The result is $(12,9,1)$: identical residency and nine misses, but one extra outgoing write. With illustrative $h=100$ nanoseconds, $r=1$ millisecond and $w=2$ milliseconds, total service time changes from $9.0012$ to $11.0012$ milliseconds. These are model costs, not hardware measurements.

Preferring a clean victim can save an immediate [page writeback](page-writeback.md), but evicting a soon-needed clean [memory page](memory-page.md) can add later misses. This tradeoff is why a miss-minimizing [optimal page replacement](optimal-page-replacement.md) benchmark and a minimum-cost policy are different questions. Real [page faults](page-fault.md) can also initialize a new [memory page](memory-page.md) or perform [copy-on-write](copy-on-write.md) without reading backing storage; those cases require different load costs.

// Destination: computer-science.bigb

## ↑ Ancestors (6)

1. [Page replacement](page-replacement.md)
2. [Paging](paging.md)
3. [Virtual memory](virtual-memory-split.md)
4. [Operating system](operating-system-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Page replacement](page-replacement.md)
