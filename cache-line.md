# Cache line

↑ **Parent:** [Cache (computing)](cache-computing.md)

A fixed-sized, aligned block of consecutive [bytes](byte.md) transferred and tracked as a unit by a data [memory cache](cache-computing.md). Here [cache line](cache-line.md) and [cache block](cache-line.md) name that unit of data, including its identity in backing [computer memory](computer-memory.md); a resident slot holds a copy. Reading one element can bring neighbouring elements into the same [cache line](cache-line.md), exploiting [spatial locality](spatial-locality.md).

For a nonnegative [integer](integer.md) [physical address](physical-address.md) $a$ and a [cache line](cache-line.md) size $B$ [bytes](byte.md), [Euclidean division](euclidean-division.md) gives the backing [cache block](cache-line.md) number $q$ and offset $d$:

$$
q=\left\lfloor\frac{a}{B}\right\rfloor,\qquad d=a\bmod B,\qquad a=Bq+d,\qquad 0\leq d<B.
$$

Here the brackets denote the [floor function](floor-function.md) and $\bmod$ gives the [remainder](remainder.md). [Cache line](cache-line.md) $q$ contains [bytes](byte.md) at [physical addresses](physical-address.md) $Bq$ through $Bq+B-1$. With $B=16$, read address 52 selects [cache block](cache-line.md) 3, spanning addresses 48–63, and offset 4. Addresses 48 and 52 therefore request the same [cache line](cache-line.md); addresses 15 and 16 request different [cache lines](cache-line.md) despite being adjacent.

<a id="image-physical-address-52-selects-cache-line-3-and-offset-4-the-resident-copy-occupies-cache-slot-0"></a>
![](cache-line-address-geometry.png)

**[Figure 73](#image-physical-address-52-selects-cache-line-3-and-offset-4-the-resident-copy-occupies-cache-slot-0). Physical address 52 selects cache line 3 and offset 4; the resident copy occupies cache slot 0**.

For a [cache line](cache-line.md) size $B=2^b$, the low $b$ [bits](bit.md) give the offset. In a [fully associative cache](fully-associative-cache.md), all remaining [bits](bit.md) identify the backing [cache block](cache-line.md) as its [cache tag](cache-tag.md); there are no address [bits](bit.md) selecting a particular [cache slot](cache-slot.md). An eight-[bit](bit.md) illustration gives $52=\mathtt{00110100}_2$: four [bits](bit.md) `0011` for [cache block](cache-line.md) 3 and four [bits](bit.md) `0100` for offset 4 in the [binary numeral system](binary-numeral-system.md). The eight-[bit](bit.md) width is illustrative; the trace does not assume an actual eight-[bit](bit.md) machine. [Memory part 2: CPU caches by Ulrich Drepper](memory-part-2-cpu-caches-by-ulrich-drepper.md)

Distinguish this identity from a [cache slot](cache-slot.md), which can hold different [cache blocks](cache-line.md) over time. After read nine in the [memory cache](cache-computing.md) example, [cache slot](cache-slot.md) 0 contains [cache line](cache-line.md) 3 and [cache slot](cache-slot.md) 1 contains [cache line](cache-line.md) 0. Their [cache tags](cache-tag.md) identify 3 and 0; neither [cache line](cache-line.md) number is its slot number. Some texts use “cache line” for the storage entry itself; this article reserves [cache slot](cache-slot.md) for that role.

**Table of contents**

- [Cache slot](cache-slot.md)
  - [Cache tag](cache-tag.md)

## ↑ Ancestors (4)

1. [Cache (computing)](cache-computing.md)
2. [Computer memory](computer-memory.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Cache (computing)](cache-computing.md)
- [Cache hit](cache-hit.md)
- [Cache line](cache-line.md)
- [Cache miss](cache-miss.md)
- [Cache slot](cache-slot.md)
- [Capacity miss](capacity-miss.md)
- [Conflict miss](conflict-miss.md)
- [Fully associative cache](fully-associative-cache.md)
- [Memory access trace](memory-access-trace.md)
- [Microkernel communication cost](microkernel-communication-cost.md)
- [Spatial locality](spatial-locality.md)
- [Temporal locality](temporal-locality.md)
