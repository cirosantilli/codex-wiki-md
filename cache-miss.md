# Cache miss

↑ **Parent:** [Cache (computing)](cache-computing.md)

A request whose required data are unavailable in the consulted [memory cache](cache-computing.md). The model in [spatial locality](spatial-locality.md) fetches the requested [cache block](cache-line.md) and evicts a resident [cache line](cache-line.md) only when capacity is full.

In the fixed [memory access trace](memory-access-trace.md) under [memory cache](cache-computing.md), reads 1, 3, 5 and 8 first request [cache blocks](cache-line.md) 0, 2, 1 and 3: four [compulsory misses](compulsory-miss.md), also called cold misses. Reads 6, 7 and 11 revisit [cache blocks](cache-line.md) that [LRU replacement](lru-replacement.md) has evicted: three [capacity misses](capacity-miss.md). Read 5 is a [compulsory miss](compulsory-miss.md) even though it also causes an eviction; a full [memory cache](cache-computing.md) alone does not determine the classification. The [fully associative cache](fully-associative-cache.md) permits every [cache block](cache-line.md) in every [cache slot](cache-slot.md), so this example has no [conflict misses](conflict-miss.md).

For a precise comparison, run the same [memory access trace](memory-access-trace.md) through an initially empty [direct-mapped cache](direct-mapped-cache.md) with the same 16-[byte](byte.md) [cache lines](cache-line.md) and two [cache slots](cache-slot.md), placing [cache block](cache-line.md) $q$ only in slot $q\bmod2$. Read 3 brings in [cache block](cache-line.md) 2 and displaces [cache block](cache-line.md) 0, leaving the other [cache slot](cache-slot.md) unused. Read 4 consequently misses at address 0, whereas the [fully associative cache](fully-associative-cache.md) still has [cache block](cache-line.md) 0. That read is a [conflict miss](conflict-miss.md): increasing placement freedom at the same capacity removes it. The complete [direct-mapped cache](direct-mapped-cache.md) trace has eight [cache misses](cache-miss.md): four [compulsory misses](compulsory-miss.md), three [capacity misses](capacity-miss.md) and one [conflict miss](conflict-miss.md).

The convention here classifies each [cache miss](cache-miss.md) by first asking whether its [cache block](cache-line.md) has ever been requested. If so, compare with an initially empty [fully associative cache](fully-associative-cache.md) of the same capacity and [cache line](cache-line.md) size using [LRU replacement](lru-replacement.md) on the same [memory access trace](memory-access-trace.md): a miss there is a [capacity miss](capacity-miss.md), while a hit there identifies a [conflict miss](conflict-miss.md) in the restricted design. This makes the comparison policy explicit; “capacity” is not a claim that no other replacement choice could save that individual read. The three categories describe this read-only demand model; external invalidations or fetching ahead of requests require additional reasoning. [11.4. CPU Caches](dive-into-systems-by-suzanne-j-matthews-and-others/11-4-cpu-caches.md)

**Table of contents**

- [Cache miss rate](cache-miss-rate.md)
- [Capacity miss](capacity-miss.md)
- [Conflict miss](conflict-miss.md)
- [Cache miss penalty](cache-miss-penalty.md)
- [Compulsory miss](compulsory-miss.md)

## ↑ Ancestors (4)

1. [Cache (computing)](cache-computing.md)
2. [Computer memory](computer-memory.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Average memory access time](average-memory-access-time.md)
- [Buffer cache access trace](buffer-cache-access-trace.md)
- [Buffer cache eviction](buffer-cache-eviction.md)
- [Buffer cache validity](buffer-cache-validity.md)
- [Cache (computing)](cache-computing.md)
- [Cache hit](cache-hit.md)
- [Cache miss](cache-miss.md)
- [Cache miss penalty](cache-miss-penalty.md)
- [Cache miss rate](cache-miss-rate.md)
- [Compulsory miss](compulsory-miss.md)
- [Conflict miss](conflict-miss.md)
- [Direct-mapped cache](direct-mapped-cache.md)
- [Fully associative cache](fully-associative-cache.md)
- [Microkernel communication cost](microkernel-communication-cost.md)
- [Spatial locality](spatial-locality.md)
- [Temporal locality](temporal-locality.md)
- [xv6 buffer cache](xv6-buffer-cache.md)
