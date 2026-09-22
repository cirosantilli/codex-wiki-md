# Fully associative cache

↑ **Parent:** [Cache (computing)](cache-computing.md)

A [memory cache](cache-computing.md) allowing any [cache block](cache-line.md) to occupy any resident slot. When full, its replacement policy chooses a victim from all resident [cache lines](cache-line.md). The examples in [temporal locality](temporal-locality.md) and [spatial locality](spatial-locality.md) use [LRU replacement](lru-replacement.md), so no additional placement restriction causes eviction.

The diagram enumerates every read of the fixed [memory access trace](memory-access-trace.md) under [memory cache](cache-computing.md). Keep [cache slots](cache-slot.md) fixed: fill the lowest-numbered unused slot first, and subsequently reuse the victim's slot. Separately list recency from least recently used to most recently used. A [cache hit](cache-hit.md) refreshes that recency without moving the resident data to another [cache slot](cache-slot.md).

<a id="image-every-read-cache-hit-or-cache-miss-eviction-cache-slot-and-recency-state-of-the-synthetic-two-slot-fully-associative-cache-with-lru-replacement"></a>
![](fully-associative-lru-read-trace.png)

**[Figure 74](#image-every-read-cache-hit-or-cache-miss-eviction-cache-slot-and-recency-state-of-the-synthetic-two-slot-fully-associative-cache-with-lru-replacement). Every read, cache hit or cache miss, eviction, cache slot and recency state of the synthetic two-slot fully associative cache with LRU replacement**.

After read 3, [cache block](cache-line.md) 0 is older than [cache block](cache-line.md) 2. Read 4 hits [cache block](cache-line.md) 0, making [cache block](cache-line.md) 2 older; read 5 must therefore evict [cache block](cache-line.md) 2 to load [cache block](cache-line.md) 1. Omitting recency updates on [cache hits](cache-hit.md) would choose the wrong victim. Read 6 immediately needs the evicted [cache block](cache-line.md) 2, showing that [LRU replacement](lru-replacement.md) uses past demand rather than knowledge of future demand.

With capacity four [cache slots](cache-slot.md) and the same [cache line](cache-line.md) size, the same [memory access trace](memory-access-trace.md) has just its four [compulsory misses](compulsory-miss.md) and eight [cache hits](cache-hit.md), since all four distinct [cache blocks](cache-line.md) fit. Greater capacity helps this trace, but full associativity alone does not make [LRU replacement](lru-replacement.md) optimal. Its attraction is freedom from placement restrictions; a hardware implementation must still identify a matching [cache tag](cache-tag.md) among eligible entries, and exact recency tracking adds work. [Memory part 2: CPU caches by Ulrich Drepper](memory-part-2-cpu-caches-by-ulrich-drepper.md)

## ↑ Ancestors (4)

1. [Cache (computing)](cache-computing.md)
2. [Computer memory](computer-memory.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Average memory access time](average-memory-access-time.md)
- [Cache (computing)](cache-computing.md)
- [Cache hit rate](cache-hit-rate.md)
- [Cache line](cache-line.md)
- [Cache miss](cache-miss.md)
- [Cache miss rate](cache-miss-rate.md)
- [Cache tag](cache-tag.md)
- [Capacity miss](capacity-miss.md)
- [Conflict miss](conflict-miss.md)
- [Fully associative cache](fully-associative-cache.md)
- [Spatial locality](spatial-locality.md)
- [Temporal locality](temporal-locality.md)
