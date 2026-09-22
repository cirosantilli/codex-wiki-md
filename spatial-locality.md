# Spatial locality

↑ **Parent:** [Computer science](computer-science-split.md)

Spatial locality is the tendency to access nearby locations in [computer memory](computer-memory.md) within a short interval. A sequential scan of a contiguous [array](array-data-structure.md) has [spatial locality](spatial-locality.md) even when each element is read only once. A [memory cache](cache-computing.md) can exploit [spatial locality](spatial-locality.md) by fetching a whole [cache line](cache-line.md) on a [cache miss](cache-miss.md): later reads of neighbouring elements become [cache hits](cache-hit.md). Proximity is in the address layout, so visually adjacent entries in a table need not be adjacent [bytes](byte.md).

Consider a $4\times4$ [array](array-data-structure.md) of 32-[bit](bit.md) [integers](integer.md), each occupying four eight-[bit](bit.md) [bytes](byte.md), stored contiguously in [row-major order](row-major-order.md). Use toy [physical addresses](physical-address.md) starting at zero, aligned to a 16-[byte](byte.md) [cache line](cache-line.md) boundary. For row $i$ and column $j$, with $0\leq i,j<4$, the address and [cache block](cache-line.md) number are

$$
\operatorname{address}(i,j)=4(4i+j),\qquad
\operatorname{line}(i,j)=\left\lfloor\frac{\operatorname{address}(i,j)}{16}\right\rfloor=i.
$$

Here $\lfloor\cdot\rfloor$ is the [floor function](floor-function.md). Each row occupies exactly one [cache line](cache-line.md): row zero begins at addresses $0,4,8,12$, row one at $16,20,24,28$, and so on. [Row-major order](row-major-order.md) describes this storage layout; traversal can follow rows or columns without moving the elements.

<a id="image-two-traversal-paths-through-the-same-row-major-array-coloured-by-physical-cache-line"></a>
![](array-traversal-spatial-locality.png)

**[Figure 20](#image-two-traversal-paths-through-the-same-row-major-array-coloured-by-physical-cache-line). Two traversal paths through the same row-major array, coloured by physical cache line**.

Read all sixteen elements and compute their [integer](integer.md) sum, keeping the accumulator outside the modelled [memory cache](cache-computing.md). Only the sixteen [array](array-data-structure.md) reads count as [memory references](memory-reference.md). The toy [fully associative cache](fully-associative-cache.md) starts empty, holds exactly one 16-[byte](byte.md) [cache line](cache-line.md), fetches the requested [cache block](cache-line.md) on every [cache miss](cache-miss.md), and uses [LRU replacement](lru-replacement.md). No [cache block](cache-line.md) is fetched ahead of a request, and no writeback costs are counted because the modelled accesses are reads.

- Traversing by rows, with $j$ varying fastest, requests [cache blocks](cache-line.md) $0,0,0,0,1,1,1,1,2,2,2,2,3,3,3,3$. Each first read in a row is a [cache miss](cache-miss.md); the next three are [cache hits](cache-hit.md). Total: four [cache misses](cache-miss.md) and twelve [cache hits](cache-hit.md) in sixteen [memory references](memory-reference.md).
- Traversing by columns, with $i$ varying fastest, requests [cache blocks](cache-line.md) $0,1,2,3$ four times. Every read replaces the sole resident [cache line](cache-line.md), so the next read always causes a [cache miss](cache-miss.md). Total: sixteen [cache misses](cache-miss.md) and zero [cache hits](cache-hit.md) in sixteen [memory references](memory-reference.md).

<a id="image-all-sixteen-memory-references-and-their-cache-hits-or-cache-misses-with-capacity-one-cache-line"></a>
![](cache-line-traversal-misses.png)

**[Figure 21](#image-all-sixteen-memory-references-and-their-cache-hits-or-cache-misses-with-capacity-one-cache-line). All sixteen memory references and their cache hits or cache misses with capacity one cache line**.

Every element is read once in both traversals. The row traversal exploits [spatial locality](spatial-locality.md) between distinct elements and [temporal locality](temporal-locality.md) of their shared [cache block](cache-line.md). The column traversal returns to each [cache block](cache-line.md) after three other distinct [cache blocks](cache-line.md), too late for the one-line [memory cache](cache-computing.md). Increase the [fully associative cache](fully-associative-cache.md) to four [cache lines](cache-line.md) and both traversals give four [compulsory misses](compulsory-miss.md) and twelve [cache hits](cache-hit.md): no loaded [cache block](cache-line.md) needs eviction. The difference therefore depends on capacity as well as access order and layout.

This makes [spatial locality](spatial-locality.md) useful and beautiful: the same logical operation on the same elements can use a fetched [cache line](cache-line.md) much more fully simply by changing traversal order. The toy counts do not predict a universal speed ratio on real hardware. Actual [cache line](cache-line.md) sizes, capacities, placement rules, fetching ahead of requests and overlapping work affect runtime; measure a concrete implementation with [statistical program profiling](statistical-program-profiling.md). Ulrich Drepper's November 2007 authored paper explains [cache line](cache-line.md) transfers and gives [array](array-data-structure.md) and [matrix](matrix.md) access examples connecting layout, [temporal locality](temporal-locality.md) and [spatial locality](spatial-locality.md). Its hardware measurements are historical examples, rather than specifications for every present-day [CPU](central-processing-unit.md). [Ulrich Drepper, What Every Programmer Should Know About Memory, sections 3.2 and 6.2.1: cache operation and optimizing data-cache access](https://www.akkadia.org/drepper/cpumemory.pdf)

// Destination: computer-science.bigb

## ↑ Ancestors (2)

1. [Computer science](computer-science-split.md)
2. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Cache (computing)](cache-computing.md)
- [Cache hit](cache-hit.md)
- [Cache line](cache-line.md)
- [Cache miss](cache-miss.md)
- [Fully associative cache](fully-associative-cache.md)
- [Page replacement](page-replacement.md)
- [Row-major order](row-major-order.md)
- [Spatial locality](spatial-locality.md)
- [Temporal locality](temporal-locality.md)
