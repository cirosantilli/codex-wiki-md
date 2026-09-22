# Cache hit

↑ **Parent:** [Cache (computing)](cache-computing.md)

A request whose required data are already available in the consulted [memory cache](cache-computing.md). In the read-only model of [spatial locality](spatial-locality.md), a requested [cache block](cache-line.md) being resident is sufficient for a [cache hit](cache-hit.md).

The [memory access trace](memory-access-trace.md) under [memory cache](cache-computing.md) has [cache hits](cache-hit.md) at reads 2, 4, 9, 10 and 12. Read 2, at address 4, benefits from the [cache line](cache-line.md) fetched by read 1 at address 0; read 9, at address 52, benefits from read 8 at address 48. These reads use different [bytes](byte.md) of the same [cache blocks](cache-line.md), illustrating [spatial locality](spatial-locality.md). Read 4 returns to address 0 while its [cache block](cache-line.md) remains resident, illustrating [temporal locality](temporal-locality.md).

A [cache hit](cache-hit.md) still takes time to identify the matching [cache tag](cache-tag.md) and obtain the requested [byte](byte.md). It is relative to the particular [memory cache](cache-computing.md) consulted: a [cache miss](cache-miss.md) in one level may be a [cache hit](cache-hit.md) in another. The model here has one consulted level and treats a valid matching resident copy as sufficient; it makes no prediction about writes or accesses whose permissions or contents change.

**Table of contents**

- [Cache hit rate](cache-hit-rate.md)

## ↑ Ancestors (4)

1. [Cache (computing)](cache-computing.md)
2. [Computer memory](computer-memory.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Average memory access time](average-memory-access-time.md)
- [Buffer cache](buffer-cache.md)
- [Buffer cache access trace](buffer-cache-access-trace.md)
- [Buffer cache validity](buffer-cache-validity.md)
- [Cache (computing)](cache-computing.md)
- [Cache hit](cache-hit.md)
- [Cache hit rate](cache-hit-rate.md)
- [Cache miss rate](cache-miss-rate.md)
- [Clean buffer](clean-buffer.md)
- [Fully associative cache](fully-associative-cache.md)
- [Memoization](memoization.md)
- [Memory access trace](memory-access-trace.md)
- [Spatial locality](spatial-locality.md)
- [Temporal locality](temporal-locality.md)
